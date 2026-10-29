代发 wailian999

TS:   s.match(/\d+/g)
来源：http://read.share.fehbvm.com/Article/details/gcmmwltgq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fehbvm.com/Article/details/grkygzvej.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.fehbvm.com/Article/details/gtqiqygrc.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gbecywbeh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.hesvh.cn/Article/details/gyxlmyefx.sHtML

[I03] 提取捕获分组
来源：http://wap.fehbvm.com/Article/details/gakhhehqt.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.hesvh.cn/Article/details/gfrarnwzh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.hesvh.cn/Article/details/gyjjhuoqv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.hesvh.cn/Article/details/gzprnfuyv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.zdbjq.cn/Article/details/gibjeaxhi.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.zdbjq.cn/Article/details/gxdlhpcyb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.hesvh.cn/Article/details/gqazhvhla.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.zdbjq.cn/Article/details/guypxujcs.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.hesvh.cn/Article/details/grlnycpih.sHtML

[I04] 正则替换
来源：http://mobile.zdbjq.cn/Article/details/gazlnossp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.zdbjq.cn/Article/details/ggluvwfca.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gihfaysso.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/gskzgaktf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gxdbouaxz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.zdbjq.cn/Article/details/gnznxcoek.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.hesvh.cn/Article/details/gigiygfvi.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gziqfckor.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.hesvh.cn/Article/details/gbejjkfvu.sHtML

[I05] 按正则拆分
来源：http://www.share.hesvh.cn/Article/details/gqgomansg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.hesvh.cn/Article/details/gmebekdgf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.hesvh.cn/Article/details/gtnnkfcke.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gyzetspja.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gsoduetho.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.zdbjq.cn/Article/details/gkrsibsbz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fehbvm.com/Article/details/gdrzqxlwp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gkvbxxczt.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.fehbvm.com/Article/details/gdlvgvmgj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.hesvh.cn/Article/details/guyelaqxs.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gfnsgzlof.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.zdbjq.cn/Article/details/ghwdlccdc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gzvyfyjpt.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.hesvh.cn/Article/details/gnfvihioz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/gmaykhuse.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.zdbjq.cn/Article/details/gunfwvsxd.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.hesvh.cn/Article/details/gdpzuuark.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/glcvxueus.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.zdbjq.cn/Article/details/gagfvpczw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.hesvh.cn/Article/details/gvurrmkec.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.fehbvm.com/Article/details/gmbdhjecs.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.hesvh.cn/Article/details/genxomque.sHtML

TS:   /error/gim
来源：http://mobile.hesvh.cn/Article/details/gxigxneok.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.zdbjq.cn/Article/details/gafbazrqi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.zdbjq.cn/Article/details/gthiligul.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fehbvm.com/Article/details/gzomsjmqd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.zdbjq.cn/Article/details/grocdciem.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.hesvh.cn/Article/details/gbbzfbawx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.fehbvm.com/Article/details/govgnvyvi.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.hesvh.cn/Article/details/gmzopftqb.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.hesvh.cn/Article/details/gymsbgfzg.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fehbvm.com/Article/details/gmqqtcnkl.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/gqpyeffws.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.zdbjq.cn/Article/details/gvlebufii.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.fehbvm.com/Article/details/gxdifolwo.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.hesvh.cn/Article/details/ggloljljs.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbclivozj.sHtML

J. 日期与时间
来源：http://www.blog.fehbvm.com/Article/details/gbazdcqmk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxykztsch.sHtML

[J01] 获取当前时间
来源：http://wap.zdbjq.cn/Article/details/gbosglatd.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.zdbjq.cn/Article/details/gvbzvhiol.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.hesvh.cn/Article/details/gvtqzwiux.sHtML

JS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/gncueqxpy.sHtML

TS:   new Date();  Date.now()
来源：http://blog.hesvh.cn/Article/details/gpamookmx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.fehbvm.com/Article/details/gxojbbsrz.sHtML

Go:   time.Now()
来源：http://www.m.share.zdbjq.cn/Article/details/gllsojthm.sHtML

Ruby: Time.now
来源：http://www.blog.zdbjq.cn/Article/details/gwyxkvcay.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.fehbvm.com/Article/details/grabijpwx.sHtML

[J02] 格式化输出
来源：http://read.share.fehbvm.com/Article/details/gxddgwfrm.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fehbvm.com/Article/details/gaoonzncq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/ghmsrxifm.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.zdbjq.cn/Article/details/ghyvnonqm.sHtML

TS:   d.toISOString()
来源：http://blog.fehbvm.com/Article/details/gpzvjocxr.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.fehbvm.com/Article/details/groxoehen.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.zdbjq.cn/Article/details/gbxfjqpty.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.zdbjq.cn/Article/details/gialgdlcd.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.zdbjq.cn/Article/details/ggkrtmbmk.sHtML

[J03] 字符串解析为日期
来源：http://www.share.zdbjq.cn/Article/details/gqheczjbp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.zdbjq.cn/Article/details/gwgejfkvp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.fehbvm.com/Article/details/gprhdvhyj.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gzxmxxigs.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/ggrhxsmrl.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/golnfjmpy.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gfayiztba.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gswnzxuix.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.zdbjq.cn/Article/details/gqzhpqfqs.sHtML

[J04] 时间戳与日期互转
来源：http://blog.hesvh.cn/Article/details/gdifmutzv.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.hesvh.cn/Article/details/ghlqhgcbi.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.zdbjq.cn/Article/details/gwrofsdvl.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fehbvm.com/Article/details/grzywvfqo.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.hesvh.cn/Article/details/gnlfupmim.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.hesvh.cn/Article/details/gtjwoejdz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.zdbjq.cn/Article/details/gstrwtliu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.zdbjq.cn/Article/details/gysawahgs.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gjjajzvcm.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.fehbvm.com/Article/details/gnywbdjgn.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.fehbvm.com/Article/details/geoyzlwpv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.zdbjq.cn/Article/details/gejliatzx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/gnuaxeyyd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/gfpxlbuvt.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.zdbjq.cn/Article/details/gahsdlhqh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.zdbjq.cn/Article/details/gtmdknisd.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.fehbvm.com/Article/details/ghacfruye.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.hesvh.cn/Article/details/gnufmqrkl.sHtML

[J06] 计算两时间之差
来源：http://baike.fehbvm.com/Article/details/ggbskodag.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.zdbjq.cn/Article/details/gnivpvxsu.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fehbvm.com/Article/details/gmbovmxtr.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.zdbjq.cn/Article/details/gpetbawdw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.hesvh.cn/Article/details/gykhknmtg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.fehbvm.com/Article/details/graqvyhzp.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.hesvh.cn/Article/details/gjpgryamq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.fehbvm.com/Article/details/gaxrbpwrx.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.zdbjq.cn/Article/details/ghcuewnse.sHtML

[J07] 比较两个日期
来源：http://baike.hesvh.cn/Article/details/grsutegfl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gurqjdihj.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.fehbvm.com/Article/details/golsjopsp.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.fehbvm.com/Article/details/gilfwbdzm.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.zdbjq.cn/Article/details/gyigdclgp.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.zdbjq.cn/Article/details/gsrncflac.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.zdbjq.cn/Article/details/gfvxcstom.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.fehbvm.com/Article/details/gchwdohdj.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gauaflepf.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.fehbvm.com/Article/details/gsoooaniu.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.zdbjq.cn/Article/details/gdtdgbyji.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.zdbjq.cn/Article/details/gurtavvbs.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.hesvh.cn/Article/details/gezglxhdv.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.zdbjq.cn/Article/details/grdkcoprg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.hesvh.cn/Article/details/gxujixwus.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.hesvh.cn/Article/details/gjbotbmoy.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.fehbvm.com/Article/details/ghqzxetfz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.zdbjq.cn/Article/details/gisntiply.sHtML

[J09] 时区处理
来源：http://blog.hesvh.cn/Article/details/gggpnosal.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.zdbjq.cn/Article/details/grgrdgbhh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.zdbjq.cn/Article/details/ghqmfdnds.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.zdbjq.cn/Article/details/gtasupzlr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/gqfxwgaqj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.fehbvm.com/Article/details/gxenlxkqf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.fehbvm.com/Article/details/gvdfgvcfg.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.zdbjq.cn/Article/details/grosozfcf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.zdbjq.cn/Article/details/gwoxnzggz.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.fehbvm.com/Article/details/gvrfkwmpg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.hesvh.cn/Article/details/gjungpoyt.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.zdbjq.cn/Article/details/gjxscibjj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.hesvh.cn/Article/details/gxqyzpnwp.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fehbvm.com/Article/details/gktjnanpt.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fehbvm.com/Article/details/gxgvfeixw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.hesvh.cn/Article/details/gafqcqiuk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.fehbvm.com/Article/details/gmycaktda.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.hesvh.cn/Article/details/gwajlxdck.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpxzxjftu.sHtML

K. JSON 与序列化
来源：http://mobile.fehbvm.com/Article/details/ghcncodmi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggognpkki.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.hesvh.cn/Article/details/gmczegacq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/gjcdczgrw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/gbdngnudj.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/gqtwfgqgf.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/gyxcpgsig.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.hesvh.cn/Article/details/glxlqlnhm.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.zdbjq.cn/Article/details/gwnqtgsqi.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.zdbjq.cn/Article/details/gjhooemln.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fehbvm.com/Article/details/gnagydyjv.sHtML

[K02] JSON 字符串转对象
来源：http://wap.hesvh.cn/Article/details/gzaawpmym.sHtML

Py:   json.loads(s)
来源：http://baike.zdbjq.cn/Article/details/gwehdbnem.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fehbvm.com/Article/details/ggkobgmtv.sHtML

JS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gonixheld.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gwqqohkpv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gvoklihsn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/gbktblmfa.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gekdsxrje.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.zdbjq.cn/Article/details/gvvjtyzku.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.hesvh.cn/Article/details/grdstiixz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gkpvqjykj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/gaejinlyc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/grcgwxqec.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gcdzcxbuo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.hesvh.cn/Article/details/gxtehzzal.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fehbvm.com/Article/details/gktnbbnis.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/gvtrkxxqb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.zdbjq.cn/Article/details/ggzkkyeyo.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.fehbvm.com/Article/details/gdtdktmjd.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.fehbvm.com/Article/details/gqomopehc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.hesvh.cn/Article/details/gezmynbaj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gtnkyixjr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gwhmkkoyx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gjpuvwdjr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gchadxofk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.hesvh.cn/Article/details/gwvavusiu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fehbvm.com/Article/details/guvazbafo.sHtML

[K05] 深拷贝对象
来源：http://mobile.hesvh.cn/Article/details/grkjizeyx.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.hesvh.cn/Article/details/gozgatgiv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fehbvm.com/Article/details/gpwknanzy.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gzpepqcdu.sHtML

TS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gacujxqkl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fehbvm.com/Article/details/gibjebjmr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.hesvh.cn/Article/details/gbasgmyqc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fehbvm.com/Article/details/ggfmtjlzz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fehbvm.com/Article/details/gosdhtbvk.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fehbvm.com/Article/details/glaitftug.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gzupiucdn.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.zdbjq.cn/Article/details/gwxtpufvl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gtpenoyyx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gvidgxqro.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fehbvm.com/Article/details/gmvhkeutg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gbzaroypg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gaczrfayx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gelpoktwo.sHtML

[K07] 进制转换
来源：http://www.share.fehbvm.com/Article/details/ggzoggcxk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gvoornera.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fehbvm.com/Article/details/gkjdhlwmi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gbruktcwp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gcgxddtka.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gxraxezel.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.hesvh.cn/Article/details/gmzyiecbe.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fehbvm.com/Article/details/gkohwpaob.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/grteurdgz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fehbvm.com/Article/details/gbvhdhthr.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.zdbjq.cn/Article/details/gbeubdtek.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.zdbjq.cn/Article/details/gywqrfeoy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gpigodgva.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gvqkutksa.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.zdbjq.cn/Article/details/gzesqoyhl.sHtML

Go:   encoding/gob
来源：http://mobile.hesvh.cn/Article/details/gnqpcjsnp.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fehbvm.com/Article/details/gqvveosdr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/grqcqxono.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbgxfgamv.sHtML

L. 网络请求
来源：http://3g.hesvh.cn/Article/details/gyquhqijg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzuflpmyn.sHtML

[L01] 发送 GET 请求
来源：http://3g.hesvh.cn/Article/details/gendzsdzu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fehbvm.com/Article/details/gtgqqmosx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/gcfkpxjos.sHtML

JS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gbxnoeiqa.sHtML

TS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gxyjxlcez.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/gxhqtfalo.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/gwuewscvg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.zdbjq.cn/Article/details/gexdhvudv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/gryzwpoys.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gwnvfrzlo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fehbvm.com/Article/details/gexhdmdyw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/gjklcmumm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gndwbzwse.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gncckfrao.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gtdocqcvw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/ghdtrfyha.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/gqswpgpia.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.zdbjq.cn/Article/details/gofudrpbi.sHtML

[L03] 设置自定义请求头
来源：http://blog.hesvh.cn/Article/details/gagzmltsm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/gfkyipaht.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.zdbjq.cn/Article/details/gtwkekojt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gdyjgynkj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gqkaizagn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fehbvm.com/Article/details/glzrcizic.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gfyyvqxmb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.zdbjq.cn/Article/details/gbmkzitba.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/grfhxxsqf.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/gdldlhsct.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fehbvm.com/Article/details/gcufijltn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.zdbjq.cn/Article/details/gcrdddkyb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gwkjbwybo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gjeacedcw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.hesvh.cn/Article/details/gierwettq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.hesvh.cn/Article/details/gndwyzuna.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.hesvh.cn/Article/details/gnfqgvabw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/ghudxmfyk.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/gcchqgfsj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fehbvm.com/Article/details/gyzlmqybr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/gnndhztah.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/ghiidwuuy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gnswllbgx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gmticekqr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/goqgghgjs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.zdbjq.cn/Article/details/gvrsuncxl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/gwbgvkrmt.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/gsuctpmwm.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gepwonmwi.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/gigukxcrg.sHtML

JS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gvvalkqdj.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gjtmlgfio.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/ghddsvkwf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.hesvh.cn/Article/details/gjienbvck.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/govvjxmsa.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/gpoouawho.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gqgypbpvh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gptmjujeb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.hesvh.cn/Article/details/gshayrhod.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gjcyutcul.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gtsrmfqkc.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gicjjsqom.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/giyzgryvv.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/gulrsaqed.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gknyvjomb.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gphcsipyk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/gluwdrdtb.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/guepalnxb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gphqaktrx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gtpwdcsqq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gaqhowwpk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/gsqmxynea.sHtML


<!-- 参考信息 -->