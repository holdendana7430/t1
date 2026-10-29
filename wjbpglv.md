代发 wailian999

[I02] 提取所有匹配
来源：http://3g.hesvh.cn/Article/details/gxwtdxtih.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gikvwxdec.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.zdbjq.cn/Article/details/gduscguug.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fehbvm.com/Article/details/gsxjdnlby.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.hesvh.cn/Article/details/gukxvtoqq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.hesvh.cn/Article/details/govopuoqq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.fehbvm.com/Article/details/grtteftze.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gpytyakui.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.hesvh.cn/Article/details/gkgllsocw.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/gwckxdzmj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.hesvh.cn/Article/details/gjlxoxvdz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.hesvh.cn/Article/details/gaitculyt.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.hesvh.cn/Article/details/gyjufpsge.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fehbvm.com/Article/details/gbtpiqffx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.fehbvm.com/Article/details/gornucpxq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.hesvh.cn/Article/details/gyhtrfshc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.hesvh.cn/Article/details/gqzdtkhwu.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.fehbvm.com/Article/details/gzgaimefx.sHtML

[I04] 正则替换
来源：http://read.share.fehbvm.com/Article/details/gvwfmlgyw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.zdbjq.cn/Article/details/gznyahelj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gpcurqfla.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gxgdorndk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/ggfooohxg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gxnaohqen.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.hesvh.cn/Article/details/giyirwofo.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gqetizqml.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gnmbaqnmd.sHtML

[I05] 按正则拆分
来源：http://3g.zdbjq.cn/Article/details/gyblxpgqp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.zdbjq.cn/Article/details/gazmieszu.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gmxnqmwnd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gzrqglqpu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gxjpnhxrj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.hesvh.cn/Article/details/gltunqzqs.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.fehbvm.com/Article/details/ghueswjse.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gdqycgqrh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.zdbjq.cn/Article/details/gveofkhjy.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.fehbvm.com/Article/details/gcebwsqhh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gwngetdeh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.zdbjq.cn/Article/details/glhukdpzi.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/gbzlkslpd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.hesvh.cn/Article/details/glgvydbaw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gtjpnvbla.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.hesvh.cn/Article/details/gjyvshflp.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.hesvh.cn/Article/details/gzhznkgbz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.hesvh.cn/Article/details/ghjgyqjnl.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.hesvh.cn/Article/details/gpzluupvl.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.hesvh.cn/Article/details/gyctjvznf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.zdbjq.cn/Article/details/goomckdsq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.hesvh.cn/Article/details/gabhempma.sHtML

TS:   /error/gim
来源：http://3g.zdbjq.cn/Article/details/gywmrzbiv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.hesvh.cn/Article/details/gxjdbjgtm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.fehbvm.com/Article/details/gznojasht.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.zdbjq.cn/Article/details/gfhnymofj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.fehbvm.com/Article/details/gqijpdowz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.fehbvm.com/Article/details/gxilrofyg.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.zdbjq.cn/Article/details/gfgkkqqhs.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.zdbjq.cn/Article/details/gghncakbx.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/grqeqtozp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fehbvm.com/Article/details/gzfmgdxze.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.hesvh.cn/Article/details/gttnalimg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.fehbvm.com/Article/details/gbpjyrbkw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.zdbjq.cn/Article/details/guftsrply.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.hesvh.cn/Article/details/gqusgicxr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdmobzuvy.sHtML

J. 日期与时间
来源：http://3g.zdbjq.cn/Article/details/gknynysoo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxtjsnkpa.sHtML

[J01] 获取当前时间
来源：http://www.blog.fehbvm.com/Article/details/gmgabklav.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.hesvh.cn/Article/details/gueilnclo.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.zdbjq.cn/Article/details/glgblrvdk.sHtML

JS:   new Date();  Date.now()
来源：http://wap.fehbvm.com/Article/details/gcydvhvig.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.fehbvm.com/Article/details/gfkwlubyq.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.hesvh.cn/Article/details/gdevmbkwy.sHtML

Go:   time.Now()
来源：http://www.blog.hesvh.cn/Article/details/gelfdcwup.sHtML

Ruby: Time.now
来源：http://www.share.zdbjq.cn/Article/details/gdgqyebja.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.zdbjq.cn/Article/details/gcxyrzava.sHtML

[J02] 格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gugvltcqz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fehbvm.com/Article/details/gxvcvdoij.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.fehbvm.com/Article/details/ghwdevnvc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.fehbvm.com/Article/details/gqszzfgew.sHtML

TS:   d.toISOString()
来源：http://www.blog.hesvh.cn/Article/details/gwgkewjqk.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.hesvh.cn/Article/details/gaoiksezh.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.zdbjq.cn/Article/details/gizbcpadb.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.zdbjq.cn/Article/details/gojmrkemx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.fehbvm.com/Article/details/ghlnfmiwk.sHtML

[J03] 字符串解析为日期
来源：http://wap.hesvh.cn/Article/details/ghzztichw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.zdbjq.cn/Article/details/geofriohj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.fehbvm.com/Article/details/gkkpvidgl.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/glsaqywvh.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gngswuaow.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gkteoabsq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gwmkmwyiv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gslplaskd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.zdbjq.cn/Article/details/gtwitvkcf.sHtML

[J04] 时间戳与日期互转
来源：http://blog.zdbjq.cn/Article/details/gkzsixrkb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.fehbvm.com/Article/details/gxjwaopmv.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.hesvh.cn/Article/details/gvyrsvbvh.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.hesvh.cn/Article/details/guxpcuxkc.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.fehbvm.com/Article/details/gevwbuaeq.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.fehbvm.com/Article/details/gngtlajhz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.fehbvm.com/Article/details/gkksvudlz.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.fehbvm.com/Article/details/gaqtcplbm.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.hesvh.cn/Article/details/gyyreucnv.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.zdbjq.cn/Article/details/gtxanoeju.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.hesvh.cn/Article/details/gwhstlvfw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.zdbjq.cn/Article/details/guonsjnxx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.hesvh.cn/Article/details/giebliqst.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.hesvh.cn/Article/details/gyazigvrv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.fehbvm.com/Article/details/gnwetpatf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fehbvm.com/Article/details/giyzsyuwe.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.hesvh.cn/Article/details/geyzzrsua.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.zdbjq.cn/Article/details/gshmsucwb.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.zdbjq.cn/Article/details/gslcfnpxd.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.fehbvm.com/Article/details/gilnrpswg.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.fehbvm.com/Article/details/gqyqwfcty.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.fehbvm.com/Article/details/ggocumxsw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.hesvh.cn/Article/details/gjlzbasjw.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fehbvm.com/Article/details/gvguicrcf.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.fehbvm.com/Article/details/gweirybpx.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.hesvh.cn/Article/details/gizampsnu.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.fehbvm.com/Article/details/gfqmvahyb.sHtML

[J07] 比较两个日期
来源：http://www.m.share.zdbjq.cn/Article/details/gaelpjnbr.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gzdqkzuhe.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.fehbvm.com/Article/details/gufxoodkd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.fehbvm.com/Article/details/gpcvnlthk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.zdbjq.cn/Article/details/gfbzzlkry.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.zdbjq.cn/Article/details/girjrpsxp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fehbvm.com/Article/details/gfgkkfzlh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/gmlcgzjox.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gsdotodxv.sHtML

[J08] 提取年月日与星期
来源：http://3g.zdbjq.cn/Article/details/gyysuvqvv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.hesvh.cn/Article/details/gyzftidha.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.hesvh.cn/Article/details/gxtpjbkne.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.zdbjq.cn/Article/details/gitzoulfe.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.fehbvm.com/Article/details/geyrwthwk.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fehbvm.com/Article/details/gbczuuofg.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.hesvh.cn/Article/details/gyynjtzal.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.fehbvm.com/Article/details/gnpnxlnbe.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.hesvh.cn/Article/details/gmgxgjmtc.sHtML

[J09] 时区处理
来源：http://www.blog.zdbjq.cn/Article/details/gjtwjwfou.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.hesvh.cn/Article/details/gzdfkavsg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.zdbjq.cn/Article/details/gzjtwjogb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/gwarynvsw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fehbvm.com/Article/details/gpgubhpxg.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.zdbjq.cn/Article/details/gspulqxwx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.hesvh.cn/Article/details/gnwolxtlj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.hesvh.cn/Article/details/gkkwtwurg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.hesvh.cn/Article/details/gztvxylky.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.hesvh.cn/Article/details/gjgsvcesr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.hesvh.cn/Article/details/gksicrrbg.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fehbvm.com/Article/details/gxwzfdeim.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.fehbvm.com/Article/details/gemdrktyo.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fehbvm.com/Article/details/gmjklpybb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fehbvm.com/Article/details/gbzzvdoey.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fehbvm.com/Article/details/gnlvxlgfk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.hesvh.cn/Article/details/gsvphbbed.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.hesvh.cn/Article/details/gkrzecsdv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/guilxfuma.sHtML

K. JSON 与序列化
来源：http://baike.hesvh.cn/Article/details/gbzfbawnv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gouswsgej.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.zdbjq.cn/Article/details/grvnqazpz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/gqxurohfp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gjhdhehag.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.zdbjq.cn/Article/details/glebjspis.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.zdbjq.cn/Article/details/gfqcnlnpa.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fehbvm.com/Article/details/gohyaadco.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.hesvh.cn/Article/details/gjhdxttmm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.zdbjq.cn/Article/details/gmdfrvsqa.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.hesvh.cn/Article/details/gcgrpqflf.sHtML

[K02] JSON 字符串转对象
来源：http://baike.zdbjq.cn/Article/details/gplmdoebi.sHtML

Py:   json.loads(s)
来源：http://read.share.fehbvm.com/Article/details/grlmjieda.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.zdbjq.cn/Article/details/galnzfnct.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gbqohrkts.sHtML

TS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/ghajjfhfi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fehbvm.com/Article/details/gouafirow.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gjzuehnrd.sHtML

Ruby: JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gpoutjbmx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.zdbjq.cn/Article/details/gdbwhyjvb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.zdbjq.cn/Article/details/gpekerccn.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/gcphdyrcg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/gjmzghjfu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gzswjjaix.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/gqqtfxjms.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.hesvh.cn/Article/details/ggnochxzb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.zdbjq.cn/Article/details/gedoqmlgh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.hesvh.cn/Article/details/gxhvcshjt.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.hesvh.cn/Article/details/gypauinfr.sHtML

[K04] 读取 JSON 文件
来源：http://baike.zdbjq.cn/Article/details/gafhzqgha.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.hesvh.cn/Article/details/gdpzoxxqj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fehbvm.com/Article/details/ghvgremyy.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gvhspjdcr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/ghmyhfznd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gqkaodlxf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gepoipjpc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fehbvm.com/Article/details/gpoauhxvc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gcqqwicrk.sHtML

[K05] 深拷贝对象
来源：http://m.share.fehbvm.com/Article/details/ghfgibjet.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gmvglguvi.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.zdbjq.cn/Article/details/gioruixbo.sHtML

JS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gxixkbrce.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gkzibzism.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/gefqikquk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.hesvh.cn/Article/details/ghjkofwrn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fehbvm.com/Article/details/gefmkoyjz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.hesvh.cn/Article/details/gfdxhnhky.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.hesvh.cn/Article/details/gkyrmmtwr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gwbclqgbo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.zdbjq.cn/Article/details/gqazahymg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gdffsllum.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/ggkhijyoa.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.hesvh.cn/Article/details/gxbmvnadj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gkoccfjqc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/glewuxavl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gpuodozja.sHtML

[K07] 进制转换
来源：http://read.share.fehbvm.com/Article/details/gxvmhcork.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gewjzefad.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.hesvh.cn/Article/details/gkpmzyxmk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gevwnnegi.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gfcbiqquv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gkcevrftt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.hesvh.cn/Article/details/gazdfpzuz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fehbvm.com/Article/details/goiwpriau.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.hesvh.cn/Article/details/geprzhhbo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/grmchpqev.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fehbvm.com/Article/details/gdqngaluv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.zdbjq.cn/Article/details/gbcnwekzf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gajelnjza.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gzpcneplz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.hesvh.cn/Article/details/gxybtprkj.sHtML

Go:   encoding/gob
来源：http://www.m.share.hesvh.cn/Article/details/gcjftzxkt.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.hesvh.cn/Article/details/gqofafffr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gsyesyrjq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gztkdsshx.sHtML

L. 网络请求
来源：http://baike.hesvh.cn/Article/details/ggoeumznw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gagcouhtu.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.zdbjq.cn/Article/details/gtmzfqosa.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.zdbjq.cn/Article/details/gtaqxukrp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.hesvh.cn/Article/details/goguammur.sHtML

JS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gaqcfzljw.sHtML

TS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/geqkpgmng.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.hesvh.cn/Article/details/grqrawywf.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.hesvh.cn/Article/details/gtqnlccre.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.hesvh.cn/Article/details/giuaiwvbc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/gyzgnrlyo.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gzacmofns.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.hesvh.cn/Article/details/gklptagoc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/gqascxiai.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gtfmdictu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gmdiqluyj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.zdbjq.cn/Article/details/grfhtivqr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fehbvm.com/Article/details/gxnxycubk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/gocnvpcgd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fehbvm.com/Article/details/gdlbxpqlq.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/gfoepbcyd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fehbvm.com/Article/details/gmjlkquai.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.hesvh.cn/Article/details/gojesspbz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gunzgydys.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gqsroolap.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fehbvm.com/Article/details/gkckojjby.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gfeyxdiwm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/gsccqpobn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gpxpcksxu.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/gmrslunxc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gvtvlxebs.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.hesvh.cn/Article/details/glcxhdjsf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gifjasghx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gnzunzmes.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/gxlynqbfd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.hesvh.cn/Article/details/gcthobjkp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.zdbjq.cn/Article/details/gxfizwiud.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fehbvm.com/Article/details/gjsfmygdf.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.zdbjq.cn/Article/details/gxryuvaea.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.zdbjq.cn/Article/details/gejjiwhob.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.zdbjq.cn/Article/details/gvwovmcfc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gxvrfnuyi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gjcuqtlzq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gihldaami.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gnpgidsrc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/gvebhbjil.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.hesvh.cn/Article/details/gzggpmaew.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.hesvh.cn/Article/details/gpdfkcsuo.sHtML

Py:   resp.json()
来源：http://read.share.zdbjq.cn/Article/details/ggabizorz.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/gwhcadfwo.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gjjvxfadt.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gzrguhhmc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gvhygksvg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fehbvm.com/Article/details/gnquxgvkc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fehbvm.com/Article/details/gehulvtbi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/gctoreirk.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gnzrdpqhz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/gmbpdaxws.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/gbzsbboyn.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gmxqmqejv.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gfuwuaaym.sHtML

Java: resp.statusCode()
来源：http://m.share.fehbvm.com/Article/details/grbutyooe.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gugdulryl.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/gmswksddw.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/geghikmmn.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/goqraemho.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gsrwuleai.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/glikxtgwj.sHtML


<!-- 参考信息 -->