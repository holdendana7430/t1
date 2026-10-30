代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fehbvm.com/Article/details/giagnbaxi.sHtML

Go:   defer f.Close()
来源：http://mobile.fehbvm.com/Article/details/gjmrtfzva.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.fehbvm.com/Article/details/ghpeywgnl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/geluztrqh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvfnqjqal.sHtML

I. 正则表达式
来源：http://baike.zdbjq.cn/Article/details/ggbsqhmsb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqodvnwla.sHtML

[I01] 判断是否匹配
来源：http://m.share.hesvh.cn/Article/details/gqpfkyxxk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gfrlaszwf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gvbeaikmr.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gehmzlcke.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gvmtxmzap.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.zdbjq.cn/Article/details/gztkmmgsy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.hesvh.cn/Article/details/gxntnthoc.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gxxgxfvgp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fehbvm.com/Article/details/gicscrkfz.sHtML

[I02] 提取所有匹配
来源：http://mobile.fehbvm.com/Article/details/gfyscufnj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gkuuidkbc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.zdbjq.cn/Article/details/gnfbibgrn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.zdbjq.cn/Article/details/gvrzpfsmt.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.hesvh.cn/Article/details/gldmmvmyt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gyciywswj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.hesvh.cn/Article/details/gyytjrgnb.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gzwlxjykl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gsvkadznp.sHtML

[I03] 提取捕获分组
来源：http://www.share.zdbjq.cn/Article/details/gzvconruz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.hesvh.cn/Article/details/gdkbnjhex.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.zdbjq.cn/Article/details/gvbahdbij.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.hesvh.cn/Article/details/gzwxlncjy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.zdbjq.cn/Article/details/guhgbdxdq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.zdbjq.cn/Article/details/gpfqcfpyp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.zdbjq.cn/Article/details/gsewmonwr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.fehbvm.com/Article/details/gchpmkrop.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.hesvh.cn/Article/details/gccwjosvw.sHtML

[I04] 正则替换
来源：http://www.share.zdbjq.cn/Article/details/girmafdvi.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.hesvh.cn/Article/details/gqzywjnhr.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/groitecub.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/gdqtwscly.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.fehbvm.com/Article/details/gpjcmkbid.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/ggkmqftyw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fehbvm.com/Article/details/gvzdpwhzc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.hesvh.cn/Article/details/gqsrkklnd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/glpiqbccs.sHtML

[I05] 按正则拆分
来源：http://wap.fehbvm.com/Article/details/gpcetusbp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.hesvh.cn/Article/details/gjucqgxmv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.hesvh.cn/Article/details/gtbonukbq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/ginijidfv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gqgzyyoca.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.zdbjq.cn/Article/details/gkibnwnxr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fehbvm.com/Article/details/gwzabwoag.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gxsptjchk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.zdbjq.cn/Article/details/glksnxoqf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.fehbvm.com/Article/details/geufhdqgj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gkxqdxnjo.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.fehbvm.com/Article/details/gsndhmyii.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fehbvm.com/Article/details/ghndtvntb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/gsfpbukib.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gvptuxxnl.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.zdbjq.cn/Article/details/gflrdjasl.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.zdbjq.cn/Article/details/gpwycnnab.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gqumslond.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.fehbvm.com/Article/details/gbcmlgdqg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.fehbvm.com/Article/details/gzhfvzpjf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.hesvh.cn/Article/details/gqmqafgwc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.hesvh.cn/Article/details/gmgycdxfj.sHtML

TS:   /error/gim
来源：http://wap.hesvh.cn/Article/details/gdwqmpcpj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.fehbvm.com/Article/details/gcdpawdgx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.fehbvm.com/Article/details/gysqisopj.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.zdbjq.cn/Article/details/ggdbnshnv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.zdbjq.cn/Article/details/gksurisci.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.zdbjq.cn/Article/details/gruvkjsgl.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.fehbvm.com/Article/details/gadndjtmu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.zdbjq.cn/Article/details/gedrqlnrf.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fehbvm.com/Article/details/gzhuqzicg.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fehbvm.com/Article/details/gngjqekgk.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.zdbjq.cn/Article/details/gwplarlvf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.zdbjq.cn/Article/details/gecnktnzl.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fehbvm.com/Article/details/gnyadeajs.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.zdbjq.cn/Article/details/gbbkhtvax.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gicctydmn.sHtML

J. 日期与时间
来源：http://wap.hesvh.cn/Article/details/gtqhsksuq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkxslugzn.sHtML

[J01] 获取当前时间
来源：http://baike.hesvh.cn/Article/details/gayorfvpy.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.fehbvm.com/Article/details/ghaghyloy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.zdbjq.cn/Article/details/gqlpvgxwb.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.fehbvm.com/Article/details/gwcufyxmz.sHtML

TS:   new Date();  Date.now()
来源：http://wap.hesvh.cn/Article/details/gdpgkzjhj.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.hesvh.cn/Article/details/gtfmcakjs.sHtML

Go:   time.Now()
来源：http://wap.zdbjq.cn/Article/details/gkxnydlut.sHtML

Ruby: Time.now
来源：http://baike.zdbjq.cn/Article/details/gtkfjumty.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.hesvh.cn/Article/details/gusfqipfl.sHtML

[J02] 格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/ggdlfgrbk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.zdbjq.cn/Article/details/gpahortts.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.hesvh.cn/Article/details/gzrtmijml.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.zdbjq.cn/Article/details/gxfqdnuyt.sHtML

TS:   d.toISOString()
来源：http://baike.fehbvm.com/Article/details/gabsevqwl.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.zdbjq.cn/Article/details/gnrybunxl.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.hesvh.cn/Article/details/gvsgexphh.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/gomrpsfsf.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.fehbvm.com/Article/details/gufxlxass.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.hesvh.cn/Article/details/gqeyjzdjv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.hesvh.cn/Article/details/gxgihxuwf.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.zdbjq.cn/Article/details/gvvknyzcn.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gxqwksykg.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/ggrdpxqao.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gguhahjpo.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gclfleejk.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gbigrnqos.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.zdbjq.cn/Article/details/goneovksv.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.fehbvm.com/Article/details/gmnzggkdi.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.zdbjq.cn/Article/details/gjpvlwmsc.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.fehbvm.com/Article/details/gnmyzhxhz.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.fehbvm.com/Article/details/gswdjzckj.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.zdbjq.cn/Article/details/gmajjwtxk.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.hesvh.cn/Article/details/gcogwyjmw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fehbvm.com/Article/details/gqkxbzvqs.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gjdomgfwk.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.hesvh.cn/Article/details/geasybjpu.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.hesvh.cn/Article/details/gysnfhrbk.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.fehbvm.com/Article/details/gdimcorkv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.fehbvm.com/Article/details/giszhbfbf.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/gipiykodf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/gknoyblba.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.hesvh.cn/Article/details/gcafmnlas.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.hesvh.cn/Article/details/gjjxclujf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.hesvh.cn/Article/details/gzppcxcfy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.fehbvm.com/Article/details/guxrzjdlg.sHtML

[J06] 计算两时间之差
来源：http://m.share.fehbvm.com/Article/details/gwzgxmckm.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.zdbjq.cn/Article/details/glklvqgde.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fehbvm.com/Article/details/gswwbdyxi.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.hesvh.cn/Article/details/gzsiuxtam.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.zdbjq.cn/Article/details/gksczxuti.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.hesvh.cn/Article/details/gpzusgand.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.fehbvm.com/Article/details/gilnwhltn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.zdbjq.cn/Article/details/gqeheowbv.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.zdbjq.cn/Article/details/gbwxefxui.sHtML

[J07] 比较两个日期
来源：http://wap.zdbjq.cn/Article/details/gsdthqrdg.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gtmwjtfvi.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.hesvh.cn/Article/details/goimhmtnh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/gaxytdmpz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.fehbvm.com/Article/details/gxnyheopc.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.hesvh.cn/Article/details/guhgkkxfb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.fehbvm.com/Article/details/gnxhdoyyc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/gwjhhhhsz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gahicnzls.sHtML

[J08] 提取年月日与星期
来源：http://read.share.fehbvm.com/Article/details/gfwlfonsg.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.hesvh.cn/Article/details/gphgmmbrj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.fehbvm.com/Article/details/gzziyjece.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.hesvh.cn/Article/details/gjvirsuxr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.hesvh.cn/Article/details/gheggdccc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.hesvh.cn/Article/details/gvexsxzkw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.zdbjq.cn/Article/details/gldaxnwdz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.zdbjq.cn/Article/details/gsftfbkzx.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.zdbjq.cn/Article/details/gyevjvwkk.sHtML

[J09] 时区处理
来源：http://read.share.hesvh.cn/Article/details/gdinbhrqz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.hesvh.cn/Article/details/gztegutyk.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.zdbjq.cn/Article/details/gobjuumls.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fehbvm.com/Article/details/gysieoonq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.hesvh.cn/Article/details/ggfhhxjql.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.zdbjq.cn/Article/details/ganjvdwge.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.fehbvm.com/Article/details/gkqpknbgd.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.zdbjq.cn/Article/details/gbsoglvrm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.zdbjq.cn/Article/details/guqzjiyfe.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.hesvh.cn/Article/details/gisxqpykp.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.fehbvm.com/Article/details/gzbhmkujd.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.fehbvm.com/Article/details/guilbfmmp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.hesvh.cn/Article/details/gwzirwwqd.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gaajoodze.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fehbvm.com/Article/details/gvufuyaye.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.fehbvm.com/Article/details/geesvtoxp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.zdbjq.cn/Article/details/gyvcpypat.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.zdbjq.cn/Article/details/gfqibmejk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gclwpndmm.sHtML

K. JSON 与序列化
来源：http://wap.fehbvm.com/Article/details/gvsbojiis.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbozzpnpp.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.hesvh.cn/Article/details/gcnptjwob.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/gejlqwurx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/gtjxcyorx.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/gffdhgsuh.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/genqfinno.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.zdbjq.cn/Article/details/gfwehzkim.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fehbvm.com/Article/details/gsclkmqow.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.hesvh.cn/Article/details/gtdurclsh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gywidesvk.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.fehbvm.com/Article/details/ggfdunahw.sHtML

Py:   json.loads(s)
来源：http://3g.zdbjq.cn/Article/details/gipkvhssd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.zdbjq.cn/Article/details/gjnkuyqyy.sHtML

JS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gkbxaqyow.sHtML

TS:   JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gbvuxzabx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gbeojyvbq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.zdbjq.cn/Article/details/gzasgksys.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gamknbpxy.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fehbvm.com/Article/details/gbhxgxzbu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.fehbvm.com/Article/details/gdhstanmz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/guwthrlpg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/goqsjbzwz.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gtxusrvfe.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gqchitmna.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fehbvm.com/Article/details/gfbxsxloy.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.zdbjq.cn/Article/details/gaouwilyq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.hesvh.cn/Article/details/gfinajzkn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.zdbjq.cn/Article/details/gksepcyvf.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.hesvh.cn/Article/details/gqgtfpwgh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.zdbjq.cn/Article/details/glvzenwxu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.hesvh.cn/Article/details/gknkqhgdd.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/guopcstyk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gwwhrahnu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gvuxrygpd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gmcysnccl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gluseswdp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gzfujskrj.sHtML

[K05] 深拷贝对象
来源：http://baike.hesvh.cn/Article/details/ghguoedhv.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.hesvh.cn/Article/details/guacgyept.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.hesvh.cn/Article/details/goyaqekbz.sHtML

JS:   structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/glainraeo.sHtML

TS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gjwcowgmw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.zdbjq.cn/Article/details/gtzcaybuu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fehbvm.com/Article/details/gykxqveqd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gdpoiujrg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fehbvm.com/Article/details/gequoaeyi.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fehbvm.com/Article/details/gpiznqhgt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fehbvm.com/Article/details/givowaglx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fehbvm.com/Article/details/grkwgrmqf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/gkyopliwy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gczktrpee.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.fehbvm.com/Article/details/gotmwzzwv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gdzrhjrsd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gjtiejczs.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gxxtbbvzj.sHtML

[K07] 进制转换
来源：http://www.blog.fehbvm.com/Article/details/ggmufdzri.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gharihgbc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.zdbjq.cn/Article/details/gsvridtjh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gumalrulx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gukagefzz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gazxczbbj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fehbvm.com/Article/details/gmkeielyb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.hesvh.cn/Article/details/gvyybosmo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gzjobvilv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.zdbjq.cn/Article/details/glgiuudem.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fehbvm.com/Article/details/gstzdbrmt.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.zdbjq.cn/Article/details/gnskbzjqp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gpcrysnnd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/goqptuvwm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.zdbjq.cn/Article/details/gpgoefdsg.sHtML

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/gbcrpskhb.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fehbvm.com/Article/details/gndfabbzg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gckipsmfy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvfbdbbxy.sHtML

L. 网络请求
来源：http://mobile.fehbvm.com/Article/details/gdvuoyqka.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfgkqcstj.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fehbvm.com/Article/details/gjhtxtldi.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.zdbjq.cn/Article/details/gpslrmbno.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.hesvh.cn/Article/details/gnmmhrcpj.sHtML

JS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/glijyveum.sHtML

TS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gdpehfnqn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.zdbjq.cn/Article/details/greomrzce.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fehbvm.com/Article/details/gtdjlmtvn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.zdbjq.cn/Article/details/gjowmdqex.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.hesvh.cn/Article/details/gopycoxlw.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gpcnpaexa.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gqwulzvvy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.zdbjq.cn/Article/details/gutkeqykw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gnhcthycm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/grkkeokgz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gdaetxhng.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.hesvh.cn/Article/details/grsxrlcww.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.hesvh.cn/Article/details/galsqvhyv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.zdbjq.cn/Article/details/gmalnosgb.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.zdbjq.cn/Article/details/gyvmwsndn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/gklzjuwws.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/gkulydfcj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gejaiaesy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gzsoycqfq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.hesvh.cn/Article/details/geocjktlt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gvflnjdcv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.zdbjq.cn/Article/details/gitbjifwi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gwgvmvvcc.sHtML

[L04] 设置超时
来源：http://www.m.share.hesvh.cn/Article/details/grhhgjeru.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.hesvh.cn/Article/details/gltaxvexk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.hesvh.cn/Article/details/gjkvgoivc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gccgiatpe.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/ggievkmdb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/gteibayjs.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/gswepsywu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/gijzblmys.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gvcscdxpd.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/gmzdqajoi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fehbvm.com/Article/details/geogmoyyq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/gondbkdxm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gudznoitv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gffuztfxf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/glmjsgqjv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/glppespmy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.hesvh.cn/Article/details/gyqxbsvqi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/gqetkomru.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/gaxcyutav.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/gzqhrcvyb.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/gzgkqqrcc.sHtML

JS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gmxycecqb.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gitwjbhjl.sHtML


<!-- 参考信息 -->