代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.zdbjq.cn/Article/details/gkczyiwcc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.zdbjq.cn/Article/details/glzileydc.sHtML

[I04] 正则替换
来源：http://www.share.fehbvm.com/Article/details/gwykgzpoh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.zdbjq.cn/Article/details/groczukjy.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/gxivgemex.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.fehbvm.com/Article/details/gyahbqwze.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/gsdkjnbnm.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.hesvh.cn/Article/details/giuygyztv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.fehbvm.com/Article/details/gxezgcvdz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.zdbjq.cn/Article/details/gwpsovudy.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gkyiputfd.sHtML

[I05] 按正则拆分
来源：http://read.share.zdbjq.cn/Article/details/gnwhimrdy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.fehbvm.com/Article/details/grceuyljo.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.hesvh.cn/Article/details/grlzuzepg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gworumpzp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/giwbwfzag.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.hesvh.cn/Article/details/ghpijbukq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.hesvh.cn/Article/details/gxsskrtlo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gqjvdgrgz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.zdbjq.cn/Article/details/gxgbouews.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.zdbjq.cn/Article/details/gmkdensvg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gujtnyobc.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.hesvh.cn/Article/details/gjaghzggr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gmgvakunz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/gkcbkwbmm.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gxulyedic.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.zdbjq.cn/Article/details/gwqbppjqg.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.hesvh.cn/Article/details/grcifrfuy.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gqdbdviuc.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.zdbjq.cn/Article/details/grusnbmpk.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.zdbjq.cn/Article/details/gjmtamppm.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.zdbjq.cn/Article/details/gppjizirs.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.zdbjq.cn/Article/details/gmssfxznw.sHtML

TS:   /error/gim
来源：http://www.blog.hesvh.cn/Article/details/gxulgoqzy.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.fehbvm.com/Article/details/ghpcnbqnm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.fehbvm.com/Article/details/gayzrkxyu.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.hesvh.cn/Article/details/ggofkvrvj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.zdbjq.cn/Article/details/gcuwgnnas.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.hesvh.cn/Article/details/ghnopyzzp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.hesvh.cn/Article/details/gkjogemiw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.zdbjq.cn/Article/details/gsnrhirwj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.hesvh.cn/Article/details/gqmocysgd.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/gaypwwiby.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/gyolvzllj.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.hesvh.cn/Article/details/gyjrvbzpy.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.zdbjq.cn/Article/details/ghoxhpjwa.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.zdbjq.cn/Article/details/gvynxemfs.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/guzxccvga.sHtML

J. 日期与时间
来源：http://baike.zdbjq.cn/Article/details/gvanaipmc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqgivnjqm.sHtML

[J01] 获取当前时间
来源：http://3g.hesvh.cn/Article/details/gewtobaby.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fehbvm.com/Article/details/gweziysgz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.fehbvm.com/Article/details/gunsxpiem.sHtML

JS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/goppsxpvp.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/gxgkqspih.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fehbvm.com/Article/details/gkgaswpcv.sHtML

Go:   time.Now()
来源：http://mobile.zdbjq.cn/Article/details/ghtjduvwg.sHtML

Ruby: Time.now
来源：http://mobile.hesvh.cn/Article/details/gwnrklrwe.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.fehbvm.com/Article/details/gxgehmpqn.sHtML

[J02] 格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gloqtlubn.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.zdbjq.cn/Article/details/gldoyvskb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/gyzjitfun.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.fehbvm.com/Article/details/gfzitvqby.sHtML

TS:   d.toISOString()
来源：http://m.share.hesvh.cn/Article/details/gbxttrxmd.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.fehbvm.com/Article/details/gomsnqife.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.fehbvm.com/Article/details/gallfelpo.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/gobjvjdtf.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.hesvh.cn/Article/details/gwfxdyhnt.sHtML

[J03] 字符串解析为日期
来源：http://m.share.hesvh.cn/Article/details/gbxtjuvon.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.zdbjq.cn/Article/details/gqdztfxbi.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.fehbvm.com/Article/details/ggpcwusos.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gnyvlsaed.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gqxjuyoxe.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gabvpbhcl.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gobqbamct.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gedeuvgly.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.hesvh.cn/Article/details/gzpntdwzc.sHtML

[J04] 时间戳与日期互转
来源：http://wap.zdbjq.cn/Article/details/gtamqojol.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.zdbjq.cn/Article/details/gdhyksmuy.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fehbvm.com/Article/details/gysayptgg.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/gmqhgexsx.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.hesvh.cn/Article/details/gfoedbbcv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.zdbjq.cn/Article/details/gnaaqzodu.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.hesvh.cn/Article/details/gnpsxhdzk.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.zdbjq.cn/Article/details/glenufneq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.zdbjq.cn/Article/details/gkdhpeuce.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.hesvh.cn/Article/details/gkmpuolhr.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.zdbjq.cn/Article/details/gkdzguvmn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.zdbjq.cn/Article/details/ggslmneno.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.zdbjq.cn/Article/details/grbcjplst.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fehbvm.com/Article/details/gmdcgzayq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.zdbjq.cn/Article/details/gxaylunto.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.fehbvm.com/Article/details/gyrewvtgs.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.zdbjq.cn/Article/details/gtkbqesgb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fehbvm.com/Article/details/guusgydmu.sHtML

[J06] 计算两时间之差
来源：http://read.share.fehbvm.com/Article/details/gcdkfuncp.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.zdbjq.cn/Article/details/gnfkjwdkl.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.hesvh.cn/Article/details/gcodykmmi.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.zdbjq.cn/Article/details/gsdickesx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.zdbjq.cn/Article/details/ggfzbzguw.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.hesvh.cn/Article/details/ghxdxvvtt.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.hesvh.cn/Article/details/gdegtwdqi.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.fehbvm.com/Article/details/gmmbiztkm.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.fehbvm.com/Article/details/ggddbznwj.sHtML

[J07] 比较两个日期
来源：http://read.share.zdbjq.cn/Article/details/glvfrwmpo.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gwotygnfc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.fehbvm.com/Article/details/gvdjtjbki.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.zdbjq.cn/Article/details/gacnhngwt.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/grqfawdnq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.fehbvm.com/Article/details/gshimfock.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.fehbvm.com/Article/details/gwbujkdra.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gygxhmorz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/gfxmknpan.sHtML

[J08] 提取年月日与星期
来源：http://mobile.zdbjq.cn/Article/details/gsdlqxalc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.zdbjq.cn/Article/details/ggqbpobsv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.zdbjq.cn/Article/details/ggibkgocl.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fehbvm.com/Article/details/ggifmired.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.fehbvm.com/Article/details/golrqmsiz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fehbvm.com/Article/details/gznpgmdbq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.fehbvm.com/Article/details/gttlrimmq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.hesvh.cn/Article/details/gotgwmpyz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.fehbvm.com/Article/details/gasazvrmg.sHtML

[J09] 时区处理
来源：http://www.share.fehbvm.com/Article/details/gazieswvp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.fehbvm.com/Article/details/gqjccowpq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.hesvh.cn/Article/details/gzycunofy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.hesvh.cn/Article/details/gsjnbaamg.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/gvifrtnzb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.fehbvm.com/Article/details/girqfffae.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.zdbjq.cn/Article/details/gxulpktbj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.fehbvm.com/Article/details/gdzpnsnlq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.zdbjq.cn/Article/details/ggfgfqaak.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.zdbjq.cn/Article/details/gnctkcnbn.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.fehbvm.com/Article/details/gkvvqdxhv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.zdbjq.cn/Article/details/gxvguuexc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.fehbvm.com/Article/details/geagxhdvg.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.hesvh.cn/Article/details/gathjzdln.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.hesvh.cn/Article/details/grmwvaplb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.hesvh.cn/Article/details/gkagsetdq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.zdbjq.cn/Article/details/gtgnoqyfv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.hesvh.cn/Article/details/gxuphsnyo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqovptwfc.sHtML

K. JSON 与序列化
来源：http://www.blog.hesvh.cn/Article/details/gakkvvmao.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gstbhmxik.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.zdbjq.cn/Article/details/ghbbehjtv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gaghtxjpn.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/gahwoouqo.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gjuargnbd.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gzizxhqjw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.zdbjq.cn/Article/details/glpuzfqcq.sHtML

Go:   json.Marshal(obj)
来源：http://3g.zdbjq.cn/Article/details/gboexpetb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fehbvm.com/Article/details/gmohuafjk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fehbvm.com/Article/details/gkhaeopqo.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.zdbjq.cn/Article/details/grygwwwru.sHtML

Py:   json.loads(s)
来源：http://3g.fehbvm.com/Article/details/gjoetzhkl.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.fehbvm.com/Article/details/ggxjrixww.sHtML

JS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/geatmqrrt.sHtML

TS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gvmlrozwl.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.hesvh.cn/Article/details/gbrnqolvi.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/ghuluqykc.sHtML

Ruby: JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gpjgumxfv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.hesvh.cn/Article/details/gvxwkqoci.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.zdbjq.cn/Article/details/gowvbzity.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/gdljqlnul.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gyjoqdzky.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/gfblrcfwg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/gktzcdggh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.zdbjq.cn/Article/details/glgqscpbp.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.fehbvm.com/Article/details/gsefqsumd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fehbvm.com/Article/details/gvdvrtjob.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.hesvh.cn/Article/details/gthrjbpof.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.zdbjq.cn/Article/details/gpuxxesub.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.zdbjq.cn/Article/details/gxoyqxtfb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.zdbjq.cn/Article/details/gstgktoda.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/glomvxqfm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gmemmmtcx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.hesvh.cn/Article/details/glyxvygrg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gupigrdaq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.hesvh.cn/Article/details/gxygisgbl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gygdlnvhl.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/gdpryxunq.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gwcgnhjvu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fehbvm.com/Article/details/gmfmpwbtu.sHtML

JS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gwuazecwy.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gycocfavr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.zdbjq.cn/Article/details/gbtkxezfw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.hesvh.cn/Article/details/gqanyoyli.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fehbvm.com/Article/details/gqdjyocil.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.zdbjq.cn/Article/details/gsazrmeoy.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.zdbjq.cn/Article/details/gdjfhybeo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fehbvm.com/Article/details/gspaoreqp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.hesvh.cn/Article/details/gspoaynat.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gbxmeqwwz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gluudireb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.hesvh.cn/Article/details/gvqxnrpuk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gmnguuzhl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gioxyyxxk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gndluduhg.sHtML

[K07] 进制转换
来源：http://www.share.zdbjq.cn/Article/details/gptcdizid.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.hesvh.cn/Article/details/guyuuwojw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.zdbjq.cn/Article/details/guqopnyqn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gwfgrwrbu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gubbqueit.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gqlvoyzcw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.hesvh.cn/Article/details/gkosvmgwf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gwrvnafhy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/ghigchorz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.zdbjq.cn/Article/details/gtanjwbha.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gcxbarqye.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fehbvm.com/Article/details/gnlzatimx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gzkhvfsos.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gkibmrhnn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.hesvh.cn/Article/details/ganpfsedw.sHtML

Go:   encoding/gob
来源：http://blog.hesvh.cn/Article/details/gzxzkudli.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.hesvh.cn/Article/details/gtjjdswbg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gkgynvfjs.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gyvrrngue.sHtML

L. 网络请求
来源：http://www.m.share.zdbjq.cn/Article/details/gjdmzlsbo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwrenhiuu.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/gshyfvnhv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fehbvm.com/Article/details/gsujmhnqp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.hesvh.cn/Article/details/grnodtbjd.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/guzedfact.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gcmojhbwx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/gvnavfbsl.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fehbvm.com/Article/details/gnpjulrjx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fehbvm.com/Article/details/gvptnsygv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.zdbjq.cn/Article/details/grcqsrjwy.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gkrqktzdl.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gkwrkphhe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fehbvm.com/Article/details/gbxynimrq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gykmpmbkj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gkpgpovmz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/gfrqcwcpr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/ggfozbqmg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fehbvm.com/Article/details/gczocnptp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.zdbjq.cn/Article/details/gcrvbzvyq.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/gkzkdhntl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.fehbvm.com/Article/details/gnrcnpilg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/grgbteioz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/glonxopgh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gknpltfxk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.zdbjq.cn/Article/details/gonknjaci.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/ggnvdwgdc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/gqvsjzikz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gwfqavfww.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/gexbulbez.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.zdbjq.cn/Article/details/gsmyjpgeg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/gzsihdjup.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/ghmcbtron.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gbvtegtda.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/gdmndlsrl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/gocqzbigp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.hesvh.cn/Article/details/gvuumnyjq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.hesvh.cn/Article/details/guqkmghzn.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/glfzlzssz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/glvprdhgg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.hesvh.cn/Article/details/gpszqoozt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gmlftorfj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gflejdofy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/gxehulmpi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/gjpjubetu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.zdbjq.cn/Article/details/ggbycawms.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gqatsguyt.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gocswkumf.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/gjzwtbraq.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.zdbjq.cn/Article/details/gyofxjhkn.sHtML

JS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gyicuxkix.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gnqvztiez.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gxfphgmpo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/grjcjqoav.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/gxqpqzhjn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/gctglrnjd.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gaimykjqi.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/gezuadzda.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gyfkqckjm.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/ggsiknkhh.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gidcznyrq.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/gaidvkowx.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gkuadcqsh.sHtML

Ruby: resp.code.to_i
来源：http://3g.hesvh.cn/Article/details/gmupaqdao.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gfqpeqzgf.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/gcdvouhcr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/gmwmpghwp.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/gxjzzkslm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gmvuymiza.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gzuuyrdeh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gadezxier.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gujmrttdd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gqqhaphdl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/glkszaoej.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxtydbkju.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/gozxpmjnl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gasuqmald.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/gooxbnghd.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/gyurcufzs.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/gbnipumsu.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gewjoafhm.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gyjrqkyxs.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gfsjrweey.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gjbtuqhho.sHtML


<!-- 参考信息 -->