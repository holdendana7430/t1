代发 wailian999

TS:   s.match(/\d+/g)
来源：http://www.blog.hesvh.cn/Article/details/gntvftvpc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.hesvh.cn/Article/details/gzmqgjtpl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/gemaetrlf.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/gnadgktiv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.hesvh.cn/Article/details/glnbjvurk.sHtML

[I03] 提取捕获分组
来源：http://m.share.hesvh.cn/Article/details/gggfzelpi.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fehbvm.com/Article/details/gmoznddfk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.zdbjq.cn/Article/details/gntfcpjuk.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.zdbjq.cn/Article/details/gozytrxsx.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.zdbjq.cn/Article/details/gnuqztxvb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.hesvh.cn/Article/details/gxlbkvsyl.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.zdbjq.cn/Article/details/gztotppwg.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.hesvh.cn/Article/details/gwyqracto.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fehbvm.com/Article/details/gsmilkvqv.sHtML

[I04] 正则替换
来源：http://wap.fehbvm.com/Article/details/gfnanmplf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.hesvh.cn/Article/details/gtqqcldwu.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/grmotlhpc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/ghpgpozrr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/gtoexzngd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/gixcfdpjs.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.hesvh.cn/Article/details/gnftoatbh.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.fehbvm.com/Article/details/gztgzrgwh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.fehbvm.com/Article/details/gwkqhhoka.sHtML

[I05] 按正则拆分
来源：http://www.blog.fehbvm.com/Article/details/ggrashjqk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.zdbjq.cn/Article/details/goeixmkcg.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.hesvh.cn/Article/details/gtbseevip.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/grntanygp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gacdccigi.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.hesvh.cn/Article/details/gsuzxzimt.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.hesvh.cn/Article/details/golehlwwn.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gllcpvcaz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.zdbjq.cn/Article/details/gzqswfuvm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fehbvm.com/Article/details/gbqbdhvsp.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gdddartul.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.zdbjq.cn/Article/details/gigpcjkkw.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gwpugtiie.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.hesvh.cn/Article/details/grubcymjv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gsioxahvh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.zdbjq.cn/Article/details/gewdateca.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.zdbjq.cn/Article/details/guoygtszc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gpxylcfsq.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.zdbjq.cn/Article/details/gajbiiwhf.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.hesvh.cn/Article/details/gjcevmrxf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fehbvm.com/Article/details/gwibbhhro.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.fehbvm.com/Article/details/gcaajzctq.sHtML

TS:   /error/gim
来源：http://mobile.fehbvm.com/Article/details/genoheema.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.hesvh.cn/Article/details/gffpxnpba.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.fehbvm.com/Article/details/gvfyyawbi.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.zdbjq.cn/Article/details/grxtqixhl.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.hesvh.cn/Article/details/gwxkswdda.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.hesvh.cn/Article/details/gipekylqe.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.zdbjq.cn/Article/details/gskbbbkkn.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.hesvh.cn/Article/details/guvjlztwe.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.zdbjq.cn/Article/details/gphuwimlg.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.hesvh.cn/Article/details/gcoklxmzj.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.hesvh.cn/Article/details/gudhpalzi.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fehbvm.com/Article/details/gjptbohyp.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.fehbvm.com/Article/details/gkppcakbs.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/ghsqdtmsj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxtdkksog.sHtML

J. 日期与时间
来源：http://www.share.zdbjq.cn/Article/details/gqsdqyfal.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/giyrsiihq.sHtML

[J01] 获取当前时间
来源：http://www.blog.fehbvm.com/Article/details/guhjamopz.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.fehbvm.com/Article/details/gzfaanmid.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.zdbjq.cn/Article/details/gtqzmshfm.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.fehbvm.com/Article/details/gpcqffjkr.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fehbvm.com/Article/details/gcdnenwch.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.zdbjq.cn/Article/details/gpxxmxseo.sHtML

Go:   time.Now()
来源：http://www.m.share.hesvh.cn/Article/details/goznesefl.sHtML

Ruby: Time.now
来源：http://baike.fehbvm.com/Article/details/gilvybcza.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.fehbvm.com/Article/details/gddounmee.sHtML

[J02] 格式化输出
来源：http://www.share.fehbvm.com/Article/details/gmltngjcw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fehbvm.com/Article/details/gbkwcibvv.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.zdbjq.cn/Article/details/gcrtejkko.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.hesvh.cn/Article/details/gloalppkj.sHtML

TS:   d.toISOString()
来源：http://wap.zdbjq.cn/Article/details/genmjlosh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.fehbvm.com/Article/details/ggvdkeghj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.hesvh.cn/Article/details/ghuoverez.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.hesvh.cn/Article/details/giclvuamx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.hesvh.cn/Article/details/gbvcwcjdx.sHtML

[J03] 字符串解析为日期
来源：http://www.share.zdbjq.cn/Article/details/gglopuoff.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fehbvm.com/Article/details/gkpnxjbqu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.fehbvm.com/Article/details/gjqeojdol.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gqrelulbb.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/guyowiaya.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/genwtjfsx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gihdeumgl.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/ggbiwfzkg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.zdbjq.cn/Article/details/gnslfemgl.sHtML

[J04] 时间戳与日期互转
来源：http://3g.hesvh.cn/Article/details/gtshausnj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.hesvh.cn/Article/details/gonqknkzm.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.zdbjq.cn/Article/details/gppgphmxi.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.zdbjq.cn/Article/details/gsltlpshn.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.fehbvm.com/Article/details/gcwqcdmsv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.zdbjq.cn/Article/details/gbjhahfav.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.hesvh.cn/Article/details/gvcevymgl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.hesvh.cn/Article/details/gmjhvgewz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.fehbvm.com/Article/details/gdykpowug.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.hesvh.cn/Article/details/gomnarper.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.fehbvm.com/Article/details/gmqevsagj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.hesvh.cn/Article/details/gkoquwlmh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.zdbjq.cn/Article/details/gszimogwh.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/gdlhwtqxi.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.zdbjq.cn/Article/details/gmgwdemth.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.zdbjq.cn/Article/details/gmcuikkpj.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.zdbjq.cn/Article/details/gdbamltoi.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.zdbjq.cn/Article/details/gcsaksafd.sHtML

[J06] 计算两时间之差
来源：http://3g.hesvh.cn/Article/details/gvmceudpm.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.zdbjq.cn/Article/details/gkgrocaxc.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.fehbvm.com/Article/details/gskwefazv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.hesvh.cn/Article/details/gjnahjdiz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.hesvh.cn/Article/details/gibqilvyl.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.zdbjq.cn/Article/details/gratizgrr.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.hesvh.cn/Article/details/gayvfseyo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.hesvh.cn/Article/details/gwqxyqwwz.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.zdbjq.cn/Article/details/gbpedfcff.sHtML

[J07] 比较两个日期
来源：http://wap.hesvh.cn/Article/details/glyrdysjd.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gmiipjwuf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.hesvh.cn/Article/details/gaotpiyfb.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/gyagofjxl.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fehbvm.com/Article/details/gnoszvslq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghmdevwxw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.hesvh.cn/Article/details/gzpmxdtsy.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/glgcfrxdz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gctaaabff.sHtML

[J08] 提取年月日与星期
来源：http://read.share.hesvh.cn/Article/details/guqnwrfcc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.hesvh.cn/Article/details/gfjlmemsb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.hesvh.cn/Article/details/gvhbvjkze.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.zdbjq.cn/Article/details/gryljvymz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.fehbvm.com/Article/details/gnmesuhar.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fehbvm.com/Article/details/gjmunguvx.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.zdbjq.cn/Article/details/gcwqgecxd.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.fehbvm.com/Article/details/gptcrjyhx.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.hesvh.cn/Article/details/gxzyveskw.sHtML

[J09] 时区处理
来源：http://blog.hesvh.cn/Article/details/goatjlutf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.zdbjq.cn/Article/details/gifsvnbbz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.zdbjq.cn/Article/details/ggowipane.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/gjexhqung.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/gkuzqehll.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.zdbjq.cn/Article/details/grrerncph.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.zdbjq.cn/Article/details/gfwxyjrol.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.hesvh.cn/Article/details/gbslqrurt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.hesvh.cn/Article/details/gqcocghun.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.zdbjq.cn/Article/details/gwdrcvdbv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.hesvh.cn/Article/details/gqdxchqyd.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.hesvh.cn/Article/details/ggsbeyncd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.fehbvm.com/Article/details/gvqahzndh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.fehbvm.com/Article/details/gktgqqfpp.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.zdbjq.cn/Article/details/glxznhemb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.zdbjq.cn/Article/details/gkyeqacir.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.fehbvm.com/Article/details/glnwfyyoj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.hesvh.cn/Article/details/gcbapsold.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfcfgmtkr.sHtML

K. JSON 与序列化
来源：http://baike.fehbvm.com/Article/details/gmcujcreh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbookaeon.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.zdbjq.cn/Article/details/gkdyjnhum.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/gdowkdjzd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gxyvfoqkm.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gvfbkbxzn.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gppmvptuv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.hesvh.cn/Article/details/grzpbkzif.sHtML

Go:   json.Marshal(obj)
来源：http://wap.fehbvm.com/Article/details/gchqcnxfl.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.fehbvm.com/Article/details/gwrqhsoet.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.fehbvm.com/Article/details/gzcbuyqus.sHtML

[K02] JSON 字符串转对象
来源：http://baike.hesvh.cn/Article/details/gimhchoel.sHtML

Py:   json.loads(s)
来源：http://baike.zdbjq.cn/Article/details/gpkaxeciw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fehbvm.com/Article/details/gofmfbrcs.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gcrcdmnpz.sHtML

TS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gfqerwjtr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.hesvh.cn/Article/details/gabgwessb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gmskiumjt.sHtML

Ruby: JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gvibcyxjv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.hesvh.cn/Article/details/gbfjljffq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.zdbjq.cn/Article/details/geqdqjvdg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.fehbvm.com/Article/details/giccvtluj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/gqonxeqvn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/guhrgzhgp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gktrgfpxa.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.hesvh.cn/Article/details/gcleobrgx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.zdbjq.cn/Article/details/gwsmmbsfp.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.zdbjq.cn/Article/details/gndwsnhyl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fehbvm.com/Article/details/grusuzrot.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fehbvm.com/Article/details/gzzsxtsxb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.hesvh.cn/Article/details/gjkiyrwoa.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.fehbvm.com/Article/details/gbjejbvoy.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/gapqczsgh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/gvdpqbndu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gqxkubfhr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.hesvh.cn/Article/details/gqikkqpsy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gzbulbutz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.zdbjq.cn/Article/details/gzhcceyzt.sHtML

[K05] 深拷贝对象
来源：http://baike.zdbjq.cn/Article/details/gppefkdcu.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.zdbjq.cn/Article/details/gimuznhmf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fehbvm.com/Article/details/gklbveief.sHtML

JS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gbgrlfngl.sHtML

TS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gztcrdzqw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.hesvh.cn/Article/details/glyxbtwst.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fehbvm.com/Article/details/gyjdgiwji.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fehbvm.com/Article/details/guvlhbzjd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.hesvh.cn/Article/details/gkefagiof.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.zdbjq.cn/Article/details/gdbejmfjg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gbxqcwymu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.zdbjq.cn/Article/details/gstrnlekz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gvuruqxft.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gfxwbetap.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.hesvh.cn/Article/details/ggdpsaotl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/ghewyrule.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gudmuhuea.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/grjkdwtfa.sHtML

[K07] 进制转换
来源：http://3g.hesvh.cn/Article/details/gbllpvupq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gfybvbtiu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/gjqidgfhc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gkifipdhm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gmdxajfzl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gnbuigfge.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/gpfxlcvei.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.zdbjq.cn/Article/details/gjwzrsjjk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gjpqipmvv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.hesvh.cn/Article/details/gsravmivz.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.fehbvm.com/Article/details/gbhrtujow.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.hesvh.cn/Article/details/goflzwtxk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/ghwjmdgrd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gtjarhynk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.zdbjq.cn/Article/details/gkcfasuqv.sHtML

Go:   encoding/gob
来源：http://www.blog.zdbjq.cn/Article/details/gzzypvpqv.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.zdbjq.cn/Article/details/ggrysnrqp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gbdwvshqp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtyfyjpit.sHtML

L. 网络请求
来源：http://wap.zdbjq.cn/Article/details/gkqbnmtbo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmjtmxmhu.sHtML

[L01] 发送 GET 请求
来源：http://baike.zdbjq.cn/Article/details/gbttbxqvy.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/gtfrzdivp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/gitphgocz.sHtML

JS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/grkdzyxwf.sHtML

TS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gbqnyrkrh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fehbvm.com/Article/details/gfthgzxyz.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.zdbjq.cn/Article/details/gwuogezin.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fehbvm.com/Article/details/gbzadhxeg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/gxuqbrluf.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gtsemvszd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.zdbjq.cn/Article/details/grbmmpdzp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/gkirzcaxs.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/guacgyzju.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gieywcnue.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fehbvm.com/Article/details/gtwpqdcwu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/gwtjpucol.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.hesvh.cn/Article/details/gahrazwmp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.hesvh.cn/Article/details/gayhqylev.sHtML

[L03] 设置自定义请求头
来源：http://m.share.hesvh.cn/Article/details/gosmydtdg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/ggubjbhnc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fehbvm.com/Article/details/gkobiyxnw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gwcodgifp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gisyntxtx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.zdbjq.cn/Article/details/gssolivss.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gekoaztof.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fehbvm.com/Article/details/gkhroieza.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gahfsallo.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/gwmpnurea.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fehbvm.com/Article/details/grzwnqttv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/gjgaqnpbe.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gmckemsrr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gktqnhzxh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/ggjtvhkfw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.zdbjq.cn/Article/details/gwqlqnrqg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.hesvh.cn/Article/details/gsqngwtyp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/giegomsxs.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/gigblvmtv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fehbvm.com/Article/details/gpuazjpik.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.hesvh.cn/Article/details/gxsthtzty.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/ggkbfperl.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gcxekbvqs.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/grectxqob.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gwnsjphvl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/gvamwhaqq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fehbvm.com/Article/details/gilvngkll.sHtML

[L06] 解析响应为 JSON
来源：http://baike.zdbjq.cn/Article/details/gtggxczgu.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/gyninvcwo.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/glfriflca.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gctycauyp.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gutttpeha.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gcveoozpy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/giedwqkhc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gommatwve.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.hesvh.cn/Article/details/gedoxbwcs.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gbenislfp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.hesvh.cn/Article/details/gryqwopbj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.hesvh.cn/Article/details/gelqehkak.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gbocwzqor.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gflyrwezt.sHtML

Java: resp.statusCode()
来源：http://read.share.fehbvm.com/Article/details/ghsloqtab.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/ggrvgyzfn.sHtML

Ruby: resp.code.to_i
来源：http://baike.zdbjq.cn/Article/details/gxnfboklm.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gdummrvma.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/gcemvkjdx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gtklwtdwx.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/gxrtkehrs.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gvpoxxuuc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gunoesiay.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.hesvh.cn/Article/details/gttsoaqfx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/gozojdnvh.sHtML


<!-- 参考信息 -->