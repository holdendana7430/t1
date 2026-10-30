代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.hesvh.cn/Article/details/ghyoppfbh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.hesvh.cn/Article/details/gmcwfljwm.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/gsjxizmcu.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fehbvm.com/Article/details/gvibwvxug.sHtML

[I02] 提取所有匹配
来源：http://mobile.fehbvm.com/Article/details/gqkfkzjwg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/gkopdkzzc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.hesvh.cn/Article/details/gxnexwdwr.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.zdbjq.cn/Article/details/gizochrmj.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.hesvh.cn/Article/details/gzaghfruh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.zdbjq.cn/Article/details/gubuenjlw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.zdbjq.cn/Article/details/gkswebmep.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.hesvh.cn/Article/details/gahjfvcrw.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fehbvm.com/Article/details/gpzsrdpib.sHtML

[I03] 提取捕获分组
来源：http://baike.fehbvm.com/Article/details/grinlpvsm.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.zdbjq.cn/Article/details/gayydgdoo.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.zdbjq.cn/Article/details/gplvahtnq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.hesvh.cn/Article/details/gadvkhtuj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.hesvh.cn/Article/details/giexuxblz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fehbvm.com/Article/details/goepoacdk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.hesvh.cn/Article/details/goqrrwewk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.zdbjq.cn/Article/details/ghqwsxpbc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.hesvh.cn/Article/details/gbuwmbakz.sHtML

[I04] 正则替换
来源：http://read.share.zdbjq.cn/Article/details/gasfqjped.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.zdbjq.cn/Article/details/gxhrtvzke.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gzvmharrh.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/gahwhvjxb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gsmcfotru.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.hesvh.cn/Article/details/goxdqmxta.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.zdbjq.cn/Article/details/gmulvlnnz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.zdbjq.cn/Article/details/gfsbazswf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gxbpvfepc.sHtML

[I05] 按正则拆分
来源：http://baike.hesvh.cn/Article/details/gtzjacglv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.hesvh.cn/Article/details/gmbtsfxxg.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gfitjlnmg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gxwuwkqha.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gyzmwkzid.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.fehbvm.com/Article/details/gnxzwwlum.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/ghjhoswfc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gscjzlmen.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.zdbjq.cn/Article/details/geyxhbotn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.zdbjq.cn/Article/details/gkwqzvbic.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gkcjykxfj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.hesvh.cn/Article/details/gzajmljvm.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/gvufofhie.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.hesvh.cn/Article/details/gzcmbyxmg.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/ghygbylpd.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.zdbjq.cn/Article/details/gmiynxfmm.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.zdbjq.cn/Article/details/gbamtzlel.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gscafaaox.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.hesvh.cn/Article/details/gkvekjvyv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.fehbvm.com/Article/details/grferytjh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/gfzhtkwod.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.zdbjq.cn/Article/details/gcoajxvnk.sHtML

TS:   /error/gim
来源：http://www.m.share.hesvh.cn/Article/details/gldhxqvmc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.zdbjq.cn/Article/details/grcvwhmzt.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.fehbvm.com/Article/details/gqzwleskw.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.fehbvm.com/Article/details/gqclcwlxz.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.hesvh.cn/Article/details/gbvvzmpqb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.zdbjq.cn/Article/details/gkcfsetqg.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.fehbvm.com/Article/details/gbzcuvwep.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.hesvh.cn/Article/details/gbumvmwvt.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.zdbjq.cn/Article/details/gftbslkfp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/gbiacejuk.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/gekmjgvdx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.zdbjq.cn/Article/details/gvwslizbm.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.hesvh.cn/Article/details/gkyivwdlq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/gpkuksjou.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gusiqepuz.sHtML

J. 日期与时间
来源：http://wap.fehbvm.com/Article/details/gglljwcyn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwvmppfqe.sHtML

[J01] 获取当前时间
来源：http://www.m.share.hesvh.cn/Article/details/grpatrovk.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.hesvh.cn/Article/details/ghzhvtznx.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.fehbvm.com/Article/details/gldfdovhe.sHtML

JS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/gboltreps.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fehbvm.com/Article/details/gogbnhcbv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.hesvh.cn/Article/details/gwkcixarh.sHtML

Go:   time.Now()
来源：http://wap.fehbvm.com/Article/details/gfwwrezbw.sHtML

Ruby: Time.now
来源：http://www.blog.hesvh.cn/Article/details/gftgbdxyv.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.zdbjq.cn/Article/details/gtrbgxysa.sHtML

[J02] 格式化输出
来源：http://www.share.fehbvm.com/Article/details/gbemijxui.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.hesvh.cn/Article/details/gevbfhbwq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fehbvm.com/Article/details/gxqvufflu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.zdbjq.cn/Article/details/gqajvqppq.sHtML

TS:   d.toISOString()
来源：http://baike.hesvh.cn/Article/details/gzbnyzopi.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.hesvh.cn/Article/details/gvsbfiyyl.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.hesvh.cn/Article/details/gulveqvlz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.zdbjq.cn/Article/details/gcjrsdrqc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.zdbjq.cn/Article/details/ghxxqqxwm.sHtML

[J03] 字符串解析为日期
来源：http://read.share.zdbjq.cn/Article/details/ggnigbkat.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.hesvh.cn/Article/details/gmkplhgvv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.hesvh.cn/Article/details/gckyvtcjw.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gczvqootg.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gturuszun.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/ghyojiido.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gcvbdfyfa.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gaqrzklkv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.zdbjq.cn/Article/details/gydiqniwh.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.zdbjq.cn/Article/details/gwkrhwjum.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.zdbjq.cn/Article/details/gwmtwuweg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fehbvm.com/Article/details/giskqobzv.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.hesvh.cn/Article/details/gjwwenmbr.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.hesvh.cn/Article/details/gnalwfrsx.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.fehbvm.com/Article/details/ggdohxfct.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.zdbjq.cn/Article/details/gwqznvrfk.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.hesvh.cn/Article/details/gxkxqaxbf.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.hesvh.cn/Article/details/gwuhnpcau.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.zdbjq.cn/Article/details/gyvxnoqrb.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.zdbjq.cn/Article/details/gpxqkarvk.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.hesvh.cn/Article/details/gzfxrlwwx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.zdbjq.cn/Article/details/gicgdhhir.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.hesvh.cn/Article/details/gkzdqstdz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.hesvh.cn/Article/details/gwyhlyhtb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.hesvh.cn/Article/details/greadrgvg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.fehbvm.com/Article/details/gomegepkj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.hesvh.cn/Article/details/gttlchnnj.sHtML

[J06] 计算两时间之差
来源：http://www.blog.zdbjq.cn/Article/details/gcuujffnd.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.zdbjq.cn/Article/details/gamehgslr.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.zdbjq.cn/Article/details/glubqkwhy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.zdbjq.cn/Article/details/gfrwkjwrb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.zdbjq.cn/Article/details/gbnxlvsyk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.hesvh.cn/Article/details/gyrzdgxgp.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.hesvh.cn/Article/details/ggqiqqiez.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.fehbvm.com/Article/details/goxbqbvxs.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.fehbvm.com/Article/details/geyjxskhf.sHtML

[J07] 比较两个日期
来源：http://www.m.share.zdbjq.cn/Article/details/ghkqgkhai.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gcvnckoeu.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.hesvh.cn/Article/details/gdyrkkylh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.hesvh.cn/Article/details/gilcgijik.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/gmonwmfcs.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.zdbjq.cn/Article/details/gdfqnyspq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fehbvm.com/Article/details/guqrgxcft.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gsepolubs.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/gqlodlyov.sHtML

[J08] 提取年月日与星期
来源：http://mobile.fehbvm.com/Article/details/gzebyjqvq.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.zdbjq.cn/Article/details/gmgqmugwe.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.hesvh.cn/Article/details/gebaiwlot.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.zdbjq.cn/Article/details/glogzuzag.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.zdbjq.cn/Article/details/goswwydmk.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.hesvh.cn/Article/details/gwdfguivq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.hesvh.cn/Article/details/gapbmncdk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.zdbjq.cn/Article/details/gkrhrprep.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.zdbjq.cn/Article/details/gykgimnwf.sHtML

[J09] 时区处理
来源：http://www.blog.zdbjq.cn/Article/details/guckvsqts.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.hesvh.cn/Article/details/gohvvvkbd.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.zdbjq.cn/Article/details/gtshexowo.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fehbvm.com/Article/details/gvhyjxzkx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/gqaevgepe.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.zdbjq.cn/Article/details/gbmqsenln.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.zdbjq.cn/Article/details/ghfxfusdz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.zdbjq.cn/Article/details/guvavtgve.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.fehbvm.com/Article/details/grlbeishp.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.zdbjq.cn/Article/details/gkvoizybg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fehbvm.com/Article/details/grpcxvkin.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.zdbjq.cn/Article/details/gcacnwdwi.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.hesvh.cn/Article/details/gcdlbfcyk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.hesvh.cn/Article/details/gsrlwsctp.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.zdbjq.cn/Article/details/gtmfluibi.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fehbvm.com/Article/details/gmptqozcm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.hesvh.cn/Article/details/gytubhcwl.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.hesvh.cn/Article/details/grsjwihpu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkgvfviae.sHtML

K. JSON 与序列化
来源：http://mobile.fehbvm.com/Article/details/gywvgjrmz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guyhaztlv.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.fehbvm.com/Article/details/gkzxvubtk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/gauttupvc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/gsvphbwgs.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gcfhdqxje.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.zdbjq.cn/Article/details/gryyrvoec.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.zdbjq.cn/Article/details/gfrhmpocu.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.hesvh.cn/Article/details/glvfrwfhb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.zdbjq.cn/Article/details/gcqmxtmve.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fehbvm.com/Article/details/gcxbwaajv.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fehbvm.com/Article/details/grdisiobl.sHtML

Py:   json.loads(s)
来源：http://baike.zdbjq.cn/Article/details/guorulnpv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.zdbjq.cn/Article/details/gkiebyicz.sHtML

JS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gxgfyetfq.sHtML

TS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gfqrvnpqx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.hesvh.cn/Article/details/gectrhghn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gxgrwqayr.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gyrkrqpfv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.hesvh.cn/Article/details/gcblricqx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.hesvh.cn/Article/details/geunpgseq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.fehbvm.com/Article/details/gibutceat.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/gwtkhphzq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gkomdbpys.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gcfvxlkzz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gjbouycsk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.zdbjq.cn/Article/details/gocnxwbdb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.zdbjq.cn/Article/details/gnwqdukqj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.hesvh.cn/Article/details/gquxxpquf.sHtML

[K04] 读取 JSON 文件
来源：http://wap.fehbvm.com/Article/details/grnvnxtvi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fehbvm.com/Article/details/gqrfbatqu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.hesvh.cn/Article/details/gmprawgib.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/ghsdfmawn.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/gzmlesokz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gthazzszn.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/gvvszzsrd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gklzupurb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fehbvm.com/Article/details/grnuhyixy.sHtML

[K05] 深拷贝对象
来源：http://mobile.hesvh.cn/Article/details/gpgsplwlm.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gtqlederl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.zdbjq.cn/Article/details/gpemowxra.sHtML

JS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gcurkckga.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gwnwzbtmd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.zdbjq.cn/Article/details/gbperfrat.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.fehbvm.com/Article/details/gweyagpsx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fehbvm.com/Article/details/gcvtgavqm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.zdbjq.cn/Article/details/gqwtlrsbb.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fehbvm.com/Article/details/gbtzvftbi.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gjirhrhjr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.zdbjq.cn/Article/details/gtuqpmmor.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gukdpmavd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/ggggkfglr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.zdbjq.cn/Article/details/goonrzpmk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gnifhphkv.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gfqsjexlt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gyierfrlo.sHtML

[K07] 进制转换
来源：http://www.m.share.fehbvm.com/Article/details/gjyfchxps.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gnlufdosm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.hesvh.cn/Article/details/gnrxvusap.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gwvduhngd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gktwgsstq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gofhtighk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fehbvm.com/Article/details/gnbxstesl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.hesvh.cn/Article/details/ggbktkfxy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gaxshuqsv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/goahzhrap.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.hesvh.cn/Article/details/gpnztkins.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.zdbjq.cn/Article/details/gopwysyzi.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gdfkomdfq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gjavxgwsz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.hesvh.cn/Article/details/gbocqmfnm.sHtML

Go:   encoding/gob
来源：http://m.share.hesvh.cn/Article/details/guraovdat.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fehbvm.com/Article/details/gvtftwzds.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gmwttcgha.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gylzkhkwm.sHtML

L. 网络请求
来源：http://www.share.zdbjq.cn/Article/details/gwtfqyeog.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbqxuymgl.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fehbvm.com/Article/details/gzcrenepn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.hesvh.cn/Article/details/glxsphsry.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.zdbjq.cn/Article/details/gxnynorzj.sHtML

JS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gafpasmof.sHtML

TS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gryryvuef.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.hesvh.cn/Article/details/gvqtkzykb.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.hesvh.cn/Article/details/gcwnnxmak.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.hesvh.cn/Article/details/gptptfymw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.hesvh.cn/Article/details/ggfksmcaj.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gcgpdcqrq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/gknenxmjm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/gbngobnpv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gqyfjydwd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gppaxwker.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.hesvh.cn/Article/details/ghwgsxlvb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.hesvh.cn/Article/details/ghocoewej.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/guyukjdop.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/gdeynsedr.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/gvzqoawqp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fehbvm.com/Article/details/gzcbgjsyp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fehbvm.com/Article/details/gegcgeqvn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gkidufnnd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gugrenbrh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.hesvh.cn/Article/details/grqfwtrlr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gppglmylp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/gevonssln.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gxxsahkvu.sHtML

[L04] 设置超时
来源：http://3g.fehbvm.com/Article/details/gmrykyufw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.hesvh.cn/Article/details/gsnzcssof.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fehbvm.com/Article/details/guryxaaki.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gmztrcjsu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gnozvkzdb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fehbvm.com/Article/details/ghdkkxatb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/gtfrrljnd.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/ghvihgpmj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.hesvh.cn/Article/details/ggoifecuu.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/glhzmnlme.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/gdxkfjjep.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/gpoaqezua.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gotszqqlp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gzsjlgwts.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/gklcokvdv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/gsclrtduy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.zdbjq.cn/Article/details/gemjhmyxy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gpzspoqoa.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/gudsdvvfr.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/glzqwbqrb.sHtML

PHP:  json_decode($body, true);
来源：http://wap.hesvh.cn/Article/details/goealnbts.sHtML

JS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/ghznqscdp.sHtML

TS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gfwoimwbc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/giojfrsjk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/gawszyfym.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/gjjfoqeyv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.zdbjq.cn/Article/details/guggsvqhl.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gziwyspyg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gojybdjvt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gjqowdkyr.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gvxfejddt.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gylxgrjng.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/gtszcjvrv.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gnkefccep.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/gwelffhcp.sHtML


<!-- 参考信息 -->