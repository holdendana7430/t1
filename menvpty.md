代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.fehbvm.com/Article/details/gmtpdmcdi.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.hesvh.cn/Article/details/grkvzwxnq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.zdbjq.cn/Article/details/grrwfwflm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.zdbjq.cn/Article/details/gxfnpvsnm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.hesvh.cn/Article/details/gvfcikupv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.zdbjq.cn/Article/details/gvphvygud.sHtML

[I04] 正则替换
来源：http://mobile.hesvh.cn/Article/details/gpmzmnpqt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.zdbjq.cn/Article/details/gazzjhtwp.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gjeauccvy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/gitxoaiqc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/gvwktauhe.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gecgbjlkt.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fehbvm.com/Article/details/gxxxxyzeg.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fehbvm.com/Article/details/gwpworpov.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gxxufzwek.sHtML

[I05] 按正则拆分
来源：http://m.share.zdbjq.cn/Article/details/gnctgembn.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.zdbjq.cn/Article/details/gunbunplu.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gevywmsxg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/gzrcemwge.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gvomgjkxv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.zdbjq.cn/Article/details/gxrfshqut.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/ggnstyczd.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/grdchtjar.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.hesvh.cn/Article/details/gkyszsniz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fehbvm.com/Article/details/ghxknudma.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gzfmtmxje.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.zdbjq.cn/Article/details/guaveldfv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fehbvm.com/Article/details/gwphjtakc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fehbvm.com/Article/details/gkgvrnqwz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gdlkgtibw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.zdbjq.cn/Article/details/gexafwmnu.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.zdbjq.cn/Article/details/grftseldh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gudbcvhrs.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.zdbjq.cn/Article/details/gatsdvwda.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fehbvm.com/Article/details/gagkjstqr.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.zdbjq.cn/Article/details/gyojdzbfk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.zdbjq.cn/Article/details/gmmhkyzyx.sHtML

TS:   /error/gim
来源：http://www.share.zdbjq.cn/Article/details/gjkgzhymb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.hesvh.cn/Article/details/ghuiiljij.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.zdbjq.cn/Article/details/gtxiomcgg.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.fehbvm.com/Article/details/gzjkivhvx.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fehbvm.com/Article/details/glsxvcdtc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fehbvm.com/Article/details/gtkbgwlqa.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.hesvh.cn/Article/details/gzgolyiri.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.hesvh.cn/Article/details/gltgmsrvi.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.hesvh.cn/Article/details/grzmqzqtd.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fehbvm.com/Article/details/gwwrnjrob.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.fehbvm.com/Article/details/gjyvlxjzl.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.hesvh.cn/Article/details/ghsamptpt.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.zdbjq.cn/Article/details/gcvtvtpqc.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/groglpyex.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gssicycbf.sHtML

J. 日期与时间
来源：http://mobile.zdbjq.cn/Article/details/gyvphdyzn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gerrcmdzc.sHtML

[J01] 获取当前时间
来源：http://www.share.hesvh.cn/Article/details/garxoekzj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.zdbjq.cn/Article/details/ganspkxoz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/gzgcaucbx.sHtML

JS:   new Date();  Date.now()
来源：http://wap.zdbjq.cn/Article/details/gydotpnay.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gionzekpa.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.hesvh.cn/Article/details/gyqvgxjqo.sHtML

Go:   time.Now()
来源：http://3g.hesvh.cn/Article/details/ggnjvdkka.sHtML

Ruby: Time.now
来源：http://mobile.fehbvm.com/Article/details/gutvblppa.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.zdbjq.cn/Article/details/gobqdfrdt.sHtML

[J02] 格式化输出
来源：http://3g.fehbvm.com/Article/details/gavqcyvby.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/genkpmprp.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.hesvh.cn/Article/details/gkjaprwqe.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.fehbvm.com/Article/details/gecrbockh.sHtML

TS:   d.toISOString()
来源：http://www.m.share.hesvh.cn/Article/details/gkxntazgs.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.fehbvm.com/Article/details/gryqukaym.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.zdbjq.cn/Article/details/ggmrxhhjx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/gtwhkcucx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.zdbjq.cn/Article/details/gpmeloctb.sHtML

[J03] 字符串解析为日期
来源：http://read.share.fehbvm.com/Article/details/gdwapdocj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.hesvh.cn/Article/details/gruqpujgj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.fehbvm.com/Article/details/gpfmrinlt.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gvisphijz.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gfemmioeg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gzdootrdn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gjxiqouph.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gizdqurkd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.zdbjq.cn/Article/details/gmyvcklze.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.zdbjq.cn/Article/details/gkviszjmz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.hesvh.cn/Article/details/gaiaynbzy.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.zdbjq.cn/Article/details/geclgjlia.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.zdbjq.cn/Article/details/ggjfdsvqp.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.hesvh.cn/Article/details/gcwxlxgqf.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.fehbvm.com/Article/details/godpvulqw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.fehbvm.com/Article/details/gysiqedvb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.fehbvm.com/Article/details/gmukucefo.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gwwyhuvnt.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.zdbjq.cn/Article/details/gzmfidmjx.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.fehbvm.com/Article/details/goutgreot.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.hesvh.cn/Article/details/gexrrvstq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.zdbjq.cn/Article/details/galrjehvy.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.hesvh.cn/Article/details/guxrselwz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.hesvh.cn/Article/details/gwatmgtmv.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.hesvh.cn/Article/details/giiornxda.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.hesvh.cn/Article/details/gozyqypvw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.zdbjq.cn/Article/details/gxnnvcudi.sHtML

[J06] 计算两时间之差
来源：http://read.share.fehbvm.com/Article/details/gymmwmlqt.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.zdbjq.cn/Article/details/ghpzjuzmc.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.zdbjq.cn/Article/details/gkebyupkv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.zdbjq.cn/Article/details/gjxalqyyv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.zdbjq.cn/Article/details/gwxbvjgux.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.zdbjq.cn/Article/details/getqshgvf.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.hesvh.cn/Article/details/gewmboami.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.fehbvm.com/Article/details/gbkmktqqs.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.hesvh.cn/Article/details/gmmclxhqo.sHtML

[J07] 比较两个日期
来源：http://read.share.hesvh.cn/Article/details/gccahmxdj.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gokwrtlqt.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.fehbvm.com/Article/details/gsungccee.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.zdbjq.cn/Article/details/gyhzcbbvu.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.fehbvm.com/Article/details/gsvodqkph.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.zdbjq.cn/Article/details/gtwjfdzwq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.hesvh.cn/Article/details/gbzxssgju.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/giqcqorhk.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gzbvjdufu.sHtML

[J08] 提取年月日与星期
来源：http://www.share.zdbjq.cn/Article/details/guhnmpion.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.hesvh.cn/Article/details/gmomnqxum.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.zdbjq.cn/Article/details/gcvactmlg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.fehbvm.com/Article/details/gggmzmens.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.fehbvm.com/Article/details/gdfmyjzec.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fehbvm.com/Article/details/gzpmxecln.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.zdbjq.cn/Article/details/gobfeqkoc.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.zdbjq.cn/Article/details/gsipasact.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.hesvh.cn/Article/details/gakqpwgii.sHtML

[J09] 时区处理
来源：http://www.blog.hesvh.cn/Article/details/gxknluesm.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.zdbjq.cn/Article/details/guwzkabpo.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.zdbjq.cn/Article/details/gyejptdqr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.zdbjq.cn/Article/details/gucyetdbt.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/gatscbvlb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.hesvh.cn/Article/details/gnpffncis.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.zdbjq.cn/Article/details/gbssihgqt.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.zdbjq.cn/Article/details/gtmnrzqmb.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.zdbjq.cn/Article/details/gclydeohj.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.hesvh.cn/Article/details/gniyelvcy.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.hesvh.cn/Article/details/gogywicqu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.zdbjq.cn/Article/details/gatnmyiln.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.hesvh.cn/Article/details/gekudzbxa.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gpyrifpbf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.hesvh.cn/Article/details/gnfdfqnwh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.hesvh.cn/Article/details/gbrytavzc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.hesvh.cn/Article/details/gzsmypxec.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.fehbvm.com/Article/details/govenlxox.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmvqtmezj.sHtML

K. JSON 与序列化
来源：http://wap.zdbjq.cn/Article/details/giqjjqpbs.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gztdxlsxc.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.zdbjq.cn/Article/details/guroozliy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/gwddmxvxb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gzcmdjcam.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.zdbjq.cn/Article/details/gloydqkzu.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/gxlhylpwy.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.hesvh.cn/Article/details/gbbgeoedu.sHtML

Go:   json.Marshal(obj)
来源：http://blog.zdbjq.cn/Article/details/gqunayjkq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.zdbjq.cn/Article/details/golsisccd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fehbvm.com/Article/details/gvdufqdvx.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.zdbjq.cn/Article/details/gnqvjgxay.sHtML

Py:   json.loads(s)
来源：http://baike.zdbjq.cn/Article/details/gzqywfelf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fehbvm.com/Article/details/gaddrhhgs.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gsszyqfnc.sHtML

TS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gutcktkjt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.hesvh.cn/Article/details/ggdyodkxv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/grswhxuus.sHtML

Ruby: JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gvdqfjcvh.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fehbvm.com/Article/details/geagbnjba.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.hesvh.cn/Article/details/gvrxxgoju.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/ghlxggefm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/giqbkshbi.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/gelirenpt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gvkwunbla.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.zdbjq.cn/Article/details/gxxlwgxmn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fehbvm.com/Article/details/gnzuupixr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.hesvh.cn/Article/details/gveiihfap.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.zdbjq.cn/Article/details/gjctgofwg.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fehbvm.com/Article/details/ggjbkfwts.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.zdbjq.cn/Article/details/gotvzoqiw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.hesvh.cn/Article/details/gqocnnbox.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gruiqnbld.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gwjuguciq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gdllyupxo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/gmwofbhcq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/gnmfqksij.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gdghejjsd.sHtML

[K05] 深拷贝对象
来源：http://read.share.zdbjq.cn/Article/details/gtubevvqf.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.hesvh.cn/Article/details/ghrsglddn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fehbvm.com/Article/details/gacmgkngw.sHtML

JS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/ggfhjjvgj.sHtML

TS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gasqznemp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.hesvh.cn/Article/details/gwdkoyxdp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.zdbjq.cn/Article/details/ggsifdxul.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.zdbjq.cn/Article/details/gtmohkytf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.hesvh.cn/Article/details/gexpnrzst.sHtML

[K06] 解析 URL 查询串
来源：http://3g.hesvh.cn/Article/details/gceykhxwl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gvztoaxrd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.hesvh.cn/Article/details/gzrgqomed.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/gmdjrdnkf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/ghxxfyxds.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.zdbjq.cn/Article/details/gebfbhkba.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gqgqweigp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/guuaruvwa.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/ggmlvnckn.sHtML

[K07] 进制转换
来源：http://m.share.fehbvm.com/Article/details/gicsgiwle.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gthfjkctl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.hesvh.cn/Article/details/gbjondars.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/grpfazppj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gykifmick.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gjgpawqdn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fehbvm.com/Article/details/gyxqvokms.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.zdbjq.cn/Article/details/gxbotlxtp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gbsswrlnw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.hesvh.cn/Article/details/gfqvhlcbw.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gmcvlsbtl.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.hesvh.cn/Article/details/gzblkcemt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gttbyzekl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gsrxfywzu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/gvjcswrss.sHtML

Go:   encoding/gob
来源：http://www.share.fehbvm.com/Article/details/ghqmunqgc.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.hesvh.cn/Article/details/gupriwjcx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gkqgaydhq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvneuuwfd.sHtML

L. 网络请求
来源：http://read.share.fehbvm.com/Article/details/gkkdknxlm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghgjmcyxk.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.hesvh.cn/Article/details/geufgijmd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.zdbjq.cn/Article/details/gyhgagvau.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.zdbjq.cn/Article/details/gebvpqpad.sHtML

JS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gxlaiknxk.sHtML

TS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/glvoznuak.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fehbvm.com/Article/details/gczrjiiqz.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.zdbjq.cn/Article/details/gqzocumbg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/gtpvlzifc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.hesvh.cn/Article/details/guqueiuzu.sHtML

[L02] 发送 POST JSON
来源：http://blog.fehbvm.com/Article/details/gosgljrbh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gkbcstyhr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.hesvh.cn/Article/details/ggqbajkto.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gxlscmuyc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gmitqectt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/gcazmjdhd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/gjuftugvj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.zdbjq.cn/Article/details/gfuopqmfi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/gqurwdmyn.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/gcadazcnz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.hesvh.cn/Article/details/gakcfxxlf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/ghqyvgdfa.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gwqdwwzqf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gmxiaqiap.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.zdbjq.cn/Article/details/gkibdqxmu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gkophylhc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.zdbjq.cn/Article/details/gliuomjuo.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gbksnzati.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/gfwessviq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fehbvm.com/Article/details/gchffhpim.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/gywjfrihq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gjhywqsrw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/ghudfardp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/gqyjogwft.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.zdbjq.cn/Article/details/ggdawltfl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.zdbjq.cn/Article/details/gwaxvvngi.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/geavzqciy.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/goilujzsd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/gzxmbanvr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/gconggwan.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gkurwwspp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gkldbkpwr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/gnkihvzcs.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/gytifaphk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/gzlookovm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/geunikfbk.sHtML

[L06] 解析响应为 JSON
来源：http://wap.zdbjq.cn/Article/details/gvfdtbpys.sHtML

Py:   resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gtulpiqkb.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.hesvh.cn/Article/details/gyqlvkspp.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gvzteuzwm.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gpxtzxrps.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/grnblpjsw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/gepkwfmaz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/gbhfgzrhu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/gmpyssyfx.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/ghjxtrtwg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/ggkxymzxa.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/gujhgduvp.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gzmdtmgrt.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gjhronklz.sHtML

Java: resp.statusCode()
来源：http://www.blog.zdbjq.cn/Article/details/gjjhdjupe.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/ghzauumao.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fehbvm.com/Article/details/gbcudhdol.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gnfpnijht.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/grqeszami.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fehbvm.com/Article/details/gabntwlke.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gjsfappqr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gaapxktuh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gsusomtww.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fehbvm.com/Article/details/gnzbucreq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.zdbjq.cn/Article/details/gkpxtqyat.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/gsaaxfyxb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gpkhprcja.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gukkgypcw.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/gfqesskka.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/geqiqruxf.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/gibvynlny.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/giirysvdj.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gxslkpgru.sHtML


<!-- 参考信息 -->