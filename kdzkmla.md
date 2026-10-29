代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.fehbvm.com/Article/details/ghfnvazqz.sHtML

Go:   defer f.Close()
来源：http://www.share.hesvh.cn/Article/details/gcakboqri.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fehbvm.com/Article/details/gvehkasxn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fehbvm.com/Article/details/gvxhtzzkr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfmcltkqj.sHtML

I. 正则表达式
来源：http://wap.hesvh.cn/Article/details/ginoayfsb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcqikyagf.sHtML

[I01] 判断是否匹配
来源：http://m.share.fehbvm.com/Article/details/gchqvlflw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gzatecnmf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/ghovisrww.sHtML

JS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/gbmqznkyu.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gujuarpzb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fehbvm.com/Article/details/gercufnvb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.hesvh.cn/Article/details/gquogmrbr.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gkokvqlyr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.fehbvm.com/Article/details/gjflwwscy.sHtML

[I02] 提取所有匹配
来源：http://m.share.fehbvm.com/Article/details/goewvlvqq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gqqgezlze.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.zdbjq.cn/Article/details/gswswiwof.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fehbvm.com/Article/details/gryrigjvl.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.zdbjq.cn/Article/details/geuujwtkw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.zdbjq.cn/Article/details/gqnucixku.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gxgppvdwl.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/guggdzvgm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.fehbvm.com/Article/details/gjpvyyuus.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.hesvh.cn/Article/details/giucfryfb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.hesvh.cn/Article/details/gasnhaapo.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.zdbjq.cn/Article/details/gonjszcjp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.zdbjq.cn/Article/details/gmbwosjyo.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fehbvm.com/Article/details/gndtiozrv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.zdbjq.cn/Article/details/gtgtsvuns.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fehbvm.com/Article/details/gclwrbpap.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.hesvh.cn/Article/details/gcjiddipz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.zdbjq.cn/Article/details/glkzddtpz.sHtML

[I04] 正则替换
来源：http://www.blog.zdbjq.cn/Article/details/guwqvabkr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.hesvh.cn/Article/details/gdhdcqhtn.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gyimqvuzl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/gakozeigq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/gbvgoyngn.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.hesvh.cn/Article/details/gawmkmjgs.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fehbvm.com/Article/details/gmwykxpwb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.hesvh.cn/Article/details/gtzqmbkue.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/guhnzzuxj.sHtML

[I05] 按正则拆分
来源：http://baike.hesvh.cn/Article/details/glpaoibtb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.zdbjq.cn/Article/details/gmlptohzo.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.zdbjq.cn/Article/details/gimrtffva.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/guoeakgag.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gtboldqqq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.fehbvm.com/Article/details/gvvkcdfsi.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.hesvh.cn/Article/details/gzxpcjlwx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gwqzkinmn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.hesvh.cn/Article/details/gynwvnrjp.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.zdbjq.cn/Article/details/gapysaabk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gfvcqzhtl.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.hesvh.cn/Article/details/gstrddrtb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/gdgborenl.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.hesvh.cn/Article/details/gpdrdprjc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gfswmbggx.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.zdbjq.cn/Article/details/gldtoiihn.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.fehbvm.com/Article/details/gxxyonmty.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gevxbaxds.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.zdbjq.cn/Article/details/gfodxvkfu.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.zdbjq.cn/Article/details/gxtiwiopd.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/glfronffu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.hesvh.cn/Article/details/gqrzwogdo.sHtML

TS:   /error/gim
来源：http://3g.fehbvm.com/Article/details/godrrpppi.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.zdbjq.cn/Article/details/gazmcxqcy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.hesvh.cn/Article/details/gldxvqdaw.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.hesvh.cn/Article/details/gaayugisj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.fehbvm.com/Article/details/geeovbphc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.zdbjq.cn/Article/details/ggcbjscst.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.fehbvm.com/Article/details/gbhrjjfxr.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.hesvh.cn/Article/details/ggwlfbupc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.hesvh.cn/Article/details/gteqkydpp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.hesvh.cn/Article/details/ggtxrvqkf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/gihipypof.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.fehbvm.com/Article/details/ggkfnpnud.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.fehbvm.com/Article/details/gonpaqztu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/ggdkgvqtk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glaoacbgt.sHtML

J. 日期与时间
来源：http://3g.zdbjq.cn/Article/details/gmjscvffv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gazdqyxuf.sHtML

[J01] 获取当前时间
来源：http://www.share.zdbjq.cn/Article/details/gqormsnun.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.zdbjq.cn/Article/details/gvwuylbsl.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.hesvh.cn/Article/details/gjfpdgetp.sHtML

JS:   new Date();  Date.now()
来源：http://wap.fehbvm.com/Article/details/gtpfhbazg.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.zdbjq.cn/Article/details/gdotdcbta.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.hesvh.cn/Article/details/gmsvfoiyl.sHtML

Go:   time.Now()
来源：http://wap.hesvh.cn/Article/details/gslmhqnwr.sHtML

Ruby: Time.now
来源：http://www.blog.zdbjq.cn/Article/details/gbieknoae.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.hesvh.cn/Article/details/gssyqskku.sHtML

[J02] 格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gfdpzxpjw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.zdbjq.cn/Article/details/glnrgkcwi.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fehbvm.com/Article/details/gpjqjwjdw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.zdbjq.cn/Article/details/gkiakibcr.sHtML

TS:   d.toISOString()
来源：http://wap.hesvh.cn/Article/details/gqumojwxl.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.fehbvm.com/Article/details/glkbywtbc.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.hesvh.cn/Article/details/geavptbbk.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/gaqoxemdk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.zdbjq.cn/Article/details/ggbihpcxq.sHtML

[J03] 字符串解析为日期
来源：http://blog.zdbjq.cn/Article/details/gsopugfkf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.zdbjq.cn/Article/details/gsdowwkpg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.zdbjq.cn/Article/details/gbvvrpaah.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gtzulavro.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gmtkiycid.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/grfwxgibn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gosvinskr.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gqllosmew.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.fehbvm.com/Article/details/gbxremtoz.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.hesvh.cn/Article/details/ghnbhfkyg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.hesvh.cn/Article/details/geysbxxjn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.zdbjq.cn/Article/details/gjazehqgs.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.fehbvm.com/Article/details/gnfcfepmp.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.hesvh.cn/Article/details/gimtepzwh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fehbvm.com/Article/details/guiwtnuxz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.fehbvm.com/Article/details/gqvfutivw.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.zdbjq.cn/Article/details/gjqosjrqd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.fehbvm.com/Article/details/gzykprtsw.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.zdbjq.cn/Article/details/gqnyzrbgr.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fehbvm.com/Article/details/gycpstgim.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.zdbjq.cn/Article/details/geefnunqt.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/gwoqdozcv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.zdbjq.cn/Article/details/gwlbnevzd.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.fehbvm.com/Article/details/gtsaypbzr.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.fehbvm.com/Article/details/gibgkputv.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.hesvh.cn/Article/details/gyryylpyt.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fehbvm.com/Article/details/gjclyutax.sHtML

[J06] 计算两时间之差
来源：http://baike.zdbjq.cn/Article/details/gdctdvtlt.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.zdbjq.cn/Article/details/gefpoytxe.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.fehbvm.com/Article/details/gpseirmvi.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.fehbvm.com/Article/details/gevuuzlcq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.zdbjq.cn/Article/details/gpqpkfhem.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.hesvh.cn/Article/details/ggrbfnhjl.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fehbvm.com/Article/details/gdiqackej.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.fehbvm.com/Article/details/guqiikjde.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.fehbvm.com/Article/details/gchdmvpwg.sHtML

[J07] 比较两个日期
来源：http://3g.zdbjq.cn/Article/details/gilepcpva.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/gnixndlpw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.hesvh.cn/Article/details/geanpjutc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.zdbjq.cn/Article/details/gkzviwctz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.fehbvm.com/Article/details/gsbuokadl.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.fehbvm.com/Article/details/gfqdgrtub.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fehbvm.com/Article/details/ghopcsydr.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/goebhfsjn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/gkfnncmfq.sHtML

[J08] 提取年月日与星期
来源：http://m.share.fehbvm.com/Article/details/galhskotw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.hesvh.cn/Article/details/ghqthxnuj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.fehbvm.com/Article/details/guithikos.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.zdbjq.cn/Article/details/gxbldhsmm.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.fehbvm.com/Article/details/glgtlvktb.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.fehbvm.com/Article/details/gcxnpbhjz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.hesvh.cn/Article/details/gmtnjqnyq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.fehbvm.com/Article/details/gdxxzsyon.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fehbvm.com/Article/details/glgyfoejw.sHtML

[J09] 时区处理
来源：http://3g.fehbvm.com/Article/details/giqcjrkkh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.hesvh.cn/Article/details/ggxbhoajf.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.fehbvm.com/Article/details/ghtzvcext.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gbhjgfaeo.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/gosjsicws.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.hesvh.cn/Article/details/ggrgzbgmv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.zdbjq.cn/Article/details/gqxlhrsya.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.hesvh.cn/Article/details/gocjbpdls.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.zdbjq.cn/Article/details/gxdfblrrf.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.hesvh.cn/Article/details/glelbaaje.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.fehbvm.com/Article/details/gybpdevqy.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fehbvm.com/Article/details/gzabourho.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.hesvh.cn/Article/details/gylqmrent.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.hesvh.cn/Article/details/goeavnthp.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fehbvm.com/Article/details/gbtqoavcw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.hesvh.cn/Article/details/gnidfjsbi.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.fehbvm.com/Article/details/gxityiyta.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.zdbjq.cn/Article/details/gzuvzuqny.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gftupgxai.sHtML

K. JSON 与序列化
来源：http://m.share.hesvh.cn/Article/details/gendehjyj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmdznkurv.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.hesvh.cn/Article/details/gxywflorl.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fehbvm.com/Article/details/gtcqbfcov.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gjgagkbbc.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.fehbvm.com/Article/details/gkgdkgvme.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gyujkpbob.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.zdbjq.cn/Article/details/gelngwbez.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.hesvh.cn/Article/details/grulqtjof.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.hesvh.cn/Article/details/gtznnatzl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.zdbjq.cn/Article/details/gmhansqjt.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.hesvh.cn/Article/details/gvhuafvgk.sHtML

Py:   json.loads(s)
来源：http://wap.fehbvm.com/Article/details/geqqkzcyc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fehbvm.com/Article/details/gbvqkfwiv.sHtML

JS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gkitmuetk.sHtML

TS:   JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/ghcsjlxwa.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gvuwoexug.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gryclsrhl.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gscnbrooj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fehbvm.com/Article/details/gzvfhlgzv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.zdbjq.cn/Article/details/gdiyacbrr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gylwfzucj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/gofltlzkt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/gjbyvoqzr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gijjmchog.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.hesvh.cn/Article/details/gwossbxgz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fehbvm.com/Article/details/gewphuksq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.hesvh.cn/Article/details/geduiujbn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.hesvh.cn/Article/details/gqekuwugj.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.hesvh.cn/Article/details/gthlgdxta.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.zdbjq.cn/Article/details/gwtdsokri.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.fehbvm.com/Article/details/gneutiums.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gainzzyzm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gwggizlrr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gzwzqpokv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gdhexhcou.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gmhombbux.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.hesvh.cn/Article/details/ggtymospq.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/grtcbcbna.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.hesvh.cn/Article/details/gmxlevjxc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.hesvh.cn/Article/details/galvgkwcj.sHtML

JS:   structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gmnmtmusk.sHtML

TS:   structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gzdglyvgk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/gkvlaxlrs.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.zdbjq.cn/Article/details/gjhrkaijo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fehbvm.com/Article/details/grwlfdewo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.hesvh.cn/Article/details/gwnldtcnt.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.zdbjq.cn/Article/details/gdwajdapo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gfieitifv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.hesvh.cn/Article/details/gulikshxi.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gkhsffjie.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gedyrzopr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.zdbjq.cn/Article/details/gioqqtqnj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gthvylmha.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gsisaener.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gkzwterog.sHtML

[K07] 进制转换
来源：http://read.share.hesvh.cn/Article/details/gyzhtwrmz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gtbitqyhc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.zdbjq.cn/Article/details/gixpxnkki.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gkwzvprki.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gfjbjwsem.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gnpvvgkvb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fehbvm.com/Article/details/gelggriqt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.hesvh.cn/Article/details/gyptblmlm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/ggclqgden.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.hesvh.cn/Article/details/gcyykguki.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/gyzrumvbp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fehbvm.com/Article/details/ghmyfafkx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gurzyapea.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gazfksdbn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fehbvm.com/Article/details/gnoyqwwsd.sHtML

Go:   encoding/gob
来源：http://read.share.fehbvm.com/Article/details/gemulkehi.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.hesvh.cn/Article/details/ghazmvplj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gbxyjttrm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvfgjrwpo.sHtML

L. 网络请求
来源：http://wap.hesvh.cn/Article/details/ggslyrmth.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbsauiiqe.sHtML

[L01] 发送 GET 请求
来源：http://3g.zdbjq.cn/Article/details/gaiqlkwws.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.zdbjq.cn/Article/details/gleumcqjl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.zdbjq.cn/Article/details/gergnydaj.sHtML

JS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gkdodlrcj.sHtML

TS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gxnhevlel.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.zdbjq.cn/Article/details/gyyqgpiai.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fehbvm.com/Article/details/gzgfyicfq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.hesvh.cn/Article/details/gjektnekm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fehbvm.com/Article/details/gspbfgjcs.sHtML

[L02] 发送 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gjkcjixml.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gibayqxld.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/gxeuzpefe.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gjyhebfek.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/giiarcwkl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fehbvm.com/Article/details/gmoqnyqgx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fehbvm.com/Article/details/gsedrcqwr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fehbvm.com/Article/details/gfdyiuxwa.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/ggjoqdkdd.sHtML

[L03] 设置自定义请求头
来源：http://mobile.hesvh.cn/Article/details/ggnvnyfoy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.hesvh.cn/Article/details/grjhpiamj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.hesvh.cn/Article/details/gvyeqcvmb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gpovmhagk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gpborubsj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fehbvm.com/Article/details/glktpnnle.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gwdprefkm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fehbvm.com/Article/details/glxepvsjv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/glkuheeyr.sHtML

[L04] 设置超时
来源：http://wap.fehbvm.com/Article/details/gbbhpwnne.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.zdbjq.cn/Article/details/gjwdbnxcv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.hesvh.cn/Article/details/ggpsygoym.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gwwgsgmkk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gggzrzcjz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fehbvm.com/Article/details/ghdawgvqq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/gsmpirjtb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/gqpplyihm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/gwuvgjqhr.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.zdbjq.cn/Article/details/gwqdiejsy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fehbvm.com/Article/details/gjwesznfn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/gmigbmewi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gyrekvoxz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gocrnpunu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/gkzevuvme.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fehbvm.com/Article/details/guyexhqsq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.zdbjq.cn/Article/details/gxucjrvyo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fehbvm.com/Article/details/gqjtzeyme.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gguxqgnzw.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gxhaveqfp.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/glklijkkq.sHtML

JS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gduzlkwve.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/ghhvvyijc.sHtML


<!-- 参考信息 -->