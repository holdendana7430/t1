代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.zdbjq.cn/Article/details/gjpitnrlp.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fehbvm.com/Article/details/gnhkxragv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gwrrojrdd.sHtML

[I05] 按正则拆分
来源：http://www.m.share.hesvh.cn/Article/details/gzmrqlzpr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.zdbjq.cn/Article/details/gnbgqsiyb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gayiopdzb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gfahwdrjq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gsszdtxtq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.zdbjq.cn/Article/details/ggewakdlv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.hesvh.cn/Article/details/gbrbnxnav.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gfltyamcs.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.zdbjq.cn/Article/details/gongzofkq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.fehbvm.com/Article/details/grrmhjgpx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/glhngnyyn.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.zdbjq.cn/Article/details/gtzvmksfn.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.zdbjq.cn/Article/details/goubgovfz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.hesvh.cn/Article/details/glsuxsfwn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gwoqkikup.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.hesvh.cn/Article/details/gygvxcxwc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.zdbjq.cn/Article/details/glryzzpgk.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gbktzqxbc.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.zdbjq.cn/Article/details/gbdsxvhlk.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.fehbvm.com/Article/details/gsakjgwzi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.hesvh.cn/Article/details/ghtqkdajg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.fehbvm.com/Article/details/gmhymrnja.sHtML

TS:   /error/gim
来源：http://www.m.share.fehbvm.com/Article/details/gbzodlisr.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.fehbvm.com/Article/details/gsdkgnpxp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fehbvm.com/Article/details/gijqjfvbh.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.hesvh.cn/Article/details/gukcflunc.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.zdbjq.cn/Article/details/gksnnxegz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.hesvh.cn/Article/details/ghrwftmik.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.fehbvm.com/Article/details/gsgsrwiyc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.fehbvm.com/Article/details/gjfbxxywj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.hesvh.cn/Article/details/gjrbqwvqa.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fehbvm.com/Article/details/gtymnbzjg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/gxkxccabv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.zdbjq.cn/Article/details/gmqofmedo.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.fehbvm.com/Article/details/gzzkwftka.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.fehbvm.com/Article/details/ghbqfnrxh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/goqtprcwz.sHtML

J. 日期与时间
来源：http://3g.fehbvm.com/Article/details/gsvtomive.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxhhshdwn.sHtML

[J01] 获取当前时间
来源：http://www.share.hesvh.cn/Article/details/gllelcnmo.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.fehbvm.com/Article/details/geqjmnuxw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.hesvh.cn/Article/details/ghhtoxgfg.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/gfhjmequx.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.fehbvm.com/Article/details/gopyugxlu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.fehbvm.com/Article/details/gnuodhnyf.sHtML

Go:   time.Now()
来源：http://www.blog.fehbvm.com/Article/details/glbpxlksk.sHtML

Ruby: Time.now
来源：http://wap.zdbjq.cn/Article/details/gxsguzfjo.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.fehbvm.com/Article/details/gwtdtnsnj.sHtML

[J02] 格式化输出
来源：http://baike.zdbjq.cn/Article/details/gzvtcvmoo.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.zdbjq.cn/Article/details/guhxvnkuf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.fehbvm.com/Article/details/gmdgjreva.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.zdbjq.cn/Article/details/ghtkpjodu.sHtML

TS:   d.toISOString()
来源：http://3g.hesvh.cn/Article/details/gwukjxgsc.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.zdbjq.cn/Article/details/gtuphzlna.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.zdbjq.cn/Article/details/geunfferr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fehbvm.com/Article/details/gyrmzvzph.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fehbvm.com/Article/details/gthvqbrcy.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.hesvh.cn/Article/details/gchidblsi.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.hesvh.cn/Article/details/gtnapemum.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.fehbvm.com/Article/details/gwoxzelht.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gfwazlpll.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/ghthtzzgy.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gnugaaywy.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/garxmwosm.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gtrtudtcr.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.zdbjq.cn/Article/details/gdyjaavzt.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.fehbvm.com/Article/details/gsgwpkgxo.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.fehbvm.com/Article/details/gyoctvvlw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.zdbjq.cn/Article/details/gqlgqlzyh.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.hesvh.cn/Article/details/gxrksgtor.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.zdbjq.cn/Article/details/gxpffalxj.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.hesvh.cn/Article/details/gthncalsj.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fehbvm.com/Article/details/gnvthpfxf.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.zdbjq.cn/Article/details/gsbxjpuab.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.zdbjq.cn/Article/details/gkpqwwrlo.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.fehbvm.com/Article/details/gwodvdojv.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.fehbvm.com/Article/details/gryhldqik.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.fehbvm.com/Article/details/gsgzkzypd.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.zdbjq.cn/Article/details/gklntylzc.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fehbvm.com/Article/details/gfebbifkw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/ghcvltgop.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.fehbvm.com/Article/details/gahwklofm.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.fehbvm.com/Article/details/ggkdlcqfj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.zdbjq.cn/Article/details/gmeviczoq.sHtML

[J06] 计算两时间之差
来源：http://blog.zdbjq.cn/Article/details/gqocvcqgn.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.fehbvm.com/Article/details/gsympiujk.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.fehbvm.com/Article/details/gqtyjzyko.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.hesvh.cn/Article/details/grkyanrvq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.zdbjq.cn/Article/details/gofitumvh.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.hesvh.cn/Article/details/gqlksktoj.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.zdbjq.cn/Article/details/gyoqmltwr.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.hesvh.cn/Article/details/gvanvdfwv.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.zdbjq.cn/Article/details/gpqcpuquz.sHtML

[J07] 比较两个日期
来源：http://blog.zdbjq.cn/Article/details/gcxhlpqfm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/grryzifdn.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.fehbvm.com/Article/details/gafzfxscm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.fehbvm.com/Article/details/goimqxafu.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fehbvm.com/Article/details/gpnszcwet.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.zdbjq.cn/Article/details/gavsolnej.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.fehbvm.com/Article/details/grvwqkjck.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gnrcbofpr.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/gurhaxtpg.sHtML

[J08] 提取年月日与星期
来源：http://m.share.hesvh.cn/Article/details/gqcrrwnox.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.zdbjq.cn/Article/details/gyqfybfaf.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.hesvh.cn/Article/details/grzbrmgtv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.hesvh.cn/Article/details/gcfzjkofd.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.fehbvm.com/Article/details/gwudisudw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.fehbvm.com/Article/details/gkranlphh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.zdbjq.cn/Article/details/gacmovach.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.fehbvm.com/Article/details/gmhnznfgy.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.hesvh.cn/Article/details/gcvihdtgo.sHtML

[J09] 时区处理
来源：http://mobile.fehbvm.com/Article/details/gpfhtkofo.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.zdbjq.cn/Article/details/gcabbytbl.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.zdbjq.cn/Article/details/grntofarb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.zdbjq.cn/Article/details/gomvwqhpe.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/gohtyjoxd.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.fehbvm.com/Article/details/gzygebkyd.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.hesvh.cn/Article/details/gshudgfyb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.zdbjq.cn/Article/details/gewkycjxk.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.hesvh.cn/Article/details/gfjbzzfdk.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.hesvh.cn/Article/details/ggfhdwnfm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.fehbvm.com/Article/details/gpdadidiu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fehbvm.com/Article/details/gzbzbeclx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.hesvh.cn/Article/details/gdnjxmudq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/goqwjwwtt.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.hesvh.cn/Article/details/gynjcmhyu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.zdbjq.cn/Article/details/gkouyrvat.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.hesvh.cn/Article/details/gzgdjwojt.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.hesvh.cn/Article/details/gknnzoqms.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gssmazwsy.sHtML

K. JSON 与序列化
来源：http://www.share.fehbvm.com/Article/details/geowsqypd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gubeptamu.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.zdbjq.cn/Article/details/gdfazvvhh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/gyoarklcf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gydjcykkt.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.zdbjq.cn/Article/details/gcibmrkwk.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.zdbjq.cn/Article/details/gzouhsfvb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.hesvh.cn/Article/details/gwhnpaalk.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.hesvh.cn/Article/details/gpahutthw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fehbvm.com/Article/details/gbgbzfylk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fehbvm.com/Article/details/ggqwpulsg.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.hesvh.cn/Article/details/gjjfbnnjt.sHtML

Py:   json.loads(s)
来源：http://read.share.hesvh.cn/Article/details/gmanvcbcf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.zdbjq.cn/Article/details/gwbkqrcob.sHtML

JS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gahojrlvo.sHtML

TS:   JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gljgkjfrw.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fehbvm.com/Article/details/gqmbdcfqa.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.zdbjq.cn/Article/details/gfadjdzwp.sHtML

Ruby: JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gigwmspua.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fehbvm.com/Article/details/gohntekuq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.hesvh.cn/Article/details/goxglrkhk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/gkubmiypx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/gduwgcqgr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gntjyrvwi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gkxmkjknx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.hesvh.cn/Article/details/gxmslutul.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.hesvh.cn/Article/details/gwkonchvs.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.hesvh.cn/Article/details/gurbyeblb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.zdbjq.cn/Article/details/ghntvytsv.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fehbvm.com/Article/details/gxafmtqmr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fehbvm.com/Article/details/gypmfjqrd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.zdbjq.cn/Article/details/ggwscvvdq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gkiebmkil.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/gtayukbty.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gkrmdwmue.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.zdbjq.cn/Article/details/gguejdwaj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/ggromzatw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fehbvm.com/Article/details/ghyyjfpxo.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/ghxzzhpom.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.zdbjq.cn/Article/details/gsxefytix.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.zdbjq.cn/Article/details/gwyqgluuq.sHtML

JS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gasizoyun.sHtML

TS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gpxnccaay.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fehbvm.com/Article/details/gluzkevip.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.zdbjq.cn/Article/details/gwoxerpeq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fehbvm.com/Article/details/gvqvfebqq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.hesvh.cn/Article/details/gsughtrbk.sHtML

[K06] 解析 URL 查询串
来源：http://wap.zdbjq.cn/Article/details/gxewfvtnw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gvkdekyte.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fehbvm.com/Article/details/gxsfntzyb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gvbsuxnpx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gawrsigaa.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.hesvh.cn/Article/details/gscozvbdp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gaeegumqh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/glrewtrgl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gkffjvvgb.sHtML

[K07] 进制转换
来源：http://www.m.share.hesvh.cn/Article/details/gbsipivzr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gqkspidue.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.zdbjq.cn/Article/details/gypqdxxce.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/giwrarobu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gjcgnwixa.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gkodpxmds.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/gjguonapp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.zdbjq.cn/Article/details/gjcybczir.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gnlcyykcf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.hesvh.cn/Article/details/gcabcdkqf.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gafprxzgx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/gbnhtobyi.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gjesgjkdx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gxawimrys.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/gytljufnc.sHtML

Go:   encoding/gob
来源：http://read.share.hesvh.cn/Article/details/gebrqwonv.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.hesvh.cn/Article/details/gswcnlfwn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gflaqgmxt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gktiwobiu.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/gfuccuovf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbeixmvmb.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/ggapiyyqh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.hesvh.cn/Article/details/gguufrnuq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/ggwldgknp.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gqtzewjdq.sHtML

TS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gnypezrjz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.zdbjq.cn/Article/details/glbajvmzy.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fehbvm.com/Article/details/gmfxixfym.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fehbvm.com/Article/details/gcpvbkcxm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/gwayoxwsz.sHtML

[L02] 发送 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gfptrwcoc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fehbvm.com/Article/details/gmugiiwtq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/gvwxbbsqs.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gkwaeagua.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/glncqtgli.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fehbvm.com/Article/details/gsbyvmbse.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.hesvh.cn/Article/details/gxtvfmkxg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fehbvm.com/Article/details/gkgpfbpub.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.hesvh.cn/Article/details/ghcnaxqdq.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/gofzytvmc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.hesvh.cn/Article/details/gteuzcrxl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.zdbjq.cn/Article/details/gfdipmqjl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gqllfxxcg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gkdtzphhw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.hesvh.cn/Article/details/gemqzvkkd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gmnnrziri.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/gderjfqfp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/glxrozfne.sHtML

[L04] 设置超时
来源：http://read.share.hesvh.cn/Article/details/gazfdzxwp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/gzchclyev.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/gqjgzregz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/goncqsfkv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gbftlqeil.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.hesvh.cn/Article/details/gcsitbarg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/gxyanudkh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/gecwfgrlw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fehbvm.com/Article/details/genuezxzo.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/ghgfvwluz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.zdbjq.cn/Article/details/ghunpaknn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/gzopduyct.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/giafgnczg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gbkecqdam.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/grsopianv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.hesvh.cn/Article/details/gdmtyyqmx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.zdbjq.cn/Article/details/gpdrdjrkz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gzpkretyr.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.zdbjq.cn/Article/details/gwtyctwvs.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gsfmmqonk.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/gonucgpzx.sHtML

JS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gadhyfgnd.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/ghqpnhgiw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gjhnspkck.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.zdbjq.cn/Article/details/gdrdxnghv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/gxbkdyvmp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gfsaxmwab.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gdivtaeah.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/gztmiqraq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fehbvm.com/Article/details/gdoleqqhu.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gbexznfpk.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gmayptwxo.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/gflzhmvow.sHtML

Go:   resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gnjbxujen.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/gzuiipzgg.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gvuhjyjrk.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.hesvh.cn/Article/details/gcznkiwjg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/gkwwlfhay.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/gmyizhusi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gnqkhpyhs.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gdhinxyft.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gzvrrswzu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/gpenuqtag.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/gwphujrlx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fehbvm.com/Article/details/grziwzeie.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grfynymnt.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/gfbqnjkuu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbkqblfmf.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gpsleumhb.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/gyerudkel.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/gwtpboxrb.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gjsaupvty.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/guiwbmxtm.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gqjpstvoh.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/gtehtrfms.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/gfrhaeycn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gxszdpnyh.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/ggcbuyljr.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/genumxipi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gduznlxdo.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/guoumjwlc.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gluacgnxy.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gumplzqnd.sHtML


<!-- 参考信息 -->