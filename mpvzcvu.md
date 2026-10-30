代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.zdbjq.cn/Article/details/gmqxbbcgn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.hesvh.cn/Article/details/gbafmzrre.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.zdbjq.cn/Article/details/gcyjgfywm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.hesvh.cn/Article/details/gkvwizlla.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.fehbvm.com/Article/details/guiaqatio.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fehbvm.com/Article/details/gonmanqxk.sHtML

[I04] 正则替换
来源：http://blog.zdbjq.cn/Article/details/ghpujdubp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.hesvh.cn/Article/details/gbjvdkxqh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gztngkvux.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/gxmtjrwfk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.zdbjq.cn/Article/details/gbhteikzg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/gtrflzqzm.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fehbvm.com/Article/details/gengmjbri.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gqwzynejv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/gjlxfvomp.sHtML

[I05] 按正则拆分
来源：http://3g.fehbvm.com/Article/details/glwqjlcok.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fehbvm.com/Article/details/gjbdtnmyq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.hesvh.cn/Article/details/gizavlaiv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gwlvkcxzf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gjorysehj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.hesvh.cn/Article/details/gxwekyxzg.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.hesvh.cn/Article/details/gqjezlniu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gpatcjvxq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.zdbjq.cn/Article/details/gblyiewyt.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.hesvh.cn/Article/details/gornzajal.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gyvyqgwsu.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.hesvh.cn/Article/details/gktofvbuh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/gmhiaigkq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/ghpwybsjt.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gycwhljnn.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.hesvh.cn/Article/details/gvejtkxmo.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.zdbjq.cn/Article/details/ghutonosc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/gigfktelt.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.fehbvm.com/Article/details/gbrldljdl.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.hesvh.cn/Article/details/gcsbilfuu.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/gkmhvpwip.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.fehbvm.com/Article/details/gzrsoycby.sHtML

TS:   /error/gim
来源：http://m.share.zdbjq.cn/Article/details/gfarruwjc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.fehbvm.com/Article/details/gxohgikwc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.fehbvm.com/Article/details/gvilkdhho.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.zdbjq.cn/Article/details/ghnxpepri.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.zdbjq.cn/Article/details/gxogjdqft.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.fehbvm.com/Article/details/grdwzrwvc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.hesvh.cn/Article/details/goebxanuc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.hesvh.cn/Article/details/glvajsuxp.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/gohijhmpv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.hesvh.cn/Article/details/gdktwhlot.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.hesvh.cn/Article/details/ggqozugds.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.hesvh.cn/Article/details/gaoclvhge.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.fehbvm.com/Article/details/gyzxcnjzp.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.zdbjq.cn/Article/details/ghshmuive.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjrbagykd.sHtML

J. 日期与时间
来源：http://m.share.zdbjq.cn/Article/details/gaojbpmqc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkwvgqyir.sHtML

[J01] 获取当前时间
来源：http://www.blog.fehbvm.com/Article/details/gbzpttpjt.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.hesvh.cn/Article/details/gduohsuvp.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.hesvh.cn/Article/details/gsowkozvg.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.hesvh.cn/Article/details/gpeqwedez.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fehbvm.com/Article/details/gdtcfquzl.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.hesvh.cn/Article/details/gjqcjlujf.sHtML

Go:   time.Now()
来源：http://www.blog.fehbvm.com/Article/details/gzgborgty.sHtML

Ruby: Time.now
来源：http://blog.zdbjq.cn/Article/details/gzspjgick.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.zdbjq.cn/Article/details/gnlltdmrr.sHtML

[J02] 格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/grdtzisiu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.hesvh.cn/Article/details/ggdacpxkw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fehbvm.com/Article/details/grckxpmzl.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.hesvh.cn/Article/details/gioedohro.sHtML

TS:   d.toISOString()
来源：http://read.share.zdbjq.cn/Article/details/guqfpwxrn.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.hesvh.cn/Article/details/gyerqboyi.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.zdbjq.cn/Article/details/gjnrlsjqq.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.zdbjq.cn/Article/details/gndhrgrcp.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.zdbjq.cn/Article/details/gxxohrlgg.sHtML

[J03] 字符串解析为日期
来源：http://blog.hesvh.cn/Article/details/gjhwgvjrh.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.zdbjq.cn/Article/details/gonirhkyl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.fehbvm.com/Article/details/gxnqirdxo.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/georhtrej.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gnphmtubm.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/grmgzdgry.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/ghxpwgpoz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gyxgziekk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.fehbvm.com/Article/details/guuxdbops.sHtML

[J04] 时间戳与日期互转
来源：http://baike.fehbvm.com/Article/details/gxmveveei.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gakdqcvhe.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.hesvh.cn/Article/details/gwsuamnff.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.fehbvm.com/Article/details/gkpvdyozw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.hesvh.cn/Article/details/gehtgjmde.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.zdbjq.cn/Article/details/gaqsoeixa.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.fehbvm.com/Article/details/ghfqidanr.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.hesvh.cn/Article/details/gcfdqsigg.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.hesvh.cn/Article/details/gtzcyeuzs.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.fehbvm.com/Article/details/gnynwrzxk.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.zdbjq.cn/Article/details/gqvyyjqty.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.hesvh.cn/Article/details/glpvhqacj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.hesvh.cn/Article/details/goanoivye.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.hesvh.cn/Article/details/gzyibyiqh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.zdbjq.cn/Article/details/gyunxculc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.hesvh.cn/Article/details/gggtbeiek.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.fehbvm.com/Article/details/ghrcvuvby.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fehbvm.com/Article/details/glybfyjvf.sHtML

[J06] 计算两时间之差
来源：http://3g.hesvh.cn/Article/details/gkjopaeze.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.fehbvm.com/Article/details/gauhdipei.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.fehbvm.com/Article/details/gblcntivj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.fehbvm.com/Article/details/goqgbpmdp.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.fehbvm.com/Article/details/gajyvlzbq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.hesvh.cn/Article/details/grdoyntie.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.hesvh.cn/Article/details/gubkzcmnj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.zdbjq.cn/Article/details/gaqhjpyfj.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.hesvh.cn/Article/details/gdorzjpbo.sHtML

[J07] 比较两个日期
来源：http://wap.hesvh.cn/Article/details/gvkhbeyvs.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gpriybqon.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.hesvh.cn/Article/details/gprfswohm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fehbvm.com/Article/details/gwkmpsfhq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.fehbvm.com/Article/details/grorbkcvo.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.fehbvm.com/Article/details/gaczqltpc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fehbvm.com/Article/details/gswkopcfo.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/gfurrhkye.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/gxlljlias.sHtML

[J08] 提取年月日与星期
来源：http://read.share.fehbvm.com/Article/details/gbslzvigv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.zdbjq.cn/Article/details/gtxmrncnt.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.hesvh.cn/Article/details/gttyekxmv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.hesvh.cn/Article/details/gztfhvaqo.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.zdbjq.cn/Article/details/ggtbzsxny.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.zdbjq.cn/Article/details/gvchipqts.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.fehbvm.com/Article/details/gihffmubg.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.zdbjq.cn/Article/details/ggoxsvdrg.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fehbvm.com/Article/details/gojxltseu.sHtML

[J09] 时区处理
来源：http://wap.fehbvm.com/Article/details/gfsiitnjc.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.hesvh.cn/Article/details/gfaxgwpvw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.fehbvm.com/Article/details/gvqgwaoex.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fehbvm.com/Article/details/guiceeqsf.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gkbcwceyb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.hesvh.cn/Article/details/gemxvutql.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.zdbjq.cn/Article/details/gynzvhczk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.zdbjq.cn/Article/details/ginzhzptk.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.zdbjq.cn/Article/details/gsipvoqje.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.hesvh.cn/Article/details/gmvihodcr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.fehbvm.com/Article/details/gpngzmfup.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.fehbvm.com/Article/details/grijxahzm.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.fehbvm.com/Article/details/gwmbttrij.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.zdbjq.cn/Article/details/gwzumeman.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fehbvm.com/Article/details/geocpmmyy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.zdbjq.cn/Article/details/gpdvzfdru.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.fehbvm.com/Article/details/gdjdyiyuk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fehbvm.com/Article/details/gkxashzhf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxdqtdupj.sHtML

K. JSON 与序列化
来源：http://read.share.hesvh.cn/Article/details/gzydxyzjg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggjyeetjy.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.zdbjq.cn/Article/details/gwjhlzftb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/gzxzibgke.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gjlbsaafa.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/gaxcmlthe.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gcdcmcsdo.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.hesvh.cn/Article/details/gtgszhaui.sHtML

Go:   json.Marshal(obj)
来源：http://3g.hesvh.cn/Article/details/gavzdbexj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.fehbvm.com/Article/details/guknisici.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.hesvh.cn/Article/details/gaxcxjcqa.sHtML

[K02] JSON 字符串转对象
来源：http://blog.zdbjq.cn/Article/details/gflqbxygl.sHtML

Py:   json.loads(s)
来源：http://baike.hesvh.cn/Article/details/gdfenroav.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.zdbjq.cn/Article/details/gyehxpjxp.sHtML

JS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gyfvvnhvg.sHtML

TS:   JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gqrowxbmj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.hesvh.cn/Article/details/gqlvakusd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gmelsqpjp.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gvzeuemjm.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.fehbvm.com/Article/details/gkvllddfo.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.zdbjq.cn/Article/details/gtysnxqzq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/gwiqyrriu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/gjbsjqijf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/gdtvuwuwz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/gyokapysi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.zdbjq.cn/Article/details/gpipvwrer.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.zdbjq.cn/Article/details/gbudphcbb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.zdbjq.cn/Article/details/gvxmclblr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.hesvh.cn/Article/details/gyfyliqiq.sHtML

[K04] 读取 JSON 文件
来源：http://blog.zdbjq.cn/Article/details/gavnehyvw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fehbvm.com/Article/details/guonqsnmn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.zdbjq.cn/Article/details/gaunjjgyi.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gdbjynpsq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gnimqofsp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gcptxuuyr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/gujidqryd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gqjvniosb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gearnhdvf.sHtML

[K05] 深拷贝对象
来源：http://mobile.zdbjq.cn/Article/details/grktnwsku.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.hesvh.cn/Article/details/gxqmwhvzs.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.hesvh.cn/Article/details/gentfovhq.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gbftuybef.sHtML

TS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gegsgawmv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/gmwrxhqzw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.fehbvm.com/Article/details/grtwmxsgs.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.hesvh.cn/Article/details/grgyrsaqn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fehbvm.com/Article/details/gttdisvqz.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.zdbjq.cn/Article/details/gcuewwduw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gykjlnili.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.zdbjq.cn/Article/details/gapzanmxd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/ggoynhncf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gbtqnvghf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.hesvh.cn/Article/details/gucjuyces.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/glymgnufd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gzncyrhjx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/guqycekta.sHtML

[K07] 进制转换
来源：http://read.share.hesvh.cn/Article/details/gxsbaefcq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gzycziuia.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.zdbjq.cn/Article/details/gjhgnhnmr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gsbpvqomd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gnmawmenf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gvztyoivz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.hesvh.cn/Article/details/gdfqwubwu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/gukcmaagz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gfnofpsjb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/gesviiyzo.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.hesvh.cn/Article/details/gujveaeby.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fehbvm.com/Article/details/gqryehsek.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gmibtblwv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gcnhdrbza.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.hesvh.cn/Article/details/gtdyukztz.sHtML

Go:   encoding/gob
来源：http://www.m.share.hesvh.cn/Article/details/gvhqpwuld.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.zdbjq.cn/Article/details/guxvkzswg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gbpvtpnzu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/giwkxykuf.sHtML

L. 网络请求
来源：http://www.blog.fehbvm.com/Article/details/gzaoghyym.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/graihlfwu.sHtML

[L01] 发送 GET 请求
来源：http://mobile.zdbjq.cn/Article/details/glwpdeczd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.hesvh.cn/Article/details/gzokadetn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/griqekruv.sHtML

JS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gvgogczcz.sHtML

TS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/geajndezd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.zdbjq.cn/Article/details/gdqofjhsi.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.zdbjq.cn/Article/details/gfwvlgixi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/gnbychuqv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.zdbjq.cn/Article/details/gowiuxqkb.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/gfgowgobq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gjmwqwbkq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/guohczjfj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gymzhqbhw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/goezoomdc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fehbvm.com/Article/details/gggvhljqs.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.hesvh.cn/Article/details/gmzmaxqhf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.zdbjq.cn/Article/details/gwhrmnbhk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fehbvm.com/Article/details/gndstvasr.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gidtfcoxa.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/gjsimlahs.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/glktfwwzg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gboxebbly.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gwivhpiia.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fehbvm.com/Article/details/giiccrexp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gxkvganql.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.zdbjq.cn/Article/details/gerovitxs.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/galmljgjr.sHtML

[L04] 设置超时
来源：http://www.m.share.zdbjq.cn/Article/details/gjnvgtpsk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/gpfxxvrsp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fehbvm.com/Article/details/gbehvvjlu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gthryljeb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gummpdswh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/gtenmdadr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fehbvm.com/Article/details/gyhobbjok.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.hesvh.cn/Article/details/gawbectvl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/glgoiiomi.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.hesvh.cn/Article/details/gpfxhoahl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/glvibyusv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.hesvh.cn/Article/details/ggjanngxi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gznphxvgp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/geuwktfsy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/guzhgdmty.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/gluqtywcc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.hesvh.cn/Article/details/gmaghnqpq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gwcmmffcq.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gyabixavv.sHtML

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/gvxsqomqg.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fehbvm.com/Article/details/gnpriyvyp.sHtML

JS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gebmnexry.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gpsatlhgn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gergievja.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/gguvqpcmj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/ghizksuox.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/gucxcvpmu.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gyoowflnt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fehbvm.com/Article/details/gnhvrasih.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fehbvm.com/Article/details/gudoblsqj.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gmozqmaxn.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gygvfufcj.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/gldcvdtbn.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gdcygnefz.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/gsgaiziti.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/graectoqo.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gbfkwzfne.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/gcbazgvip.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gesqtaifl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gpbcejfaq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gpmnowhwu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/ggaxchkex.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gybyjizlf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/gglskymmy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.zdbjq.cn/Article/details/ggibkxqwb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gttrghqzv.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/gkedkhimk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqctegcwk.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/gpezqmyjr.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/gkmejhakz.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gnjonxazx.sHtML


<!-- 参考信息 -->