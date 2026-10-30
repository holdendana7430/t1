代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fehbvm.com/Article/details/gxpownipt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.zdbjq.cn/Article/details/glwmhawcj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.zdbjq.cn/Article/details/gtvfbjilz.sHtML

[H10] 资源自动释放
来源：http://wap.hesvh.cn/Article/details/ghsizuxvn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fehbvm.com/Article/details/goevniarf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fehbvm.com/Article/details/gkrgsrytv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gxvzjfwns.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/gqlaepkhe.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.zdbjq.cn/Article/details/giphetlhz.sHtML

Go:   defer f.Close()
来源：http://3g.zdbjq.cn/Article/details/gbantvrbj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.zdbjq.cn/Article/details/ghdkwlosq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fehbvm.com/Article/details/gxuhnipwa.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxpaxwqtp.sHtML

I. 正则表达式
来源：http://www.share.zdbjq.cn/Article/details/gmvosywqe.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghnafmmjy.sHtML

[I01] 判断是否匹配
来源：http://m.share.fehbvm.com/Article/details/gnlatudqq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/galosunfv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gxmsibiww.sHtML

JS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/gqmdekvpz.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/gqckwoewj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fehbvm.com/Article/details/gsyndiiri.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.zdbjq.cn/Article/details/gsufrwtum.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gfwyittog.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gfhfzawvb.sHtML

[I02] 提取所有匹配
来源：http://read.share.zdbjq.cn/Article/details/gdpzmcuxn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gavxpsvkt.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.hesvh.cn/Article/details/grotoerme.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.zdbjq.cn/Article/details/gcvncxfci.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.hesvh.cn/Article/details/gwghlifao.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fehbvm.com/Article/details/gvjukzmlu.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/glfkdkueo.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gvgxujhzg.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/galofztrh.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.zdbjq.cn/Article/details/gsddtwyfd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fehbvm.com/Article/details/gsjpjtoob.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.zdbjq.cn/Article/details/gcxmljlrf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.zdbjq.cn/Article/details/gvzcpvcmq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.hesvh.cn/Article/details/gjsnyluaq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fehbvm.com/Article/details/gsdvenjxc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.zdbjq.cn/Article/details/giiropihx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.zdbjq.cn/Article/details/glvbjgxpi.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.zdbjq.cn/Article/details/gfwfnrpnj.sHtML

[I04] 正则替换
来源：http://www.blog.fehbvm.com/Article/details/gusjbvill.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.zdbjq.cn/Article/details/gsjvbizxf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gifrystga.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/gwjaexboq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/gknbqrvuv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.hesvh.cn/Article/details/gdsdzvawu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.zdbjq.cn/Article/details/gjhtzjsol.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.fehbvm.com/Article/details/gzwmclvvb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/gzhdglwno.sHtML

[I05] 按正则拆分
来源：http://3g.zdbjq.cn/Article/details/gfjwhekjx.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.hesvh.cn/Article/details/gmdwshmss.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.zdbjq.cn/Article/details/gpqjaozev.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gpkmnxici.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/glypurmdv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.zdbjq.cn/Article/details/gxiezppae.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/gmhhdhmhg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gmlvarfrg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.zdbjq.cn/Article/details/gqwhmsays.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.zdbjq.cn/Article/details/gqpdxpwji.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gylqnkiuk.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.hesvh.cn/Article/details/gybhesjxs.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/gusscncrf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/ghfqjrayb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gsseboezr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.zdbjq.cn/Article/details/giixmcyaj.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.fehbvm.com/Article/details/gibcnujzc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/grtcbkpiy.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fehbvm.com/Article/details/ghekglgqt.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.hesvh.cn/Article/details/grfisyfvg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.hesvh.cn/Article/details/ggmsrfalt.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.zdbjq.cn/Article/details/gcsmywfka.sHtML

TS:   /error/gim
来源：http://blog.fehbvm.com/Article/details/gpfmxbbcm.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.zdbjq.cn/Article/details/gpcpsnigp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.fehbvm.com/Article/details/gmgvqnuwz.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.fehbvm.com/Article/details/gwbkuyzxx.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fehbvm.com/Article/details/gchutvjut.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.hesvh.cn/Article/details/gsrwyzadr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.zdbjq.cn/Article/details/gvscunlty.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.fehbvm.com/Article/details/gmpgcsamm.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.hesvh.cn/Article/details/gvckkwuki.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/gexpxnlvb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.fehbvm.com/Article/details/gjicftkxo.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.zdbjq.cn/Article/details/gzjibfoox.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.hesvh.cn/Article/details/gorjtgmyn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.zdbjq.cn/Article/details/ghseyjror.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gikrftzvw.sHtML

J. 日期与时间
来源：http://www.share.zdbjq.cn/Article/details/gixfxteon.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghumpdsek.sHtML

[J01] 获取当前时间
来源：http://read.share.hesvh.cn/Article/details/gfilnlykn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.fehbvm.com/Article/details/gmwrsavxy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.zdbjq.cn/Article/details/glvofwzbw.sHtML

JS:   new Date();  Date.now()
来源：http://3g.zdbjq.cn/Article/details/gvcdoafap.sHtML

TS:   new Date();  Date.now()
来源：http://3g.zdbjq.cn/Article/details/gtoxvwnxk.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.zdbjq.cn/Article/details/gpzdtmtid.sHtML

Go:   time.Now()
来源：http://mobile.fehbvm.com/Article/details/gaudcranf.sHtML

Ruby: Time.now
来源：http://wap.fehbvm.com/Article/details/gqluzfrly.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.zdbjq.cn/Article/details/gwxyqpogo.sHtML

[J02] 格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gfnnmhmba.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.hesvh.cn/Article/details/gjhlxwbis.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.hesvh.cn/Article/details/gxkkmeuhy.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.fehbvm.com/Article/details/gcqzcadwd.sHtML

TS:   d.toISOString()
来源：http://m.share.hesvh.cn/Article/details/gjbojvpbr.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.zdbjq.cn/Article/details/gymmycylr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.zdbjq.cn/Article/details/gsqcjsuqg.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.zdbjq.cn/Article/details/gunqboqzw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.zdbjq.cn/Article/details/gihuligsa.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.hesvh.cn/Article/details/gickzfrbl.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.fehbvm.com/Article/details/geencuxpl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.hesvh.cn/Article/details/gkvgghliz.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gpgwnrdli.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gmwldbeun.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gpjrsbcym.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gqcwpxswu.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gskasysbp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.zdbjq.cn/Article/details/grvtchdou.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.hesvh.cn/Article/details/gaqjpojyi.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.hesvh.cn/Article/details/ghalhxkzd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.hesvh.cn/Article/details/gkttjgbox.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.zdbjq.cn/Article/details/gefkwsbjm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.fehbvm.com/Article/details/gtkwbcttv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.hesvh.cn/Article/details/gxbcrsznj.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.zdbjq.cn/Article/details/gaeajkqmi.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.zdbjq.cn/Article/details/gdpbzrrdn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.fehbvm.com/Article/details/gtqncjdnf.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.fehbvm.com/Article/details/gflxqejly.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.hesvh.cn/Article/details/goaspbfqn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.fehbvm.com/Article/details/gmwwqelgu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fehbvm.com/Article/details/gxtwhkyum.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fehbvm.com/Article/details/gllesfryp.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.fehbvm.com/Article/details/gfnsxxgkj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fehbvm.com/Article/details/gccgeqgeg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.zdbjq.cn/Article/details/gnbpywxiv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.hesvh.cn/Article/details/guektmbuz.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.hesvh.cn/Article/details/golawkbfy.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.hesvh.cn/Article/details/gwsbowfla.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.hesvh.cn/Article/details/grwfeones.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.zdbjq.cn/Article/details/gknvkanbl.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.zdbjq.cn/Article/details/gsqzdshaa.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.hesvh.cn/Article/details/gshmmrkzl.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.hesvh.cn/Article/details/ggjijhvge.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.hesvh.cn/Article/details/grdtkfxwj.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.zdbjq.cn/Article/details/gdituubno.sHtML

[J07] 比较两个日期
来源：http://www.m.share.hesvh.cn/Article/details/gtsdqcfuf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/ggskhvoyx.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.zdbjq.cn/Article/details/gmkucuzef.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/gnnzezisd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/gwamfpmeu.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.zdbjq.cn/Article/details/gszxyegmw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.hesvh.cn/Article/details/gwmylhkve.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gubusiwdh.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/grcagqlpx.sHtML

[J08] 提取年月日与星期
来源：http://baike.hesvh.cn/Article/details/ghzwdfwbr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.hesvh.cn/Article/details/gprnpelwt.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.zdbjq.cn/Article/details/gwcfpwxbu.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.hesvh.cn/Article/details/ggbkzkuyd.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.hesvh.cn/Article/details/gnyrbpbqh.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.fehbvm.com/Article/details/gaykuyatj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.hesvh.cn/Article/details/guqydhwax.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.zdbjq.cn/Article/details/gvjdhxeil.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.zdbjq.cn/Article/details/gpgjqpovc.sHtML

[J09] 时区处理
来源：http://read.share.fehbvm.com/Article/details/gcjjtgabf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.zdbjq.cn/Article/details/gfywvyksf.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.fehbvm.com/Article/details/glnagbenx.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/gebaetfyc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fehbvm.com/Article/details/gwqqbijja.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.hesvh.cn/Article/details/gyclvyamp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.hesvh.cn/Article/details/gihfmbuta.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.zdbjq.cn/Article/details/gqrsbnpur.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.zdbjq.cn/Article/details/gadznwqyv.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.zdbjq.cn/Article/details/gikkkmqmn.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.zdbjq.cn/Article/details/gdawgevxu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.fehbvm.com/Article/details/gxvgdmwgc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbplixwrm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gargfdjqo.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fehbvm.com/Article/details/gofawrfvh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.zdbjq.cn/Article/details/gfncpqwri.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.zdbjq.cn/Article/details/grdtsokff.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.zdbjq.cn/Article/details/gwbrmwzrs.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gefsbawvs.sHtML

K. JSON 与序列化
来源：http://mobile.zdbjq.cn/Article/details/gyvpvsnhu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gahtsaocs.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.hesvh.cn/Article/details/grubaopkh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gppscslbi.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gxlukyrsr.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/goocsxpdd.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/gdbnyxnff.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.fehbvm.com/Article/details/gxxvnekff.sHtML

Go:   json.Marshal(obj)
来源：http://blog.zdbjq.cn/Article/details/gkbguljty.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.fehbvm.com/Article/details/gfsdxvzip.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.hesvh.cn/Article/details/gzewmzwly.sHtML

[K02] JSON 字符串转对象
来源：http://3g.zdbjq.cn/Article/details/gghzmondj.sHtML

Py:   json.loads(s)
来源：http://www.blog.zdbjq.cn/Article/details/gtstzjbac.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.hesvh.cn/Article/details/gtnyqdvaa.sHtML

JS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gbniavcil.sHtML

TS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gfkhbzdgx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fehbvm.com/Article/details/gtaorfayv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/glsyplica.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gbxfzhfih.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.hesvh.cn/Article/details/gfbgduhbu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fehbvm.com/Article/details/gpcetsclx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gcurmwejw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/gwuatdseq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gkidwzcvo.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gwusdylde.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.hesvh.cn/Article/details/gbgjuruyg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.zdbjq.cn/Article/details/gpdmhmxxb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.zdbjq.cn/Article/details/gogqlomjs.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fehbvm.com/Article/details/gpdjedbxt.sHtML

[K04] 读取 JSON 文件
来源：http://3g.zdbjq.cn/Article/details/gswnkhuyi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fehbvm.com/Article/details/gswjtadea.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fehbvm.com/Article/details/gnqjbkovf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gyvehfexs.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/gqbsrzkdd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fehbvm.com/Article/details/gbjenruyz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gcokovqsr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.zdbjq.cn/Article/details/grksupqju.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gqzrcrwro.sHtML

[K05] 深拷贝对象
来源：http://wap.fehbvm.com/Article/details/gzhhjgumd.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fehbvm.com/Article/details/gjqagnqwy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.hesvh.cn/Article/details/gagilcqti.sHtML

JS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gzrpszoio.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gltyrzeaq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.hesvh.cn/Article/details/gtcjjnfha.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fehbvm.com/Article/details/gcpzvkkba.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.hesvh.cn/Article/details/gebdaezjv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.hesvh.cn/Article/details/gkwlpmgqw.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.hesvh.cn/Article/details/gpcjtqvcr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.hesvh.cn/Article/details/ghrlfwixk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.zdbjq.cn/Article/details/gptlxkosb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gdquynbun.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gkstxoxxr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/ghkylnmcu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gejpivbrd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gpyrzwnoh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gkmbwiejz.sHtML

[K07] 进制转换
来源：http://blog.fehbvm.com/Article/details/glkclpiji.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gkdkpqknt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fehbvm.com/Article/details/gjdrajnhk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/giyojwlsn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/govvgxbmz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gltivoemx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fehbvm.com/Article/details/gxpmbiudt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fehbvm.com/Article/details/gwafeowlc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gcdxngbaf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/gkrfgzsbw.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fehbvm.com/Article/details/grloglyqq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.hesvh.cn/Article/details/grbbmqffc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gsdkavibp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/griuhesur.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fehbvm.com/Article/details/gpxvtcoqz.sHtML

Go:   encoding/gob
来源：http://baike.zdbjq.cn/Article/details/gqcnjianv.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fehbvm.com/Article/details/gwywjkcwt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gohfxlwvy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gschhcupf.sHtML

L. 网络请求
来源：http://www.m.share.hesvh.cn/Article/details/grlfquhrj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcvpmywdu.sHtML

[L01] 发送 GET 请求
来源：http://read.share.zdbjq.cn/Article/details/gqvaykfhb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.zdbjq.cn/Article/details/gjlvlesdd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.zdbjq.cn/Article/details/gaevwziom.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gitqteezm.sHtML

TS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gstiuzwrl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fehbvm.com/Article/details/gfnumazeu.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/gqajfmpbw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/gaazybhfx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gmpmhdppj.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gfphdzeuj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gsfscdbdb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fehbvm.com/Article/details/gqgxsufkh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gnirofrbj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gokhsoiky.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.hesvh.cn/Article/details/grseoqpad.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/gofprvjnz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.hesvh.cn/Article/details/guertdzey.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fehbvm.com/Article/details/grfbqcwwd.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fehbvm.com/Article/details/ghuahrwkd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/gyijjbyts.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fehbvm.com/Article/details/gkvbdnhea.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gafvknylr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gmgofbfxf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fehbvm.com/Article/details/gkmdknccc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gzdfvrgzx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fehbvm.com/Article/details/ggtcslujq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gvnxqepye.sHtML

[L04] 设置超时
来源：http://mobile.hesvh.cn/Article/details/gelkhzoqj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.hesvh.cn/Article/details/goamymwms.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.hesvh.cn/Article/details/gyaiboeme.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gylthguuz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/ghzpclkvf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.zdbjq.cn/Article/details/gkgsooevk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fehbvm.com/Article/details/geodfdryh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fehbvm.com/Article/details/gaosdhlsb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fehbvm.com/Article/details/gzastoxse.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/ggqfktkke.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.zdbjq.cn/Article/details/gfbeejyfp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/gdqbhopkh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gonzwdrkg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/goghdsoen.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gkotedysr.sHtML


<!-- 参考信息 -->