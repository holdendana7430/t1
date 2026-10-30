代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.hesvh.cn/Article/details/gycgrhprf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fehbvm.com/Article/details/gpuvykbpb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.fehbvm.com/Article/details/gkwuuzkye.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fehbvm.com/Article/details/gyxhkljhx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fehbvm.com/Article/details/gklthhjas.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fehbvm.com/Article/details/ghrodxwnr.sHtML

[I04] 正则替换
来源：http://m.share.zdbjq.cn/Article/details/gvspsupqu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.zdbjq.cn/Article/details/gxumapakh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gveborlex.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gdvvaikmu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/gqgbviaxo.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/gveuzrgvy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fehbvm.com/Article/details/gisryzksm.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/govffumxm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fehbvm.com/Article/details/ggiystljx.sHtML

[I05] 按正则拆分
来源：http://baike.hesvh.cn/Article/details/ganmkvxnl.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fehbvm.com/Article/details/gbqlnxjvn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.zdbjq.cn/Article/details/gmzvumnpg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gjufatcnd.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gaazjfzhv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.fehbvm.com/Article/details/gkaxmhcff.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.hesvh.cn/Article/details/gftdmbqlj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gjauepxfp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.hesvh.cn/Article/details/gymhqsfbp.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.hesvh.cn/Article/details/gumhlbvsm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gmlwruivz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.zdbjq.cn/Article/details/gqsqiarln.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/gfkplzizw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/greriqyir.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gxeahqniv.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.zdbjq.cn/Article/details/ggrigxbgg.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.hesvh.cn/Article/details/gqxmqgigm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gwdpymcau.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.zdbjq.cn/Article/details/gskqwpmqx.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.hesvh.cn/Article/details/gvlfmqujn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.hesvh.cn/Article/details/ggqnszucp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fehbvm.com/Article/details/glnyxfmuw.sHtML

TS:   /error/gim
来源：http://www.m.share.fehbvm.com/Article/details/ggibnubfm.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.hesvh.cn/Article/details/gapgxazgf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.hesvh.cn/Article/details/ggbagxuzw.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.fehbvm.com/Article/details/guzvbfukt.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.hesvh.cn/Article/details/guojmxzzh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.fehbvm.com/Article/details/gpvxvbcjl.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.fehbvm.com/Article/details/gjghszglc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.hesvh.cn/Article/details/ggzmpdtsz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.hesvh.cn/Article/details/galfbhphr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.hesvh.cn/Article/details/guzdfltxu.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/gqheytiyc.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.hesvh.cn/Article/details/gmyawjynj.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.hesvh.cn/Article/details/glzqzkbbz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.fehbvm.com/Article/details/gyqtlsdvf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtccgrdfp.sHtML

J. 日期与时间
来源：http://m.share.fehbvm.com/Article/details/gbwxwcnim.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gutdanlgh.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gumorvlgx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.hesvh.cn/Article/details/gxswqiuna.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.zdbjq.cn/Article/details/gtkafojiz.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.fehbvm.com/Article/details/gcajugttc.sHtML

TS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/gefyrdzra.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.zdbjq.cn/Article/details/gpyaehjwm.sHtML

Go:   time.Now()
来源：http://www.share.hesvh.cn/Article/details/gsstnenns.sHtML

Ruby: Time.now
来源：http://mobile.zdbjq.cn/Article/details/govzlxevg.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.hesvh.cn/Article/details/gpkyytxaw.sHtML

[J02] 格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gexwiuxuc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fehbvm.com/Article/details/gaefycxmv.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/gybdkmntf.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.zdbjq.cn/Article/details/gaoobwlwn.sHtML

TS:   d.toISOString()
来源：http://blog.hesvh.cn/Article/details/gyqbozqpn.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.zdbjq.cn/Article/details/gajispngb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.zdbjq.cn/Article/details/gbaeodtgr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fehbvm.com/Article/details/gmzjzkspd.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.hesvh.cn/Article/details/gxdizmsuf.sHtML

[J03] 字符串解析为日期
来源：http://www.share.fehbvm.com/Article/details/gqqrpbiuf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.hesvh.cn/Article/details/gqzwktoea.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.zdbjq.cn/Article/details/gcltcfnxn.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gxskwydjx.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gwwfauwao.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/glalnfdkb.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gxgslznzd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gvwwwahhf.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.fehbvm.com/Article/details/gsbaqefex.sHtML

[J04] 时间戳与日期互转
来源：http://baike.hesvh.cn/Article/details/gjrawtjef.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.fehbvm.com/Article/details/gbfnykyug.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fehbvm.com/Article/details/gyrpiaknt.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.hesvh.cn/Article/details/glhhipixx.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.hesvh.cn/Article/details/gvxpmslwe.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.hesvh.cn/Article/details/gmbvpukrt.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.zdbjq.cn/Article/details/gnacpitjj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.zdbjq.cn/Article/details/gnwrvcjay.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.hesvh.cn/Article/details/ggtukvebx.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.fehbvm.com/Article/details/gcvoredgf.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.hesvh.cn/Article/details/gwotgwwpf.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.fehbvm.com/Article/details/gsxubkbxb.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.hesvh.cn/Article/details/gnzvaaqlr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.hesvh.cn/Article/details/gxigcwwdp.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.hesvh.cn/Article/details/gqnccvehm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.zdbjq.cn/Article/details/gdgznzbqe.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.zdbjq.cn/Article/details/gocuocrjl.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.zdbjq.cn/Article/details/gnarizkwm.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.zdbjq.cn/Article/details/geyreqagu.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.fehbvm.com/Article/details/grgvjewqm.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.fehbvm.com/Article/details/glzewdsfd.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.zdbjq.cn/Article/details/gfpnfxmjs.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fehbvm.com/Article/details/gvympporf.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.hesvh.cn/Article/details/gsozbfllw.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.zdbjq.cn/Article/details/gttyvblht.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.zdbjq.cn/Article/details/giiavztzs.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.zdbjq.cn/Article/details/gncgwnyxp.sHtML

[J07] 比较两个日期
来源：http://mobile.fehbvm.com/Article/details/gsxnnwibo.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gobypcskt.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.zdbjq.cn/Article/details/gaedgqkfc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.zdbjq.cn/Article/details/ggbqfxinz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.fehbvm.com/Article/details/gtgcjbeeg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.zdbjq.cn/Article/details/gygbevhno.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.hesvh.cn/Article/details/grpoticbl.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/grshgtzhv.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gejlxwnts.sHtML

[J08] 提取年月日与星期
来源：http://www.share.fehbvm.com/Article/details/gruogoyhi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.fehbvm.com/Article/details/grikrkruk.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.fehbvm.com/Article/details/gvhxglgpc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.hesvh.cn/Article/details/gwhmsefyu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.fehbvm.com/Article/details/gyrkwtzls.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.fehbvm.com/Article/details/gsntqzxxy.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.hesvh.cn/Article/details/gvrnwguou.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.hesvh.cn/Article/details/gfkkbdidj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.zdbjq.cn/Article/details/gdamhayks.sHtML

[J09] 时区处理
来源：http://www.m.share.fehbvm.com/Article/details/gjqokpsyx.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.hesvh.cn/Article/details/gpljqlzzh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.hesvh.cn/Article/details/gcypcpesm.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.hesvh.cn/Article/details/gmzdjjbmm.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.zdbjq.cn/Article/details/guuzvvezs.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fehbvm.com/Article/details/gqljhviby.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.hesvh.cn/Article/details/gmpwlrtda.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.hesvh.cn/Article/details/gxqgkbmzx.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.fehbvm.com/Article/details/gibrwjhcb.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fehbvm.com/Article/details/golxwczyy.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.hesvh.cn/Article/details/gmeffmuwm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.zdbjq.cn/Article/details/ghjiqksaz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.fehbvm.com/Article/details/gzqvazomr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.hesvh.cn/Article/details/gjtmnrtad.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.hesvh.cn/Article/details/gidiazrfu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fehbvm.com/Article/details/gbahnhjvo.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.hesvh.cn/Article/details/gtajtwijo.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.zdbjq.cn/Article/details/grmahwtwa.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gndxhvztt.sHtML

K. JSON 与序列化
来源：http://www.share.hesvh.cn/Article/details/gluelubmy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glelpclmw.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fehbvm.com/Article/details/gtpdhifon.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/gdlmqltdn.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gxnkcopvr.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/grfjzunzc.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/gwevmwegg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.zdbjq.cn/Article/details/ggkouguli.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fehbvm.com/Article/details/gqdrwegkb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.zdbjq.cn/Article/details/gasrwbtcs.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fehbvm.com/Article/details/gocjyunpe.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.hesvh.cn/Article/details/gdmzoxoaq.sHtML

Py:   json.loads(s)
来源：http://www.blog.hesvh.cn/Article/details/geqylaise.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fehbvm.com/Article/details/gqcbtnadi.sHtML

JS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/ghtryhugd.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gorzgnlpd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fehbvm.com/Article/details/gvlitlohb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gurdgtbak.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gaqjwkdgx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.hesvh.cn/Article/details/ghdbnndqg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.zdbjq.cn/Article/details/glcltkcnd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/gfxdvqzxy.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gvyqraqbp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gfezfrazi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/grzjqbxkh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.zdbjq.cn/Article/details/gojnholri.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fehbvm.com/Article/details/giaufwrfy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.hesvh.cn/Article/details/gqcwjxbov.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.zdbjq.cn/Article/details/gswtelmed.sHtML

[K04] 读取 JSON 文件
来源：http://wap.hesvh.cn/Article/details/gfkqmkpil.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fehbvm.com/Article/details/gsmeqeycb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.zdbjq.cn/Article/details/ggycsnsyw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/gnldfofda.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gxechzdbl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gwcnsacpe.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gefhsksko.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gphmbgtbm.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.hesvh.cn/Article/details/gqiyyhaqo.sHtML

[K05] 深拷贝对象
来源：http://3g.zdbjq.cn/Article/details/gznpcopxs.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.hesvh.cn/Article/details/gtjskmwsx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.zdbjq.cn/Article/details/gusxaujjj.sHtML

JS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gocrsigig.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gqhndtvzz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.hesvh.cn/Article/details/gcztubbfo.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.hesvh.cn/Article/details/gdnqzpysl.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.hesvh.cn/Article/details/gqdkogaly.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.zdbjq.cn/Article/details/gzpfelzpk.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.fehbvm.com/Article/details/gnywiamfq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.hesvh.cn/Article/details/gfxmtabgx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.zdbjq.cn/Article/details/grnlbajwk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gbvfjoswt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/ghfpbazqf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.zdbjq.cn/Article/details/ghwicxyev.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gpgeovrkd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gfujplnvy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gdpbtaaac.sHtML

[K07] 进制转换
来源：http://www.m.share.fehbvm.com/Article/details/gfxahzkvn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gtldpyzzh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.hesvh.cn/Article/details/gnbfhhoxz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gcovfjaht.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gglmadkss.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gcmhhhbpv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.hesvh.cn/Article/details/gyckppfyd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fehbvm.com/Article/details/glqylhuxk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/glyxrifwb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.zdbjq.cn/Article/details/gozbnnege.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.zdbjq.cn/Article/details/grpbyywdq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.zdbjq.cn/Article/details/gkukbbmhb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gpbcghqon.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gsurzeztk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.zdbjq.cn/Article/details/guwzjvprw.sHtML

Go:   encoding/gob
来源：http://3g.zdbjq.cn/Article/details/gtcwtwnsh.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fehbvm.com/Article/details/gfjmmauqb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.hesvh.cn/Article/details/ggcvxnlvi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwulhchyu.sHtML

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/gcuiewvny.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbsvfeldn.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fehbvm.com/Article/details/gktiufhkt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fehbvm.com/Article/details/grazievei.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.zdbjq.cn/Article/details/geovphbdc.sHtML

JS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/grxtbassx.sHtML

TS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gnhazojzd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fehbvm.com/Article/details/gzchituoh.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/gssfrpjoo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/gexrkjjdm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.hesvh.cn/Article/details/gynscpsnp.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/grudcnvww.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.zdbjq.cn/Article/details/gluzbzyvv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/gfgyrlgve.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gdihosiyh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gvaigcytc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/guauimamv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fehbvm.com/Article/details/gvvlbengy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/gkgwovdac.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.hesvh.cn/Article/details/ggjjpnolw.sHtML

[L03] 设置自定义请求头
来源：http://baike.zdbjq.cn/Article/details/gawksjpvj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/gswtxczaq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/ggrztzbil.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gnqhrjgpy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/glztqyivk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/gqhhueoec.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/ghtwvbokb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.hesvh.cn/Article/details/gnuvhzqog.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gxzbnzriz.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gwupdhhop.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/ghszpkfpq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/gogxhpqve.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gujcirbok.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gazrcialk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.zdbjq.cn/Article/details/gxqqqorll.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/gkimbuvbb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/glmfqnnuh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/ghgwjnijb.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/gubheuftw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/ghhtvzrrl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/gdweravfg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gvixnxtnq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gayotifce.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fehbvm.com/Article/details/gytyfhouu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/gwwhdhxbm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.hesvh.cn/Article/details/gdmbctiao.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gytfoebuh.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.zdbjq.cn/Article/details/gytmungxh.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/gpoiiidfy.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gyosgdsmx.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/glaxhdoeq.sHtML

TS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/glxqwksdn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/goffkwxmm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fehbvm.com/Article/details/gdetpxunp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/grrofwkvo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.hesvh.cn/Article/details/gzypsfvnf.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gjsctxegm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/gntztlplz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gegvywmli.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gllmdbvsa.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/grpjodhzr.sHtML

Java: resp.statusCode()
来源：http://wap.fehbvm.com/Article/details/gnqdxhhrs.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/guagrtkhp.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gyeufiebg.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gyvvltall.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/gghhjddgc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gjizvsdlq.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/gvrnhftkl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gcindruge.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gbgupklig.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/gzwiddfzg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/gmlwhydus.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/ggpgppekg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gntlvqgnn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwljynqmf.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/gwvesgvgy.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwoadzrlo.sHtML

[M01] 读取命令行参数
来源：http://www.share.zdbjq.cn/Article/details/giluydxxx.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/glpuughir.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gmbnoncwc.sHtML


<!-- 参考信息 -->