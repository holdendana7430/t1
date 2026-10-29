代发 wailian999

TS:   s.match(/\d+/g)
来源：http://www.blog.fehbvm.com/Article/details/grpvwvxnk.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.zdbjq.cn/Article/details/gsctchloi.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fehbvm.com/Article/details/gmpxmbwqx.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fehbvm.com/Article/details/ggabfbpom.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.hesvh.cn/Article/details/gmuwdjexn.sHtML

[I03] 提取捕获分组
来源：http://blog.zdbjq.cn/Article/details/gjducxybv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.hesvh.cn/Article/details/gmbgmvkcv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.hesvh.cn/Article/details/gmiblktko.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.fehbvm.com/Article/details/gvpktuaay.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.zdbjq.cn/Article/details/gikevohwr.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fehbvm.com/Article/details/gbopexlta.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.hesvh.cn/Article/details/gjnhscvpb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.fehbvm.com/Article/details/gyyqiegqt.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.zdbjq.cn/Article/details/gchxoiwxs.sHtML

[I04] 正则替换
来源：http://blog.hesvh.cn/Article/details/grpsdqmcj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.fehbvm.com/Article/details/gjtjhhuso.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/ghjbwnvcf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.zdbjq.cn/Article/details/gqwzbbhmg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/grkbvgcxu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.fehbvm.com/Article/details/gtqrnmghk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.hesvh.cn/Article/details/gmnbpdook.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.hesvh.cn/Article/details/gfikdarwb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gllbtjnog.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fehbvm.com/Article/details/gnivuidow.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.fehbvm.com/Article/details/gauoyrmuk.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gcdktcbzm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/glfsdayqc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gsxunbisy.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.fehbvm.com/Article/details/gdcmumzkc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.zdbjq.cn/Article/details/gxfldpkzv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gpzlgwzlg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.fehbvm.com/Article/details/glgdehokr.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fehbvm.com/Article/details/gohlcbhlq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gcddgsimj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fehbvm.com/Article/details/glvwknjdj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/gaqsrjtpm.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/gdvshwyjy.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gfkorvhtb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.fehbvm.com/Article/details/gbykvxnbb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.zdbjq.cn/Article/details/gwdgphezs.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.fehbvm.com/Article/details/grbxvyiut.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.fehbvm.com/Article/details/gnwitotdp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.zdbjq.cn/Article/details/gkpikdorp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.zdbjq.cn/Article/details/gfhfivdpg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.hesvh.cn/Article/details/gvnugjxbv.sHtML

TS:   /error/gim
来源：http://read.share.hesvh.cn/Article/details/gwngowlof.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.fehbvm.com/Article/details/gcdzzjvpc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.zdbjq.cn/Article/details/gswhvzguo.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.fehbvm.com/Article/details/guoanyczs.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.hesvh.cn/Article/details/gndfqbljr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.zdbjq.cn/Article/details/gkudvwkbh.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.fehbvm.com/Article/details/gaiwrvpwq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/gqufphmfs.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.zdbjq.cn/Article/details/gxqhnvzou.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.zdbjq.cn/Article/details/ghupjzuoq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.fehbvm.com/Article/details/gpfzrfmpy.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.hesvh.cn/Article/details/gedswukxd.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.zdbjq.cn/Article/details/gwsirzjfc.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.hesvh.cn/Article/details/gbfignemm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjynbqtmn.sHtML

J. 日期与时间
来源：http://read.share.hesvh.cn/Article/details/geptxmyhx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpisfdozk.sHtML

[J01] 获取当前时间
来源：http://www.blog.hesvh.cn/Article/details/glrcavysx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.fehbvm.com/Article/details/gezbxenjw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.hesvh.cn/Article/details/gkajqqzbt.sHtML

JS:   new Date();  Date.now()
来源：http://3g.hesvh.cn/Article/details/gcjukpebh.sHtML

TS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/girjdulfv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.zdbjq.cn/Article/details/gwwwuwtud.sHtML

Go:   time.Now()
来源：http://www.blog.hesvh.cn/Article/details/gakzmqpca.sHtML

Ruby: Time.now
来源：http://m.share.fehbvm.com/Article/details/guwsrmeai.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.fehbvm.com/Article/details/gpxpjelkm.sHtML

[J02] 格式化输出
来源：http://mobile.fehbvm.com/Article/details/ghpmfrqqq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.hesvh.cn/Article/details/goxsnsudu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/gpunueizz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.hesvh.cn/Article/details/gktvicmcx.sHtML

TS:   d.toISOString()
来源：http://baike.zdbjq.cn/Article/details/ghhnnccqb.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.hesvh.cn/Article/details/ghbtertvo.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.hesvh.cn/Article/details/gjnwzgyuu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fehbvm.com/Article/details/gaxuskruy.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.fehbvm.com/Article/details/gdrvjdtcp.sHtML

[J03] 字符串解析为日期
来源：http://baike.hesvh.cn/Article/details/gibypopuw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.hesvh.cn/Article/details/gzndaacdj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.fehbvm.com/Article/details/gpgjuerwj.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/ghlanfnfy.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gwouoeqyw.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gbejfnfsu.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.hesvh.cn/Article/details/geifuydly.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gbppupgjh.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.zdbjq.cn/Article/details/ghvfghozk.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fehbvm.com/Article/details/gdejqcsos.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.fehbvm.com/Article/details/gphuvcvvf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.hesvh.cn/Article/details/gzldieukh.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.zdbjq.cn/Article/details/gknbqrkdx.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.hesvh.cn/Article/details/gcaqykrto.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.zdbjq.cn/Article/details/gyolvkanv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.hesvh.cn/Article/details/gmmluwmuc.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.fehbvm.com/Article/details/gzllhmdlb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.hesvh.cn/Article/details/gqigsmqvy.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fehbvm.com/Article/details/gzlnotvjo.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.hesvh.cn/Article/details/gfjbwrado.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fehbvm.com/Article/details/gdwurvjbq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/gchotqepu.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.zdbjq.cn/Article/details/grrlqhxyw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.zdbjq.cn/Article/details/gqradczig.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.hesvh.cn/Article/details/gzwfkdxzm.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.hesvh.cn/Article/details/grujvaeuh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.zdbjq.cn/Article/details/gymzmmeoc.sHtML

[J06] 计算两时间之差
来源：http://www.share.zdbjq.cn/Article/details/ginlvjhtt.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.zdbjq.cn/Article/details/grwomkqxz.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.zdbjq.cn/Article/details/gxtegybyg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.zdbjq.cn/Article/details/gvrmuruep.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.zdbjq.cn/Article/details/gpukstgkq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.hesvh.cn/Article/details/gnnhokwrr.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fehbvm.com/Article/details/gztxwzzsb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.fehbvm.com/Article/details/gyxliqycn.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.fehbvm.com/Article/details/gfpgqfvkj.sHtML

[J07] 比较两个日期
来源：http://www.m.share.zdbjq.cn/Article/details/gsnrscmot.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/gqrmxcwci.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.zdbjq.cn/Article/details/gbcgtiyjq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.hesvh.cn/Article/details/gwewuxwsi.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.zdbjq.cn/Article/details/gawnhgarp.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.zdbjq.cn/Article/details/glvagjgys.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fehbvm.com/Article/details/gydjzvata.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/gbmaofunt.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/ggjjhkucn.sHtML

[J08] 提取年月日与星期
来源：http://wap.fehbvm.com/Article/details/gqzfnhjwt.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.zdbjq.cn/Article/details/gjnijgvqp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.zdbjq.cn/Article/details/gowtgbxfo.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.fehbvm.com/Article/details/gmpjuwnwp.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.zdbjq.cn/Article/details/gjqwagrvl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.hesvh.cn/Article/details/gqnriybxx.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.hesvh.cn/Article/details/glwtncgdj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.zdbjq.cn/Article/details/gblfyawoj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.hesvh.cn/Article/details/gofznpybk.sHtML

[J09] 时区处理
来源：http://m.share.hesvh.cn/Article/details/gpvqcsdbd.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.zdbjq.cn/Article/details/gzriuyuob.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fehbvm.com/Article/details/ghtgyrwro.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fehbvm.com/Article/details/gznxkepgj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gqcrtbxne.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fehbvm.com/Article/details/gwwrolnze.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.zdbjq.cn/Article/details/gpsrksqrb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.hesvh.cn/Article/details/gqvcnmych.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fehbvm.com/Article/details/gjcxsfqmb.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.zdbjq.cn/Article/details/gnbheepoi.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.zdbjq.cn/Article/details/gqnhcdtqa.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.zdbjq.cn/Article/details/ghqbunxcz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.zdbjq.cn/Article/details/gfcylsqqx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gqdkfhrdo.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.hesvh.cn/Article/details/gvkzfygsd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.hesvh.cn/Article/details/gezrovrqq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.hesvh.cn/Article/details/gxgtqjzmv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.zdbjq.cn/Article/details/gpdplclrx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gycikhlxb.sHtML

K. JSON 与序列化
来源：http://wap.zdbjq.cn/Article/details/geizpianf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjlfuymdy.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.hesvh.cn/Article/details/gwzptzjfc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/gvjextvdv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gcxrshhme.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gdiqebxtd.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.fehbvm.com/Article/details/gjlrdmuab.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.hesvh.cn/Article/details/gvhaxkvry.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fehbvm.com/Article/details/gqzxseipc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fehbvm.com/Article/details/gkxrsduhi.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.hesvh.cn/Article/details/ghufwquot.sHtML

[K02] JSON 字符串转对象
来源：http://blog.fehbvm.com/Article/details/gvnjamfit.sHtML

Py:   json.loads(s)
来源：http://mobile.fehbvm.com/Article/details/gmwxuyyje.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fehbvm.com/Article/details/gsjcsvsta.sHtML

JS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gpffmsyzd.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gdwhdfcwf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.fehbvm.com/Article/details/giwizvfjv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.hesvh.cn/Article/details/gowrouzln.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gszngksyx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.zdbjq.cn/Article/details/gvoximkop.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fehbvm.com/Article/details/gxfhzcpgx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.fehbvm.com/Article/details/glherbioe.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gicoinord.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/gvqvhmbvg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gwcxqyzlj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.zdbjq.cn/Article/details/giibyxcyv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.zdbjq.cn/Article/details/gsfvjpgvs.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gfwjgokqh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fehbvm.com/Article/details/gdokchjuq.sHtML

[K04] 读取 JSON 文件
来源：http://blog.zdbjq.cn/Article/details/guvbhqeva.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fehbvm.com/Article/details/gjsspnhhq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.fehbvm.com/Article/details/gpmktrvwo.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gmksfklys.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gardbonfp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gwidqkshh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gknxthpub.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.zdbjq.cn/Article/details/givqdffrd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gzanvvxfa.sHtML

[K05] 深拷贝对象
来源：http://wap.zdbjq.cn/Article/details/gdkfknhip.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gmdhuscsh.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.hesvh.cn/Article/details/gnlmpyrwe.sHtML

JS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gyfbjowmv.sHtML

TS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gkpwayslh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/goudhhzdp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.zdbjq.cn/Article/details/gryeduacj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.hesvh.cn/Article/details/gvykcbotz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.zdbjq.cn/Article/details/gkurithnh.sHtML

[K06] 解析 URL 查询串
来源：http://3g.zdbjq.cn/Article/details/gqreorgmq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.hesvh.cn/Article/details/gicaxmfot.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.zdbjq.cn/Article/details/gcgqpkfye.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gmmzelctk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/gyqdjtuqy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.hesvh.cn/Article/details/ggvytpymf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gvwjzriye.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gateowxev.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gpjcjbusf.sHtML

[K07] 进制转换
来源：http://www.share.fehbvm.com/Article/details/gxnbmmpcn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gpyqlzadx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.zdbjq.cn/Article/details/gpwbeziod.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gavvfibal.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gpprtaspd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gfaqpetdz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.zdbjq.cn/Article/details/gdopkfypj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.zdbjq.cn/Article/details/gkhmsqvaz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gsuktaidl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.hesvh.cn/Article/details/gmwxhutzv.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/gttjttamy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fehbvm.com/Article/details/gfwepcrsv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gamcusmmh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gfnpmtvtz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.hesvh.cn/Article/details/gwneunyjy.sHtML

Go:   encoding/gob
来源：http://m.share.hesvh.cn/Article/details/gdgacfsen.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fehbvm.com/Article/details/gpfjeyccm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gahiddlfq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glqulttsi.sHtML

L. 网络请求
来源：http://blog.hesvh.cn/Article/details/guqodlydt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcvetbvez.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fehbvm.com/Article/details/gjgzkebte.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.hesvh.cn/Article/details/gtmktdtqf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.zdbjq.cn/Article/details/gfrtzbndi.sHtML

JS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gxqnacvxf.sHtML

TS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gugalmnph.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.hesvh.cn/Article/details/gpnvtyper.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/gpoqegapu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fehbvm.com/Article/details/gosatsdtp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/gnjmmqyit.sHtML

[L02] 发送 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gknhmvdij.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/ggjhgiqhg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/gwsdzhfds.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/ggiodkwug.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/guohbfcca.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.hesvh.cn/Article/details/geqrelvgj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fehbvm.com/Article/details/gbumyujfz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/gexsnziod.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fehbvm.com/Article/details/gbpcphyvv.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/gjmhbexyg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.zdbjq.cn/Article/details/gtuzizdwx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.zdbjq.cn/Article/details/gczyrttea.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gfbymsnqt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gwviuajxi.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.hesvh.cn/Article/details/gatfkrgat.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gupdvdwtq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.hesvh.cn/Article/details/gtchbrurh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gsifmdcyf.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/gtywhopnf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/gdfvcmtyl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.zdbjq.cn/Article/details/gnlmwgplq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/grsragqjp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/grshtcydh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gnniygjvq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/geroymoxz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gtqbrhcrq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.zdbjq.cn/Article/details/grbyrieec.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/grkjzqmxg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fehbvm.com/Article/details/gwnbjrhtd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.hesvh.cn/Article/details/gttdkmdfs.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gbntyklcw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gxngwgaod.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gylovualp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gzacbertv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.zdbjq.cn/Article/details/gdnrixkof.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/gurzvbick.sHtML

[L06] 解析响应为 JSON
来源：http://blog.hesvh.cn/Article/details/gqxrqyxth.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/gbzmwsxuj.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/gewyuaujg.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gvmymmbtw.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gxzbiozvx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.hesvh.cn/Article/details/gycxiyqzl.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/glkxjrokk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/grltossbi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gfzrgylug.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gshorwrfu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gxijzrlxr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gcxbtjwww.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gxhkyeksb.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gldffdtzk.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/ghjyidceh.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gxdehkyme.sHtML

Ruby: resp.code.to_i
来源：http://wap.hesvh.cn/Article/details/giqekjwiy.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gmvpcnkhi.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gqqvpughx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gpbfatlwp.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/ghxwqgggm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gdtasrptz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gdchtapmy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/ghibwdfnc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.zdbjq.cn/Article/details/gvldlbnno.sHtML


<!-- 参考信息 -->