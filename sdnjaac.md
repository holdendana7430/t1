代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fanxiaobao.xyz/Article/details/gfjszlsjv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fanxiaobao.xyz/Article/details/grglczpbq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giavihntx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fanxiaobao.xyz/Article/details/gggecjyko.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gwchjmobx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fanxiaobao.xyz/Article/details/gntviiouh.sHtML

[I04] 正则替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmqfbxpl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtoyjcrj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpxmxgxb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.fanxiaobao.xyz/Article/details/gtifjbyma.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.fanxiaobao.xyz/Article/details/gkerpaxdd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.fanxiaobao.xyz/Article/details/gmsyywmrd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzmhxhlf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/gapnbhmnp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.fanxiaobao.xyz/Article/details/gayryzcmx.sHtML

[I05] 按正则拆分
来源：http://mobile.fanxiaobao.xyz/Article/details/gytziwlcd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauglqufj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gnnqslfvb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.fanxiaobao.xyz/Article/details/guryzwcop.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gojflrivh.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfptnqqoo.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmdnwxgb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwsfzhhy.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.fanxiaobao.xyz/Article/details/gsmtiyonc.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fanxiaobao.xyz/Article/details/gdlilvlol.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjszqhktg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.fanxiaobao.xyz/Article/details/gfkycitjv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbtdwtqr.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fanxiaobao.xyz/Article/details/gzpfviwsa.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtchfzvgi.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtiwixkd.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.fanxiaobao.xyz/Article/details/gcvcmcbay.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.fanxiaobao.xyz/Article/details/gpdzdsusq.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.fanxiaobao.xyz/Article/details/gmrfquqwb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.fanxiaobao.xyz/Article/details/gshwehzfp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfkfppci.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.fanxiaobao.xyz/Article/details/glgjspjwk.sHtML

TS:   /error/gim
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgwbsblq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsfeustt.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.fanxiaobao.xyz/Article/details/gldongjhv.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fanxiaobao.xyz/Article/details/gqyxzzkim.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.fanxiaobao.xyz/Article/details/grzjvjkes.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gamidehhw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.fanxiaobao.xyz/Article/details/gzoywibpz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.fanxiaobao.xyz/Article/details/gjuxnfbcv.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjetkkscj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmtatzve.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.fanxiaobao.xyz/Article/details/gixqtqgaw.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsckayec.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.fanxiaobao.xyz/Article/details/gipdibusk.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.fanxiaobao.xyz/Article/details/gjpwmcceq.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyylztmzb.sHtML

J. 日期与时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuizorll.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhzothfu.sHtML

[J01] 获取当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqmcgzmo.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.fanxiaobao.xyz/Article/details/gqftfrzzi.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.fanxiaobao.xyz/Article/details/ggreqrfsj.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwmirfvx.sHtML

TS:   new Date();  Date.now()
来源：http://baike.fanxiaobao.xyz/Article/details/gyfjbjeph.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhuuoald.sHtML

Go:   time.Now()
来源：http://baike.fanxiaobao.xyz/Article/details/glbdtpyux.sHtML

Ruby: Time.now
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwujgcxnt.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.fanxiaobao.xyz/Article/details/grbnhlczj.sHtML

[J02] 格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgpaziji.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fanxiaobao.xyz/Article/details/gwodpmzmx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.fanxiaobao.xyz/Article/details/gtznnpabv.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvzafkxi.sHtML

TS:   d.toISOString()
来源：http://read.share.fanxiaobao.xyz/Article/details/givscwkww.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvwhfbof.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.fanxiaobao.xyz/Article/details/guvkoggrl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmamxfrkr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.fanxiaobao.xyz/Article/details/gucboansv.sHtML

[J03] 字符串解析为日期
来源：http://wap.fanxiaobao.xyz/Article/details/gbxxjgndm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.fanxiaobao.xyz/Article/details/gmglwlokz.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.fanxiaobao.xyz/Article/details/grsjoneqt.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.fanxiaobao.xyz/Article/details/gfmvozooa.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghimqfops.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/gqdxeputs.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiebqrye.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fanxiaobao.xyz/Article/details/gacionbjb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.fanxiaobao.xyz/Article/details/ggeeqzyyz.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fanxiaobao.xyz/Article/details/gcibyfoyp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.fanxiaobao.xyz/Article/details/grqmtjlov.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.fanxiaobao.xyz/Article/details/gwobwrotq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.fanxiaobao.xyz/Article/details/gljsrasxg.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvtyqxhw.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.fanxiaobao.xyz/Article/details/greyarcmm.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gffnmtlbp.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxuxoywc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.fanxiaobao.xyz/Article/details/gpbjxcinx.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.fanxiaobao.xyz/Article/details/gzlyqorms.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrbzvfgf.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fanxiaobao.xyz/Article/details/gukqvmcqx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fanxiaobao.xyz/Article/details/gimhtmwol.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fanxiaobao.xyz/Article/details/gynhrhtbs.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.fanxiaobao.xyz/Article/details/grqiqbrqe.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.fanxiaobao.xyz/Article/details/ghowuyjbk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.fanxiaobao.xyz/Article/details/ggnxxwijr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.fanxiaobao.xyz/Article/details/gittprygz.sHtML

[J06] 计算两时间之差
来源：http://www.share.fanxiaobao.xyz/Article/details/gytglzrdv.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyejbvwav.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fanxiaobao.xyz/Article/details/goqxduysg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrhsayka.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdlhymbl.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdwbxues.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fanxiaobao.xyz/Article/details/gfeewzmjh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.fanxiaobao.xyz/Article/details/gfyyccjcb.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnpdbcyu.sHtML

[J07] 比较两个日期
来源：http://baike.fanxiaobao.xyz/Article/details/gqeiwoucs.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.fanxiaobao.xyz/Article/details/gggevntan.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.fanxiaobao.xyz/Article/details/gqirmtzce.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqoutcyb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.fanxiaobao.xyz/Article/details/gulqzfkvt.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsszqaqrm.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvrtgksu.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.fanxiaobao.xyz/Article/details/gssxwqjsi.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.fanxiaobao.xyz/Article/details/gyomeopyt.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyeolymxe.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fanxiaobao.xyz/Article/details/gloimtdxl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.fanxiaobao.xyz/Article/details/gayovldkr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.fanxiaobao.xyz/Article/details/gymajoqsy.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpepvcko.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fanxiaobao.xyz/Article/details/gskinfwwr.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwxqylhf.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.fanxiaobao.xyz/Article/details/gdqdrvrhs.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpiervql.sHtML

[J09] 时区处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gptpgnayj.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.fanxiaobao.xyz/Article/details/gbvqbcrsw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlwcazrh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fanxiaobao.xyz/Article/details/grziykydb.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhwymfrv.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.fanxiaobao.xyz/Article/details/gnpyopmwu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fanxiaobao.xyz/Article/details/gloulksdj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.fanxiaobao.xyz/Article/details/glzcigmcj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fanxiaobao.xyz/Article/details/ghiipuwnm.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrgrhaap.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gazzzqpmv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidkmuejh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gaxsrgzjm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gqqpaorqx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gbyrbaksv.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktvrjjbp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlpjizpf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhncxqmy.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gcotddxch.sHtML

K. JSON 与序列化
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyhpsyqq.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlpkjwxc.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphmwvacs.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqzfuglq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxtgdtje.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyatemzae.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gmixurnzw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fanxiaobao.xyz/Article/details/gokbedtpf.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gppdzmgju.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fanxiaobao.xyz/Article/details/gtckfwogh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcymnpjmd.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glowctfqr.sHtML

Py:   json.loads(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxqjmnjy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gyosakrfi.sHtML

JS:   JSON.parse(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gfyprrtcs.sHtML

TS:   JSON.parse(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gkejqmfzf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.fanxiaobao.xyz/Article/details/gckruxeoe.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fanxiaobao.xyz/Article/details/gzpbmppfv.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqkajpir.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gewjdkhhv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxwcohih.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyspzbre.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fanxiaobao.xyz/Article/details/gojoymjll.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gntvkqmva.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/ggmpyzbxz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gnmqvvmcv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.fanxiaobao.xyz/Article/details/ghupjgjoq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gnglykpow.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fanxiaobao.xyz/Article/details/goyiyldxp.sHtML

[K04] 读取 JSON 文件
来源：http://wap.fanxiaobao.xyz/Article/details/gggnzargp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.fanxiaobao.xyz/Article/details/gwawoiqva.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtusnecqt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrgfnbnz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gkacrdgxt.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlyxsllx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.fanxiaobao.xyz/Article/details/gfbbpwvav.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fanxiaobao.xyz/Article/details/gtrtgfsjb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fanxiaobao.xyz/Article/details/gdnlqqalm.sHtML

[K05] 深拷贝对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gamrzkykz.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/ghzduqatz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fanxiaobao.xyz/Article/details/gxeoopkod.sHtML

JS:   structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gokzamwak.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmyneymg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwupjfah.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpsngsye.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/gpabahxyk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fanxiaobao.xyz/Article/details/gqlhuiegf.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fanxiaobao.xyz/Article/details/gbgnnlqcu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fanxiaobao.xyz/Article/details/gpfjkplge.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnosbzub.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fanxiaobao.xyz/Article/details/gatrnbijq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrwsnssk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fanxiaobao.xyz/Article/details/gkjcvtqoe.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqizldfs.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylcojpzs.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fanxiaobao.xyz/Article/details/glszwhldf.sHtML

[K07] 进制转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksixjxuy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gwcjwzjji.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezevmwtm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyrqpbzl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/grdryldik.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gghecwgui.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcahvymag.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.fanxiaobao.xyz/Article/details/gewzuxmzz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gfijptdqo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkgpevph.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/grxjxkhib.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlgaubzm.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpobmvsgq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfrtspvw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fanxiaobao.xyz/Article/details/gbhhpbocv.sHtML

Go:   encoding/gob
来源：http://www.blog.fanxiaobao.xyz/Article/details/glesyuyif.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnegxoju.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fanxiaobao.xyz/Article/details/gzqiwrvap.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gjspubehp.sHtML

L. 网络请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gatgelsym.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/galxwjdgu.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gljuddhrs.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fanxiaobao.xyz/Article/details/gevbvpulg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fanxiaobao.xyz/Article/details/gugmquebc.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsssagfb.sHtML

TS:   await fetch(url)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhyfwzxa.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fanxiaobao.xyz/Article/details/gmszakedu.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnrgyqqf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fanxiaobao.xyz/Article/details/gqoobzhdp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fanxiaobao.xyz/Article/details/gjgndspqx.sHtML

[L02] 发送 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/glrbasqoo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxupmhlu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotzadtfu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fanxiaobao.xyz/Article/details/gtiklqbgb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fanxiaobao.xyz/Article/details/gbkwnracw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvioinkzs.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fanxiaobao.xyz/Article/details/ggugfuqpz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwmuihrx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflsqlfgv.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoiwvgah.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkcvirui.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gvedkifzy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fanxiaobao.xyz/Article/details/grsziccwx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvfvghry.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrifnrzk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjcgnskw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyyegxae.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fanxiaobao.xyz/Article/details/gztewdrtj.sHtML

[L04] 设置超时
来源：http://baike.fanxiaobao.xyz/Article/details/ghxdlmreu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsitvunqw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnttehcij.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzuqqwar.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixeybucj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fanxiaobao.xyz/Article/details/guccsbdow.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fanxiaobao.xyz/Article/details/gvvinxfsw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlztyrzh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/goekmyvyn.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fanxiaobao.xyz/Article/details/gdlohceey.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfeyxyivn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmivcdwvm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fanxiaobao.xyz/Article/details/gisbgiokz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxiupahku.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fanxiaobao.xyz/Article/details/gbfptvmzw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fanxiaobao.xyz/Article/details/grhrldqgh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fanxiaobao.xyz/Article/details/grhnpeohy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/grtgqxafq.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxhqlydg.sHtML

Py:   resp.json()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpshewsyx.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbyvaxgl.sHtML

JS:   await resp.json()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjtmmhdo.sHtML

TS:   await resp.json()
来源：http://blog.fanxiaobao.xyz/Article/details/gkyvjidkb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfzjennp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fanxiaobao.xyz/Article/details/glmdqktfa.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fanxiaobao.xyz/Article/details/gutdyhgip.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fanxiaobao.xyz/Article/details/gopyvkkyo.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gdfqdpwxt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fanxiaobao.xyz/Article/details/gccxyrhsg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcchkswrm.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fanxiaobao.xyz/Article/details/ghiqdzolg.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbtviujb.sHtML

Java: resp.statusCode()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwzphksu.sHtML

Go:   resp.StatusCode
来源：http://wap.fanxiaobao.xyz/Article/details/gygwxzavq.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fanxiaobao.xyz/Article/details/gouscnhgz.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fanxiaobao.xyz/Article/details/glhzoyzzc.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fanxiaobao.xyz/Article/details/gupsfozqu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fanxiaobao.xyz/Article/details/gnahhgbph.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhkfnpxu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gdvebbuol.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbzldmnn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fanxiaobao.xyz/Article/details/gdudopshw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqichjfwj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fanxiaobao.xyz/Article/details/gbardtfzk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gozjobdno.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gwdybhqmg.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/giosuikeg.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspahnxwc.sHtML

[M01] 读取命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gvdrfdvzx.sHtML

Py:   sys.argv[1:]
来源：http://baike.fanxiaobao.xyz/Article/details/ggtxslscd.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlfdplqd.sHtML


<!-- 参考信息 -->