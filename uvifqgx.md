代发 wailian999

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcthxlwdt.sHtML

I. 正则表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/glvcvtokw.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvefezedn.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyenhzle.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdtiqhfz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gbpdbnmrj.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gmtverasn.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbiiusaok.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuohwdlr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gppayuufc.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fanxiaobao.xyz/Article/details/grocovfmg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gtvgyjcfq.sHtML

[I02] 提取所有匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsshhbvf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fanxiaobao.xyz/Article/details/grbimqkrd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwwtlcbr.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.fanxiaobao.xyz/Article/details/gzvoyulvq.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fanxiaobao.xyz/Article/details/guiagmxkr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gblogvgnm.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gymmbbcoe.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fanxiaobao.xyz/Article/details/gckzdysmv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidoblcyw.sHtML

[I03] 提取捕获分组
来源：http://3g.fanxiaobao.xyz/Article/details/gjymvyeqw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsosqjgzm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.fanxiaobao.xyz/Article/details/gpocykspt.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.fanxiaobao.xyz/Article/details/gyrtmfcbk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcsnlebn.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmccunaij.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnlctqut.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fanxiaobao.xyz/Article/details/gvkupndad.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitlrrunp.sHtML

[I04] 正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gupwyqlhf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gilzeoxse.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtppqumld.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvavlmsi.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqipvajho.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fanxiaobao.xyz/Article/details/gtpchlpcb.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/gircnqxkp.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fanxiaobao.xyz/Article/details/gaazeesfx.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.fanxiaobao.xyz/Article/details/gdfjbritm.sHtML

[I05] 按正则拆分
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghraahhof.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwxasail.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpvngxms.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fanxiaobao.xyz/Article/details/gohtxhgvk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fanxiaobao.xyz/Article/details/gnnqizewr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnthgczbe.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fanxiaobao.xyz/Article/details/grfatfzuy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fanxiaobao.xyz/Article/details/gidouvrnc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnnrjjtb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbubkraxj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjaucycsz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.fanxiaobao.xyz/Article/details/gslaihtfx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzucfcsh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfhgtalo.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.fanxiaobao.xyz/Article/details/gybkkleml.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.fanxiaobao.xyz/Article/details/grksyupzw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fanxiaobao.xyz/Article/details/guitbuhcp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.fanxiaobao.xyz/Article/details/glnnpowlc.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlrlptvy.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.fanxiaobao.xyz/Article/details/gzggihgzr.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.fanxiaobao.xyz/Article/details/gliqeeooe.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcytdgykw.sHtML

TS:   /error/gim
来源：http://baike.fanxiaobao.xyz/Article/details/guddtxybi.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.fanxiaobao.xyz/Article/details/gfcqeyikf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.fanxiaobao.xyz/Article/details/goxrgorho.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqmeudou.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.fanxiaobao.xyz/Article/details/gfrxnxtze.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhiiddhq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvaxqdpw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.fanxiaobao.xyz/Article/details/gipuvekcc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fanxiaobao.xyz/Article/details/gijvteabw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwbguird.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.fanxiaobao.xyz/Article/details/gdrjxgzou.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkxfeixn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhxarzle.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkolysbkx.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnvgvxhj.sHtML

J. 日期与时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gvaspbqfe.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gloajtqgk.sHtML

[J01] 获取当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gpaagxspw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbetheyi.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.fanxiaobao.xyz/Article/details/gttesuicc.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.fanxiaobao.xyz/Article/details/guxcnrchc.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyxrqyqt.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fanxiaobao.xyz/Article/details/gstqkuzfz.sHtML

Go:   time.Now()
来源：http://mobile.fanxiaobao.xyz/Article/details/gxilscvjy.sHtML

Ruby: Time.now
来源：http://wap.fanxiaobao.xyz/Article/details/gfsevmxei.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.fanxiaobao.xyz/Article/details/ghktvcqhx.sHtML

[J02] 格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgqgwnvk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhnqcyqx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.fanxiaobao.xyz/Article/details/gppplrpbc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fanxiaobao.xyz/Article/details/gbqcnkuhp.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwlpbbnp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fanxiaobao.xyz/Article/details/gahkinies.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtjtgxxb.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fanxiaobao.xyz/Article/details/gmxjblwxk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glibaoftn.sHtML

[J03] 字符串解析为日期
来源：http://mobile.fanxiaobao.xyz/Article/details/gfohgpdfb.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.fanxiaobao.xyz/Article/details/givtllemi.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.fanxiaobao.xyz/Article/details/gierzbiru.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfcvrekc.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepbqifvk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.fanxiaobao.xyz/Article/details/glitxevkp.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonkipzbo.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.fanxiaobao.xyz/Article/details/gykfigfuf.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsuldiez.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gokokvcnm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.fanxiaobao.xyz/Article/details/glsmmbcoz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwlhqxvn.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewkojlwk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.fanxiaobao.xyz/Article/details/gbcqlliir.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnywporch.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gviliksdi.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcnjjmka.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.fanxiaobao.xyz/Article/details/gizgbazwh.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.fanxiaobao.xyz/Article/details/gepledqmh.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnmkzvwz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.fanxiaobao.xyz/Article/details/gymdumjnh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvditrzmg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyddttcu.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fanxiaobao.xyz/Article/details/gwfrhudcn.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhmquzig.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqdingsv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcyswtjq.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzudwnvb.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.fanxiaobao.xyz/Article/details/ghdspgbns.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuuspdvc.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.fanxiaobao.xyz/Article/details/giaceyjkw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnjanjso.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmtzypfv.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.fanxiaobao.xyz/Article/details/gljpmcryt.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvqeizof.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.fanxiaobao.xyz/Article/details/gjtcqufgs.sHtML

[J07] 比较两个日期
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgnzocff.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbqahyck.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gclpegnid.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrxapjxx.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.fanxiaobao.xyz/Article/details/gajdukhig.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcozcyyy.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwybjborc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsuxzcje.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.fanxiaobao.xyz/Article/details/gljsxlxzg.sHtML

[J08] 提取年月日与星期
来源：http://baike.fanxiaobao.xyz/Article/details/gkhcltufo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdraburlx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.fanxiaobao.xyz/Article/details/glgeebugl.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzrpiydk.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.fanxiaobao.xyz/Article/details/gmqelxeqn.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.fanxiaobao.xyz/Article/details/geqxaeszj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fanxiaobao.xyz/Article/details/gcqtpppkl.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgtokytc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwzdzpxh.sHtML

[J09] 时区处理
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyspunvu.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.fanxiaobao.xyz/Article/details/gbxinrcxz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqimazty.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgkmdccs.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeeobgno.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.fanxiaobao.xyz/Article/details/gqbyfwxdt.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehldwjsc.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxmhefaj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljgtiozr.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.fanxiaobao.xyz/Article/details/gmijrewrp.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmpimgwz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvxpighw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdzuhuhp.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwszkbtju.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gnrpmedwx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsdoenrm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.fanxiaobao.xyz/Article/details/gqbvyfyhd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gtycpomyu.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbolkkbe.sHtML

K. JSON 与序列化
来源：http://baike.fanxiaobao.xyz/Article/details/gntxvugkg.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/giejezefo.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gncptvixk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fanxiaobao.xyz/Article/details/gaysugowr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnsbhfka.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gujtuybtk.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gfbwppyxu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fanxiaobao.xyz/Article/details/gipnzscha.sHtML

Go:   json.Marshal(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gidxiawlc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fanxiaobao.xyz/Article/details/gbbcqiiym.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymmtdvly.sHtML

[K02] JSON 字符串转对象
来源：http://blog.fanxiaobao.xyz/Article/details/gwfoycuhx.sHtML

Py:   json.loads(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuhsfosf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfwxraek.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqlhanxt.sHtML

TS:   JSON.parse(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gljkqubnm.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fanxiaobao.xyz/Article/details/gpmciroym.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fanxiaobao.xyz/Article/details/gvgopzkjv.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwgdqmjy.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gzjgmhbjy.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghckbpeme.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.fanxiaobao.xyz/Article/details/gctkirien.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fanxiaobao.xyz/Article/details/gnpcmyvvn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwgennag.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmthzrwyo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gkkipnkna.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fanxiaobao.xyz/Article/details/gddnqnvwu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/golbtbqyh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fanxiaobao.xyz/Article/details/ghevnzvwd.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjmyxdwi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fanxiaobao.xyz/Article/details/gqpjiaggr.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrfmtqkq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gnowjubtk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gshlqndwb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmjnavsf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fanxiaobao.xyz/Article/details/gxisstork.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fanxiaobao.xyz/Article/details/ghfkaiqhb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyvpmfjj.sHtML

[K05] 深拷贝对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gmusjhgwr.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvpyswvi.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtfqmlsu.sHtML

JS:   structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyabmyfd.sHtML

TS:   structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpxjgiis.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.fanxiaobao.xyz/Article/details/gsnpcuqkt.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.fanxiaobao.xyz/Article/details/geoocnmls.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyhwihhd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fanxiaobao.xyz/Article/details/gcqrxwauo.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fanxiaobao.xyz/Article/details/gesjlrncb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fanxiaobao.xyz/Article/details/grznecbwo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnafcewf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fanxiaobao.xyz/Article/details/gcfpgaacz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsuhzvgg.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fanxiaobao.xyz/Article/details/gztciehfc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzqjbqar.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fanxiaobao.xyz/Article/details/gcxkkemqw.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fanxiaobao.xyz/Article/details/gjehzxoqm.sHtML

[K07] 进制转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrikgllx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyffsqnj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqzrhhfl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.fanxiaobao.xyz/Article/details/ganashgyv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gxworqxat.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/grzbzaqul.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fanxiaobao.xyz/Article/details/ggxxiltad.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvgtqseo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjskiumz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmkhmlxm.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gwgtasxts.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gkrsfjtdu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fanxiaobao.xyz/Article/details/gensjfwbp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgywhwon.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fanxiaobao.xyz/Article/details/glthyahpb.sHtML

Go:   encoding/gob
来源：http://baike.fanxiaobao.xyz/Article/details/gllagvmte.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxsnemcj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fanxiaobao.xyz/Article/details/gquvicndy.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoxmuvpy.sHtML

L. 网络请求
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdzzaaex.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gnprbhuuj.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gclqoqund.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fanxiaobao.xyz/Article/details/gxfzkeckz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fanxiaobao.xyz/Article/details/grnnmsega.sHtML

JS:   await fetch(url)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpfnjsbb.sHtML

TS:   await fetch(url)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpiejptsb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrkxlajx.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fanxiaobao.xyz/Article/details/grvmjxdxs.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fanxiaobao.xyz/Article/details/ghocquefl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fanxiaobao.xyz/Article/details/gndonoslx.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gichzpnrf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjatbkyyx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fanxiaobao.xyz/Article/details/gogzuoilx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fanxiaobao.xyz/Article/details/grglyhtqu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmunnxps.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fanxiaobao.xyz/Article/details/glwbqovim.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fanxiaobao.xyz/Article/details/gmacnfivo.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fanxiaobao.xyz/Article/details/gduiazfqy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqbkhkov.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawvmqaoj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxlnrekm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchxbimst.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqddpxxy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fanxiaobao.xyz/Article/details/grfioftpv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fanxiaobao.xyz/Article/details/gprwfjxiz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkkqllvy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecxbfxbe.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fanxiaobao.xyz/Article/details/glchliqbs.sHtML

[L04] 设置超时
来源：http://wap.fanxiaobao.xyz/Article/details/ggyfzekha.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fanxiaobao.xyz/Article/details/gakouytnw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fanxiaobao.xyz/Article/details/gtywfyjow.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fanxiaobao.xyz/Article/details/guxvmtgux.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fanxiaobao.xyz/Article/details/gfqgeplmx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fanxiaobao.xyz/Article/details/gaibhcxoo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fanxiaobao.xyz/Article/details/gcbcmdehy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxatejbbc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fanxiaobao.xyz/Article/details/grnmhedpb.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvtjinuk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyfssuru.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexalssln.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjuvqkdl.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fanxiaobao.xyz/Article/details/gbekcizjj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fanxiaobao.xyz/Article/details/gndeejecj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdwvgplhr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fanxiaobao.xyz/Article/details/gqxsqcnir.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gnjgovjlk.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gecwhkqyq.sHtML

Py:   resp.json()
来源：http://blog.fanxiaobao.xyz/Article/details/gmtsmopmp.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gmyzyohpc.sHtML

JS:   await resp.json()
来源：http://blog.fanxiaobao.xyz/Article/details/gyqpedort.sHtML

TS:   await resp.json()
来源：http://baike.fanxiaobao.xyz/Article/details/gsypqqdnj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fanxiaobao.xyz/Article/details/gvemzsffi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtqfariq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfbzkrjr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fanxiaobao.xyz/Article/details/gbapxhcva.sHtML


<!-- 参考信息 -->