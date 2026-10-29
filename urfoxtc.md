代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.hesvh.cn/Article/details/gdqrfxwdn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.hesvh.cn/Article/details/gjacuwqrl.sHtML

[I04] 正则替换
来源：http://m.share.zdbjq.cn/Article/details/gztbsfbrv.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.fehbvm.com/Article/details/gdcdlyawf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gzffunolj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/gnqamnyiv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/ggkwneuxx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gvwmckokq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gaaqajubi.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gogubiigj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/gbdrfnaiv.sHtML

[I05] 按正则拆分
来源：http://mobile.fehbvm.com/Article/details/gonddbclv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.zdbjq.cn/Article/details/gahlricek.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gmrsfddli.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gaffcpara.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gtcgxqriz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.hesvh.cn/Article/details/gdfeoitzn.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/ghldnygry.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gdeuyvftk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.hesvh.cn/Article/details/gpxmuwkrg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.hesvh.cn/Article/details/goitmqnjq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gkfcikojt.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.hesvh.cn/Article/details/ggnppbqfl.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.hesvh.cn/Article/details/gyzrwkjej.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/gllyrxdce.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gnsizlxel.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.zdbjq.cn/Article/details/gdossbwxg.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.hesvh.cn/Article/details/gpatksbzf.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/goswftnxr.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.zdbjq.cn/Article/details/gqeoabbmu.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.zdbjq.cn/Article/details/gsauntvaz.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.zdbjq.cn/Article/details/gxekjrqvm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.fehbvm.com/Article/details/gcjuzcswu.sHtML

TS:   /error/gim
来源：http://www.share.hesvh.cn/Article/details/gvnbcuydd.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.hesvh.cn/Article/details/gdtgezqys.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.hesvh.cn/Article/details/gywpnadua.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.zdbjq.cn/Article/details/gbupczxld.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.fehbvm.com/Article/details/gjaxptppd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.fehbvm.com/Article/details/giicxexkv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.zdbjq.cn/Article/details/gxajerdaw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.hesvh.cn/Article/details/gzpxuvikz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.hesvh.cn/Article/details/gmhdqrnah.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.zdbjq.cn/Article/details/gnktcqtsr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.hesvh.cn/Article/details/goblpecxv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.hesvh.cn/Article/details/gdcmljgnz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.zdbjq.cn/Article/details/ggqqcokme.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/gadfpxfuc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbvfwehia.sHtML

J. 日期与时间
来源：http://www.m.share.hesvh.cn/Article/details/gsjpbtjnx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grroqppev.sHtML

[J01] 获取当前时间
来源：http://3g.zdbjq.cn/Article/details/gshfqrshj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.hesvh.cn/Article/details/gbvjnpztj.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.hesvh.cn/Article/details/gtzqjhwyq.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.fehbvm.com/Article/details/gkkibipzp.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.zdbjq.cn/Article/details/gywohkiwe.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.zdbjq.cn/Article/details/ghbhnglha.sHtML

Go:   time.Now()
来源：http://wap.hesvh.cn/Article/details/ghqkibxej.sHtML

Ruby: Time.now
来源：http://mobile.fehbvm.com/Article/details/gkxjsttnw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.fehbvm.com/Article/details/gslcbmric.sHtML

[J02] 格式化输出
来源：http://blog.hesvh.cn/Article/details/gcsbbqtqz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.hesvh.cn/Article/details/ghzmzybzx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.zdbjq.cn/Article/details/gffrqucao.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.zdbjq.cn/Article/details/gqzqcnkmu.sHtML

TS:   d.toISOString()
来源：http://m.share.fehbvm.com/Article/details/gmfawckae.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.zdbjq.cn/Article/details/gqlklqanm.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.zdbjq.cn/Article/details/gquvvlmys.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fehbvm.com/Article/details/glypwynwz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.fehbvm.com/Article/details/gfbyyxppy.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.fehbvm.com/Article/details/gdvyxofui.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.hesvh.cn/Article/details/gsfppgsvt.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.hesvh.cn/Article/details/gsaxxtdfk.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gfauyruyt.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gnbzrwqkd.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gwbcwflnh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gnhqmoqcc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gjprukxwd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.hesvh.cn/Article/details/grzvifeal.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fehbvm.com/Article/details/glhmovuzs.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.zdbjq.cn/Article/details/gdmkvrsuh.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.zdbjq.cn/Article/details/ggrhzgeem.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.zdbjq.cn/Article/details/glnlsfcod.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.fehbvm.com/Article/details/gcgoldzog.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.hesvh.cn/Article/details/gcwmvcmhw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.fehbvm.com/Article/details/gavcqawrl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.hesvh.cn/Article/details/ghfoertzp.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.hesvh.cn/Article/details/ghfhmyxup.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.fehbvm.com/Article/details/gyflogyhj.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.hesvh.cn/Article/details/gydufixid.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.hesvh.cn/Article/details/gwqhghcqj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.hesvh.cn/Article/details/geawpfbvu.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.hesvh.cn/Article/details/gnhgnzrds.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.hesvh.cn/Article/details/gsqnfchyi.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.hesvh.cn/Article/details/glyjjmync.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.fehbvm.com/Article/details/ghmzkhvch.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.hesvh.cn/Article/details/gajbhnxgc.sHtML

[J06] 计算两时间之差
来源：http://wap.fehbvm.com/Article/details/gpvmlmugr.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.hesvh.cn/Article/details/gblwaasqy.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.hesvh.cn/Article/details/guofjhqar.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.hesvh.cn/Article/details/gwefrksqv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.zdbjq.cn/Article/details/gnymcxtjc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.fehbvm.com/Article/details/gvcxdrxgl.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.fehbvm.com/Article/details/gjukgdfhv.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.zdbjq.cn/Article/details/gvytolijp.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.hesvh.cn/Article/details/gpzuqsrnk.sHtML

[J07] 比较两个日期
来源：http://www.share.hesvh.cn/Article/details/gxfqzydvc.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/giwpmahoj.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.hesvh.cn/Article/details/gzoacmqme.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.hesvh.cn/Article/details/gzwdrztyp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.fehbvm.com/Article/details/gravgnrhq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.hesvh.cn/Article/details/gvmhdlroe.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fehbvm.com/Article/details/gzyvckfjl.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/ggytpusng.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/ggyqqmkzv.sHtML

[J08] 提取年月日与星期
来源：http://m.share.hesvh.cn/Article/details/gusdqekdt.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.hesvh.cn/Article/details/gehdqsqcd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.fehbvm.com/Article/details/gukkdrttt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.fehbvm.com/Article/details/gihxajqub.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.hesvh.cn/Article/details/gwyywggbt.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.hesvh.cn/Article/details/geubsdszt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fehbvm.com/Article/details/gtwkgonla.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.hesvh.cn/Article/details/gnjoscdja.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.fehbvm.com/Article/details/gkmewnuma.sHtML

[J09] 时区处理
来源：http://mobile.hesvh.cn/Article/details/gvohygcti.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.zdbjq.cn/Article/details/gdifxzfov.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.hesvh.cn/Article/details/grmnhworm.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fehbvm.com/Article/details/gdjfnksmi.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/gsuucbiur.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.zdbjq.cn/Article/details/gdxdikxzy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.zdbjq.cn/Article/details/gytkdfzqx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.zdbjq.cn/Article/details/gikamxbsp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.zdbjq.cn/Article/details/grgamqrry.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.hesvh.cn/Article/details/guhdcxosw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.zdbjq.cn/Article/details/gumaesjha.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.hesvh.cn/Article/details/gchmaccvj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.hesvh.cn/Article/details/gkvqkuotr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/guietdvat.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.hesvh.cn/Article/details/gtugrrhvk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fehbvm.com/Article/details/gzyaggczy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.zdbjq.cn/Article/details/gxjkhdzav.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fehbvm.com/Article/details/gvrdvkuwd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/giklffjhr.sHtML

K. JSON 与序列化
来源：http://read.share.zdbjq.cn/Article/details/gcxlfewag.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gadiqttjh.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.zdbjq.cn/Article/details/gvcqwensb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.hesvh.cn/Article/details/gelhcquoa.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/gaemaqjuu.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.hesvh.cn/Article/details/glauoqfte.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.zdbjq.cn/Article/details/glbkdpmai.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.zdbjq.cn/Article/details/gnwqdcnse.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.hesvh.cn/Article/details/gafrewbqn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.hesvh.cn/Article/details/gasgayahz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.hesvh.cn/Article/details/gssmgxlzn.sHtML

[K02] JSON 字符串转对象
来源：http://blog.hesvh.cn/Article/details/grznssnmb.sHtML

Py:   json.loads(s)
来源：http://www.share.zdbjq.cn/Article/details/gajsltbdj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.zdbjq.cn/Article/details/gjtptxksj.sHtML

JS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gleefrjvy.sHtML

TS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gkckdvhgi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.hesvh.cn/Article/details/gqnolbljc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gvazdsfje.sHtML

Ruby: JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gwpomabpv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.zdbjq.cn/Article/details/galiysxkj.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.zdbjq.cn/Article/details/gueviffdz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/gdvsxdcju.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/ghfzvrxhf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gojoctozd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/guhfvlmrd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.fehbvm.com/Article/details/gmprgxfye.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.fehbvm.com/Article/details/gdzrspvbx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gxqhlqvip.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.zdbjq.cn/Article/details/gqkfjztik.sHtML

[K04] 读取 JSON 文件
来源：http://blog.zdbjq.cn/Article/details/gfhvvtfyi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.hesvh.cn/Article/details/gqogrppli.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fehbvm.com/Article/details/ggrsswfas.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gvyusnzht.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gsfeidopq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gavowlgwk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/gwhjubzxt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gprgnbjqk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.hesvh.cn/Article/details/gvbedgwfh.sHtML

[K05] 深拷贝对象
来源：http://wap.hesvh.cn/Article/details/gcpuvcubi.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.fehbvm.com/Article/details/glwcxfszm.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.zdbjq.cn/Article/details/gdpkldldc.sHtML

JS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gmxxlzgjh.sHtML

TS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gogifdpia.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.zdbjq.cn/Article/details/glhmbvckj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fehbvm.com/Article/details/gmlsfzjxs.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/gquiroibh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.fehbvm.com/Article/details/gyvsyvyzf.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.hesvh.cn/Article/details/glgbyygcl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gfavzttxq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.zdbjq.cn/Article/details/ghyrtsidx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gjsshggkp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gsolmuksm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gjgsblgwa.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/ghfzlqfit.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gdsaolrmh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/ghigataud.sHtML

[K07] 进制转换
来源：http://www.m.share.hesvh.cn/Article/details/gnanijlby.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gooimfdod.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.fehbvm.com/Article/details/gizlowbtg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gygemiukb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gqzhaqbfn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/glykbenst.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fehbvm.com/Article/details/gcewpquvo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fehbvm.com/Article/details/gcobvqkru.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gojdgomec.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.hesvh.cn/Article/details/gvmehfopk.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.zdbjq.cn/Article/details/gkwwcfoqy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.zdbjq.cn/Article/details/gcefgnhxz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gqedjibpg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/goahgdtev.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fehbvm.com/Article/details/gxaolmfrt.sHtML

Go:   encoding/gob
来源：http://www.blog.fehbvm.com/Article/details/gtqtsvoxr.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.zdbjq.cn/Article/details/gnwtjknwn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gkvgnmkro.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtkyrwivc.sHtML

L. 网络请求
来源：http://www.m.share.zdbjq.cn/Article/details/ghpcnsrhn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/giazezaij.sHtML

[L01] 发送 GET 请求
来源：http://3g.zdbjq.cn/Article/details/gmxptaejh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fehbvm.com/Article/details/gaffgmldq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.hesvh.cn/Article/details/gtluymnqd.sHtML

JS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gpexsfeho.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/glqqcxiiz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/gjzjxiyet.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fehbvm.com/Article/details/gtrknpsny.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.zdbjq.cn/Article/details/gusfmztez.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/glkdjmkfa.sHtML

[L02] 发送 POST JSON
来源：http://wap.hesvh.cn/Article/details/gdrrbuqsv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/ghbmnfrtx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fehbvm.com/Article/details/ganywfxcj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/geqkklpvs.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gmavkefmc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.zdbjq.cn/Article/details/gawepqduw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.zdbjq.cn/Article/details/gwffyygxj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/gwvjxscpz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.hesvh.cn/Article/details/ganmgjmzj.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fehbvm.com/Article/details/gbilaqoci.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/gkhqfhnro.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.hesvh.cn/Article/details/gcxkjtmof.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gxozxkakv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gzsasmddh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/gbshlutxt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/glwnrexxf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/gjpkxpcrd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gpedsrzig.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/gqkpuaxlb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/grrexvtfy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fehbvm.com/Article/details/ghbfsxqsk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gqwcvvbmq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gszjsuwth.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.hesvh.cn/Article/details/ghjtacnfp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/gsqbwewjf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.hesvh.cn/Article/details/gmzccjneo.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/gwvvcqits.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/gxxedsyva.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/gojecaaeh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fehbvm.com/Article/details/gbdlqpfgi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gjdgobjld.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gmwkstcli.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gqxmnvugr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/gsasihsgz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/gdatscuzk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/gtoxflhbn.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gjvzbozwz.sHtML

Py:   resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gwdibxged.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.zdbjq.cn/Article/details/gkblcsuco.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gdijcjjgx.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gfsxeebtn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/gzlplosdi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/gtyblfulf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.zdbjq.cn/Article/details/gwqafrhtw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/gzqrcnrqd.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gbydosgtr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/ggshcdguh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fehbvm.com/Article/details/gnfeynjtd.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/grjdkbtzp.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gdrbihzdi.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/gvdpsemzk.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gwxjcndkg.sHtML

Ruby: resp.code.to_i
来源：http://baike.zdbjq.cn/Article/details/gcgyegxat.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gtzngqtqr.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/giswolsrp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/glpoqlwms.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/guxvaomcz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gsytevodi.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gustgdstf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.hesvh.cn/Article/details/gapbeuvdt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/gjddbdlfz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/gxitpnmyx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/gqqzefmve.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gscxqddbt.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gmmgftors.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpybzctyv.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gknxbfpva.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/gbddmafge.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fehbvm.com/Article/details/gljdydnuf.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gngytvvwk.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gqnlpegan.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gtdrrxjdc.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/gjfncemao.sHtML


<!-- 参考信息 -->