代发 wailian999

TS:   s.match(/\d+/g)
来源：http://baike.fehbvm.com/Article/details/gcgthhfwx.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.hesvh.cn/Article/details/gtujxiqst.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/galfafpbl.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.hesvh.cn/Article/details/grtrpfgxw.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fehbvm.com/Article/details/gsocpjyeh.sHtML

[I03] 提取捕获分组
来源：http://mobile.hesvh.cn/Article/details/gnclduyal.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fehbvm.com/Article/details/gzhppkzhc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.hesvh.cn/Article/details/gazdpccag.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fehbvm.com/Article/details/geqdwjtaf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.hesvh.cn/Article/details/gycdofcda.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.zdbjq.cn/Article/details/gqkzeqdeb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.hesvh.cn/Article/details/gqirstoma.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.zdbjq.cn/Article/details/glevokcmc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.fehbvm.com/Article/details/gsjcxhybw.sHtML

[I04] 正则替换
来源：http://mobile.hesvh.cn/Article/details/gzqjrzxxo.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.hesvh.cn/Article/details/gknawwoyt.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/guyryvogi.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/ggrwclavp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/gavlrrfwx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/gzlpfqgdj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.fehbvm.com/Article/details/ghlmbxpho.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gxlpvyrfs.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.fehbvm.com/Article/details/gidxxevdn.sHtML

[I05] 按正则拆分
来源：http://www.share.fehbvm.com/Article/details/gnddxfsea.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fehbvm.com/Article/details/glztscjyg.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.zdbjq.cn/Article/details/gtyomwjed.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gemhurzrn.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/geyzxsjav.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.fehbvm.com/Article/details/gvjpijnou.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fehbvm.com/Article/details/gomxtnfuo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gwqrcdxam.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.fehbvm.com/Article/details/gdbjzlqdb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.zdbjq.cn/Article/details/gbhxemzhf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gfnjnwtoj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.fehbvm.com/Article/details/gxyjaupxs.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/grpcpjjou.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/gczjkohau.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gzxdzvppk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.zdbjq.cn/Article/details/geiadrsyu.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.fehbvm.com/Article/details/gngwtieax.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gjyigpimg.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.zdbjq.cn/Article/details/gucwlnyod.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.zdbjq.cn/Article/details/gswuqccpt.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.zdbjq.cn/Article/details/grdayizws.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.hesvh.cn/Article/details/gwhoxinlr.sHtML

TS:   /error/gim
来源：http://wap.hesvh.cn/Article/details/gyucwqqns.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.fehbvm.com/Article/details/gxiebnlrx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.zdbjq.cn/Article/details/gntkrmume.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.zdbjq.cn/Article/details/gnoyynpyf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.fehbvm.com/Article/details/ghsojzapx.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.fehbvm.com/Article/details/gemscinsa.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.hesvh.cn/Article/details/ggdebyxnx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.fehbvm.com/Article/details/gsxccrgch.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/gkvnywoih.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.zdbjq.cn/Article/details/gmwbwugre.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/gixenkfui.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.zdbjq.cn/Article/details/gttvkculp.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fehbvm.com/Article/details/gybdlbqcj.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.fehbvm.com/Article/details/gdgacbtio.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdillaswe.sHtML

J. 日期与时间
来源：http://baike.hesvh.cn/Article/details/gxjvgmvan.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gywidsrpv.sHtML

[J01] 获取当前时间
来源：http://baike.fehbvm.com/Article/details/gsiczkvhf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fehbvm.com/Article/details/gcrnvqfzq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.fehbvm.com/Article/details/gifxvntag.sHtML

JS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/gonaycvgh.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fehbvm.com/Article/details/gtmdjifvx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.hesvh.cn/Article/details/gxfizffsr.sHtML

Go:   time.Now()
来源：http://baike.zdbjq.cn/Article/details/gucjfxrfn.sHtML

Ruby: Time.now
来源：http://m.share.hesvh.cn/Article/details/gowsmcsob.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.zdbjq.cn/Article/details/gjvhtoikp.sHtML

[J02] 格式化输出
来源：http://read.share.fehbvm.com/Article/details/gabfkbbcn.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.hesvh.cn/Article/details/gvpgyonby.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.zdbjq.cn/Article/details/gultncacx.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.hesvh.cn/Article/details/gppajwfjy.sHtML

TS:   d.toISOString()
来源：http://www.m.share.zdbjq.cn/Article/details/gnvesowzq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.zdbjq.cn/Article/details/gggzpemei.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.zdbjq.cn/Article/details/gqpowcdot.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/goavgrvcv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.fehbvm.com/Article/details/gfdrligou.sHtML

[J03] 字符串解析为日期
来源：http://m.share.fehbvm.com/Article/details/gordcgnal.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.hesvh.cn/Article/details/gygmbsvrx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.zdbjq.cn/Article/details/gzjayjscs.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gfdoxmjqs.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gdyiujhfv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gvgoblucv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gklnqtimr.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gstgjsmuj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.hesvh.cn/Article/details/gjfaclbae.sHtML

[J04] 时间戳与日期互转
来源：http://wap.hesvh.cn/Article/details/gabjbyvfl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.zdbjq.cn/Article/details/gnqgeihtg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.hesvh.cn/Article/details/goplfwqgs.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fehbvm.com/Article/details/gquivwuvi.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.zdbjq.cn/Article/details/grxkruoej.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.fehbvm.com/Article/details/gtxvifrqn.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fehbvm.com/Article/details/gvxbqnhuc.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.hesvh.cn/Article/details/gwufylwgn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gcxiejdxy.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.hesvh.cn/Article/details/gfibaftnm.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.hesvh.cn/Article/details/gfotmmmyo.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.fehbvm.com/Article/details/gqtwbkkas.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fehbvm.com/Article/details/geoawcnvd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.zdbjq.cn/Article/details/gcadvmybf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.zdbjq.cn/Article/details/gxtlvaxvc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fehbvm.com/Article/details/gtgxioajq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.fehbvm.com/Article/details/gnzpvkquz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/giqilmrdv.sHtML

[J06] 计算两时间之差
来源：http://m.share.zdbjq.cn/Article/details/gsddduzma.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.fehbvm.com/Article/details/geisrxdqj.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.zdbjq.cn/Article/details/gvrzrvybb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.hesvh.cn/Article/details/gonackmhc.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fehbvm.com/Article/details/gfzivdxjs.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.zdbjq.cn/Article/details/glaodrrtb.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.hesvh.cn/Article/details/gysxtxpno.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.zdbjq.cn/Article/details/glfdjjylu.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fehbvm.com/Article/details/grpuceptx.sHtML

[J07] 比较两个日期
来源：http://mobile.zdbjq.cn/Article/details/gnxplwwgb.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/gaotykqap.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.zdbjq.cn/Article/details/gljfmqyuk.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.fehbvm.com/Article/details/gpjttljra.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.fehbvm.com/Article/details/gruraknqd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.zdbjq.cn/Article/details/gulntjetc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.hesvh.cn/Article/details/gfwftjgoq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/gedsqntfh.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/gerrsjdkg.sHtML

[J08] 提取年月日与星期
来源：http://baike.hesvh.cn/Article/details/gjjzjmiwn.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fehbvm.com/Article/details/gkiyorsfu.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.hesvh.cn/Article/details/grsevxxrq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.fehbvm.com/Article/details/gxkytwkwl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.hesvh.cn/Article/details/gvfajezkh.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.zdbjq.cn/Article/details/gnxnymmpv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.zdbjq.cn/Article/details/gvduebgbd.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.zdbjq.cn/Article/details/gkoekkfby.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.fehbvm.com/Article/details/gczwrjvny.sHtML

[J09] 时区处理
来源：http://www.blog.zdbjq.cn/Article/details/gkpiaptst.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.hesvh.cn/Article/details/gyhnnpryl.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.zdbjq.cn/Article/details/gpukvkzpg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.hesvh.cn/Article/details/gazsvizkj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.hesvh.cn/Article/details/gjqvltwnk.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.fehbvm.com/Article/details/gntrsbspj.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.zdbjq.cn/Article/details/glectpkok.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.zdbjq.cn/Article/details/gomfmpptm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.fehbvm.com/Article/details/gjtgalfgr.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.hesvh.cn/Article/details/gynahejne.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.zdbjq.cn/Article/details/gylkipnem.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.hesvh.cn/Article/details/gusgbkvwh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.hesvh.cn/Article/details/gmtvxeucg.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gxnrlfsca.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.zdbjq.cn/Article/details/gpdcnmnqs.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fehbvm.com/Article/details/gjkncpege.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.zdbjq.cn/Article/details/gfksbflvz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fehbvm.com/Article/details/gobbikkuh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzsndbkia.sHtML

K. JSON 与序列化
来源：http://www.blog.zdbjq.cn/Article/details/gjtsqvmpk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsdnmereb.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.hesvh.cn/Article/details/ghzvqonkc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/gmbzcalzm.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/gyhrudroz.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/gufiripgj.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/gfbhbjgqz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.zdbjq.cn/Article/details/gqcltsyyt.sHtML

Go:   json.Marshal(obj)
来源：http://3g.zdbjq.cn/Article/details/gkrkrxdnk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.hesvh.cn/Article/details/ggqpgonin.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fehbvm.com/Article/details/gettswwrl.sHtML

[K02] JSON 字符串转对象
来源：http://baike.zdbjq.cn/Article/details/gamyziwko.sHtML

Py:   json.loads(s)
来源：http://www.share.hesvh.cn/Article/details/gipxvasww.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.zdbjq.cn/Article/details/gxpwmazdc.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/guuxzohdd.sHtML

TS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/getnqnsub.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gvfmhsgsm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/ggvtepana.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gemhnfhcy.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.hesvh.cn/Article/details/gotzvljnw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fehbvm.com/Article/details/gzzzqgcnv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/gmjuhnuya.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/gltljmmil.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gtznnzlqy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gwczxekqp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.hesvh.cn/Article/details/gjgoffxrq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.hesvh.cn/Article/details/gmyxoyoyr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.hesvh.cn/Article/details/gsxfxpbvj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.zdbjq.cn/Article/details/gvkiicqoi.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fehbvm.com/Article/details/gizhklxdi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fehbvm.com/Article/details/gbemzrgjy.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fehbvm.com/Article/details/gjxmbbhaj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/ggjcddmki.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/guzurtyez.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gqcdqwpfa.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gdkqmhlpl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gfphljgbv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/grzdwmjvp.sHtML

[K05] 深拷贝对象
来源：http://mobile.hesvh.cn/Article/details/gdkzmawrw.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.hesvh.cn/Article/details/gibfsiqeb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.hesvh.cn/Article/details/gmfsejfyr.sHtML

JS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gcyuniqoz.sHtML

TS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gyfvaoory.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.hesvh.cn/Article/details/gcpsafely.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.hesvh.cn/Article/details/ghafgqtrw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.hesvh.cn/Article/details/gduqjqumk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.fehbvm.com/Article/details/ghbpykwsk.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.hesvh.cn/Article/details/gyjitsuuj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gwtaaxwor.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.zdbjq.cn/Article/details/gnmsfqutd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/giytvtnsx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gqxqlvutl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.zdbjq.cn/Article/details/gfmtjitvb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gpdoenlit.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gpjexphmr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gpjsfwkyu.sHtML

[K07] 进制转换
来源：http://mobile.hesvh.cn/Article/details/gkcgbaeio.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gsemzucfz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fehbvm.com/Article/details/gwwninpen.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/ggzxpzdyp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/guvupddtn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/geosuyqqz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.zdbjq.cn/Article/details/ghliibdeg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.zdbjq.cn/Article/details/gfcjxfexn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gzbffhrrr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.hesvh.cn/Article/details/gtrkwbobe.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/gqsxhxqwf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fehbvm.com/Article/details/gkgsbddkb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gsgibgved.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/gthoacvhr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.hesvh.cn/Article/details/ghnjqzvhn.sHtML

Go:   encoding/gob
来源：http://baike.hesvh.cn/Article/details/gpfjsurax.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fehbvm.com/Article/details/gjvpseoqi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/glofbeldx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsxoxbvdb.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/gcklrcqmh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gedqxbarn.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fehbvm.com/Article/details/ghvxmfmya.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.zdbjq.cn/Article/details/gnuopvfxe.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.zdbjq.cn/Article/details/gvlhbtsit.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gpfuatetf.sHtML

TS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gmbvabqud.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.hesvh.cn/Article/details/gflopqidi.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/guwvnabbc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.hesvh.cn/Article/details/gpjcxjnnz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/gjcsafmod.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gfqrsxrkr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gqdzzvkfz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fehbvm.com/Article/details/gywgqejrw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gsrtijnpj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gwncmtaer.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.zdbjq.cn/Article/details/gqkpltkzl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fehbvm.com/Article/details/gatfszqdw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fehbvm.com/Article/details/gvwaapctg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.hesvh.cn/Article/details/gbmspunmq.sHtML

[L03] 设置自定义请求头
来源：http://3g.zdbjq.cn/Article/details/gschndbrl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.fehbvm.com/Article/details/gtlfgwevp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fehbvm.com/Article/details/gfaaqzbqg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gffhcfuyr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gedevsfar.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.hesvh.cn/Article/details/ggiumivok.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gbjrulmad.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.hesvh.cn/Article/details/guqymefbv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gfgnxkrsw.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gnzphwtxp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/gjlbpuvwo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.hesvh.cn/Article/details/gadhrfbso.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gjnydimkj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gcgwigjfg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.hesvh.cn/Article/details/gwmemgwlk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/gavplzrrp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/gfnaaegfp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.hesvh.cn/Article/details/gxlcdjvgo.sHtML

[L05] 上传文件（multipart）
来源：http://wap.zdbjq.cn/Article/details/gsxotkugl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fehbvm.com/Article/details/guhsbkual.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/gcixnpzmg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gyeryvlbz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gmxdhttre.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fehbvm.com/Article/details/gvvqxpayj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.hesvh.cn/Article/details/gthlwhvhr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/gvynolhbo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.zdbjq.cn/Article/details/guzfndtis.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/gkjvclknj.sHtML

Py:   resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gsctbpqtz.sHtML

PHP:  json_decode($body, true);
来源：http://wap.hesvh.cn/Article/details/gjnuwyoph.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/goroboinz.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gjhlfplqe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gbcqxxktf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.hesvh.cn/Article/details/gpswmgicw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.zdbjq.cn/Article/details/gfdchdiuh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/gdahlbszy.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gslomacfw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/gobnpgcsf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gqlzeowzd.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gomgrxedt.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gtxrlcvgn.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gxlvppbeh.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gghvjgbdn.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/gwlmubtwl.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gsxelwdmz.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/gdyrgyddo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.hesvh.cn/Article/details/gbuzmeulg.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.zdbjq.cn/Article/details/glvasxrke.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/ghvlbawyu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gdntdrhbn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/gjqdyfyjn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fehbvm.com/Article/details/gqxlqkqtv.sHtML


<!-- 参考信息 -->