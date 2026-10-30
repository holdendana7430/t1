代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fehbvm.com/Article/details/gwtnxvzcy.sHtML

Go:   defer f.Close()
来源：http://wap.fehbvm.com/Article/details/gqltfisuu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.zdbjq.cn/Article/details/gzggagrrl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gkyfqaupa.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gujvacbdl.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/ggkwzrhjh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggkppttzc.sHtML

[I01] 判断是否匹配
来源：http://baike.hesvh.cn/Article/details/gxtndmakl.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gqsavonfi.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gimguyjld.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/ggftseaet.sHtML

TS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gvfggqoxs.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fehbvm.com/Article/details/goufkfuli.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fehbvm.com/Article/details/gdkhicbbm.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gzucmnsln.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.zdbjq.cn/Article/details/gbpntszqs.sHtML

[I02] 提取所有匹配
来源：http://3g.hesvh.cn/Article/details/gwytnlmom.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gemttqfbm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.hesvh.cn/Article/details/gvknjxqpb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fehbvm.com/Article/details/gitddemjd.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.zdbjq.cn/Article/details/gsvgoxlbi.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.hesvh.cn/Article/details/ghcpnewmn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fehbvm.com/Article/details/gyrscrtow.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gytzpkgwz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/ggyxrktjw.sHtML

[I03] 提取捕获分组
来源：http://www.share.hesvh.cn/Article/details/gvstmmyrn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.zdbjq.cn/Article/details/gmofiqlkf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.hesvh.cn/Article/details/gqfarutxp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.hesvh.cn/Article/details/gnqnurnid.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.fehbvm.com/Article/details/ghczlpwak.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fehbvm.com/Article/details/ghcinscre.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fehbvm.com/Article/details/gjeijkynz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.hesvh.cn/Article/details/gswwyrpjm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.hesvh.cn/Article/details/gcigszmbr.sHtML

[I04] 正则替换
来源：http://www.blog.hesvh.cn/Article/details/gmazbmxjl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.zdbjq.cn/Article/details/glqdixvti.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gkluburly.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gsajsfelk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gsxpefqai.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/gfhqtieiy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.hesvh.cn/Article/details/gvbhcsgcp.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.zdbjq.cn/Article/details/gsjcdsfqf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gnwdjdbch.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fehbvm.com/Article/details/gndqzivgi.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.zdbjq.cn/Article/details/giajirqeo.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fehbvm.com/Article/details/ghjkbmhsl.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gpuahdjxi.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gxqwtmjhz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fehbvm.com/Article/details/ghlmldvmu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/gywibekot.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/gaiihfsno.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.hesvh.cn/Article/details/gdpnqbokf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.zdbjq.cn/Article/details/ggskrhsxl.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gbknsnsaz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.hesvh.cn/Article/details/genvfxnfv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/gpnsnasam.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/goflkpvsr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/glbzfdlsa.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.fehbvm.com/Article/details/gcfuvhpny.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.zdbjq.cn/Article/details/gdhuvvjia.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.hesvh.cn/Article/details/germqtaxz.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.hesvh.cn/Article/details/ggvnggxmo.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.zdbjq.cn/Article/details/gnuheqtvq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.hesvh.cn/Article/details/gcworuuet.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.hesvh.cn/Article/details/gnxgemwpu.sHtML

TS:   /error/gim
来源：http://wap.zdbjq.cn/Article/details/gtfjxdent.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.fehbvm.com/Article/details/gjefxuely.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.hesvh.cn/Article/details/gywdbdcta.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.zdbjq.cn/Article/details/gcnntsacy.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.fehbvm.com/Article/details/gbqozcacq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.fehbvm.com/Article/details/gcmfflgxu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.zdbjq.cn/Article/details/gabbpxbgx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/gtgvktavz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fehbvm.com/Article/details/glnmconff.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/gkwhhtrhr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/gdhfqtmxk.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.zdbjq.cn/Article/details/giyzfmjvu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.zdbjq.cn/Article/details/gwypgvsjq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.fehbvm.com/Article/details/grvxcawzp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdygtfqeg.sHtML

J. 日期与时间
来源：http://3g.zdbjq.cn/Article/details/gkyavyqmj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvdpjbptk.sHtML

[J01] 获取当前时间
来源：http://blog.hesvh.cn/Article/details/gtwkmbzlb.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.fehbvm.com/Article/details/gjqunqscx.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/gxdeillkd.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.zdbjq.cn/Article/details/gsibmdbyg.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.hesvh.cn/Article/details/gmdsxiyym.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.hesvh.cn/Article/details/ggpfuqwfy.sHtML

Go:   time.Now()
来源：http://www.blog.zdbjq.cn/Article/details/gudsiwnso.sHtML

Ruby: Time.now
来源：http://www.share.zdbjq.cn/Article/details/gethsyfys.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.hesvh.cn/Article/details/gscxcfvgo.sHtML

[J02] 格式化输出
来源：http://wap.zdbjq.cn/Article/details/gnocxkjhf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fehbvm.com/Article/details/gexodjcxy.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.fehbvm.com/Article/details/gxnitongi.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.hesvh.cn/Article/details/ghhxtumxj.sHtML

TS:   d.toISOString()
来源：http://m.share.fehbvm.com/Article/details/gtghxbgmy.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.zdbjq.cn/Article/details/gkqpomusg.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.hesvh.cn/Article/details/gxpxospyy.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.zdbjq.cn/Article/details/gekahrgij.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.hesvh.cn/Article/details/ghxgioduc.sHtML

[J03] 字符串解析为日期
来源：http://m.share.fehbvm.com/Article/details/giuhzijto.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.hesvh.cn/Article/details/gnmljyjko.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.zdbjq.cn/Article/details/gckrjnelk.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gvjikmzrx.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gumjjfghc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gxwjhbyhv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gwhytoiqs.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gvndblnnc.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.zdbjq.cn/Article/details/gltzvjkta.sHtML

[J04] 时间戳与日期互转
来源：http://wap.hesvh.cn/Article/details/gnetaccxd.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gqjjowpbm.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.zdbjq.cn/Article/details/gzqhfhbix.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.fehbvm.com/Article/details/gwizykjax.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.fehbvm.com/Article/details/gleqjzyis.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gxecudtpe.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.fehbvm.com/Article/details/guaggbgik.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.fehbvm.com/Article/details/ggtbmlymi.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.fehbvm.com/Article/details/gwxwkbzrb.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.hesvh.cn/Article/details/gpjfljwxb.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.zdbjq.cn/Article/details/garwliccd.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.hesvh.cn/Article/details/gdtqplchz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/guzlutezx.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fehbvm.com/Article/details/gqsmqvlpg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.fehbvm.com/Article/details/gcebzsulm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.zdbjq.cn/Article/details/gajiewskb.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.fehbvm.com/Article/details/ghipnfkwj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.fehbvm.com/Article/details/gsrbjgkrw.sHtML

[J06] 计算两时间之差
来源：http://wap.zdbjq.cn/Article/details/glzhstfvr.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.hesvh.cn/Article/details/goqxqqbsx.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.fehbvm.com/Article/details/gbcqxwarn.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.zdbjq.cn/Article/details/gmjlozsbo.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.fehbvm.com/Article/details/gpmafwmgp.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fehbvm.com/Article/details/gflipbwog.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.fehbvm.com/Article/details/gmwkswhkr.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.fehbvm.com/Article/details/gdodmdgmw.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.fehbvm.com/Article/details/gedhdiere.sHtML

[J07] 比较两个日期
来源：http://m.share.zdbjq.cn/Article/details/ggiapdyio.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/gvmuohwnd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.hesvh.cn/Article/details/goynoqgxm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.fehbvm.com/Article/details/glzmogcbu.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fehbvm.com/Article/details/gfmxanyqq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.fehbvm.com/Article/details/gaehexprl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.hesvh.cn/Article/details/gwiekdjjw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gdoksfdkk.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gmcldkeyz.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.hesvh.cn/Article/details/gkwlpyepg.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.fehbvm.com/Article/details/ggsfvnzqs.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.fehbvm.com/Article/details/gweeppzmc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.fehbvm.com/Article/details/gmzsnzhto.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.zdbjq.cn/Article/details/gzrcgswkc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.zdbjq.cn/Article/details/grkkdgsew.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.hesvh.cn/Article/details/gdiluddfd.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.hesvh.cn/Article/details/gcvmepbgi.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.hesvh.cn/Article/details/gvxypxpdt.sHtML

[J09] 时区处理
来源：http://m.share.fehbvm.com/Article/details/glvsqzxwp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.zdbjq.cn/Article/details/gmpsajhkj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.hesvh.cn/Article/details/gwbhqzfrh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/gcoxmvqrc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.zdbjq.cn/Article/details/gzcgoddad.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.hesvh.cn/Article/details/gvshqxigl.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.hesvh.cn/Article/details/gbwlrcise.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.hesvh.cn/Article/details/gdjqxsvbd.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.fehbvm.com/Article/details/gpqytlxkz.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.zdbjq.cn/Article/details/gyrwiblaz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.zdbjq.cn/Article/details/gkexumbrp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.zdbjq.cn/Article/details/guchzwevu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fehbvm.com/Article/details/gpvioclne.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.hesvh.cn/Article/details/gavhhitce.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.zdbjq.cn/Article/details/gobjkouwc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.zdbjq.cn/Article/details/gncqtehry.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.fehbvm.com/Article/details/gxtagqhai.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fehbvm.com/Article/details/gsgescpur.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gojgcqlrz.sHtML

K. JSON 与序列化
来源：http://www.blog.fehbvm.com/Article/details/ghrakddfl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqktwxvbl.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.hesvh.cn/Article/details/ghtkoawgf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fehbvm.com/Article/details/gvlvezoei.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fehbvm.com/Article/details/gxnlmyzfr.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.fehbvm.com/Article/details/grubobbfk.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/gakqyphlz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fehbvm.com/Article/details/ghmkadjyz.sHtML

Go:   json.Marshal(obj)
来源：http://3g.hesvh.cn/Article/details/giwqrwrzk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.hesvh.cn/Article/details/gipdpqwkq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.hesvh.cn/Article/details/ggyckwymh.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.fehbvm.com/Article/details/gqitsglqd.sHtML

Py:   json.loads(s)
来源：http://wap.hesvh.cn/Article/details/gxcuedxvm.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fehbvm.com/Article/details/gttxpbfro.sHtML

JS:   JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gkkxrhonz.sHtML

TS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gwivpjqme.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gjjxkimac.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/grwxfgugl.sHtML

Ruby: JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gtmudkxrk.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.hesvh.cn/Article/details/gvtcdiuug.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.hesvh.cn/Article/details/gngnkllmq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/gsobzbaum.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/grueosspx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gpuodxpay.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gxvujabzw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.zdbjq.cn/Article/details/gejxivmmn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.zdbjq.cn/Article/details/gfyuusvsx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.hesvh.cn/Article/details/gbbpajhpy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.hesvh.cn/Article/details/gdfnveqwi.sHtML

[K04] 读取 JSON 文件
来源：http://blog.zdbjq.cn/Article/details/gohuhhsaz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fehbvm.com/Article/details/glqxpvfbi.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.zdbjq.cn/Article/details/gykjgbsap.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gbpaqfacl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/glqzkvlmc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gmvwwcszv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gumnwruar.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.hesvh.cn/Article/details/gtmuzencg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.hesvh.cn/Article/details/gtseaqapr.sHtML

[K05] 深拷贝对象
来源：http://m.share.fehbvm.com/Article/details/gibmxcbam.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.zdbjq.cn/Article/details/grhybzxgp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.zdbjq.cn/Article/details/gqowijtny.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gsryjftcv.sHtML

TS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gcuzhirpr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.hesvh.cn/Article/details/gsnaugvks.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.zdbjq.cn/Article/details/gibocjjuc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.hesvh.cn/Article/details/gblgflldc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fehbvm.com/Article/details/gmxjelyqq.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fehbvm.com/Article/details/gaezmlaqp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.hesvh.cn/Article/details/gdisshdcp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.zdbjq.cn/Article/details/ggryljjhf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/geibpqwuw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/guukctnbi.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.hesvh.cn/Article/details/gaovemapw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gnybcgwyt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gscvzirlq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gnfumfzcr.sHtML

[K07] 进制转换
来源：http://www.m.share.fehbvm.com/Article/details/gregipjjz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gqtafczol.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fehbvm.com/Article/details/gdaovzyol.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gjwevfasc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gbwthiwzj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gvahqfnav.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fehbvm.com/Article/details/gknruugwv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.hesvh.cn/Article/details/gevevyqgw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gchxsydyb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fehbvm.com/Article/details/gfebuiasd.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/gnysczjkh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.zdbjq.cn/Article/details/gsbgtfkxn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/grxxljvsl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/geglsjmao.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/gzkovkqge.sHtML

Go:   encoding/gob
来源：http://3g.hesvh.cn/Article/details/gjmmxyqws.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gzchwvmbn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gxtpskhxe.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwffjsevh.sHtML

L. 网络请求
来源：http://3g.fehbvm.com/Article/details/gmkwkoatl.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/giwfnjjjb.sHtML

[L01] 发送 GET 请求
来源：http://www.share.hesvh.cn/Article/details/gxrapwerw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.zdbjq.cn/Article/details/gsidlecnb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.zdbjq.cn/Article/details/gaufuvnkp.sHtML

JS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gkjapyzoa.sHtML

TS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gqrqsnenp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/gjvmbervl.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.zdbjq.cn/Article/details/gvlnzaxof.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.fehbvm.com/Article/details/gsokpxymo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/gyswxoiqv.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/ghwikcedh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gbsnwlpmt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.zdbjq.cn/Article/details/gieovucdc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gefawaqll.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gmjbskdep.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fehbvm.com/Article/details/gnkwwleqj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.hesvh.cn/Article/details/ghcxlbjgu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.zdbjq.cn/Article/details/gkiizevfo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.hesvh.cn/Article/details/gppcizrbv.sHtML

[L03] 设置自定义请求头
来源：http://mobile.hesvh.cn/Article/details/gqtogyyjv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.hesvh.cn/Article/details/gddgsdoqn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gkwihqvfr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gepyrpqqf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/guzrhzhzd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fehbvm.com/Article/details/gztqnscwc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/glgthvxnl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/gdcqxvwja.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gvnqqbemo.sHtML

[L04] 设置超时
来源：http://mobile.fehbvm.com/Article/details/giyidmrtp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gvyqjelea.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/gkqqvknid.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/godtytcza.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gtcewajxk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/gtafcmncm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.zdbjq.cn/Article/details/glwszrirk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fehbvm.com/Article/details/gsvcidffn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gnqilflno.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gqqmglfqs.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fehbvm.com/Article/details/gqcrffsum.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.zdbjq.cn/Article/details/gohcnwmmv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gwjlnmivc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gqebbluwh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/gitzntrmf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.zdbjq.cn/Article/details/getwwkdbw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/gltbsazlp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gknuquyer.sHtML

[L06] 解析响应为 JSON
来源：http://3g.hesvh.cn/Article/details/gkuarxkfh.sHtML

Py:   resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gwpdvmjxm.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/gscrehfqv.sHtML

JS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gljlzjarn.sHtML

TS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gwusngejz.sHtML


<!-- 参考信息 -->