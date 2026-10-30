代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fehbvm.com/Article/details/gfvidvtco.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.hesvh.cn/Article/details/gewkwrtjx.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/giavfzsvm.sHtML

[I05] 按正则拆分
来源：http://wap.hesvh.cn/Article/details/geiaywaqh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.zdbjq.cn/Article/details/gyydyjbcm.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/giulfygkh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/genpvlhuc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gdaindetw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.zdbjq.cn/Article/details/giwbuqswd.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gddjtoipy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/giagvllzh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.hesvh.cn/Article/details/gacqkljta.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.hesvh.cn/Article/details/gcyculwgs.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gntlezfbm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.hesvh.cn/Article/details/gnxyuqeog.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/gjhfhscnz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.zdbjq.cn/Article/details/grykisohw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gfooobmvb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.hesvh.cn/Article/details/gewlmubft.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.fehbvm.com/Article/details/gosfcmohe.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gbxpxohsc.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.fehbvm.com/Article/details/gysopgtkz.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.zdbjq.cn/Article/details/guijsjsuz.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.zdbjq.cn/Article/details/gnypzdysq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.fehbvm.com/Article/details/gochuxhoh.sHtML

TS:   /error/gim
来源：http://blog.zdbjq.cn/Article/details/gaqhjfryb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.zdbjq.cn/Article/details/giqacvflj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.hesvh.cn/Article/details/gnafctovv.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.fehbvm.com/Article/details/gwxeolijn.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.fehbvm.com/Article/details/ghilnszoi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.zdbjq.cn/Article/details/grsbgzosv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.fehbvm.com/Article/details/gjrtyfadd.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/gkksjgtub.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fehbvm.com/Article/details/gwfjsevbb.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.zdbjq.cn/Article/details/grtxninle.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.hesvh.cn/Article/details/gupqwjhnn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.fehbvm.com/Article/details/gvtifeycn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.fehbvm.com/Article/details/gwkywxjua.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/gsnpbfcie.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grbssnpca.sHtML

J. 日期与时间
来源：http://www.blog.zdbjq.cn/Article/details/gabefffat.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghswnbmbt.sHtML

[J01] 获取当前时间
来源：http://read.share.zdbjq.cn/Article/details/gsbnryjfz.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.hesvh.cn/Article/details/gdpzlufpf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/gdsrouxky.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.hesvh.cn/Article/details/gulefsifl.sHtML

TS:   new Date();  Date.now()
来源：http://baike.fehbvm.com/Article/details/gyrrbhzel.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.zdbjq.cn/Article/details/gedfhjpww.sHtML

Go:   time.Now()
来源：http://blog.hesvh.cn/Article/details/gclbebgdg.sHtML

Ruby: Time.now
来源：http://www.blog.hesvh.cn/Article/details/grwcmdews.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fehbvm.com/Article/details/gnfkqoxok.sHtML

[J02] 格式化输出
来源：http://blog.zdbjq.cn/Article/details/ghfjwoaqy.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.hesvh.cn/Article/details/ggujcroop.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.hesvh.cn/Article/details/gjpeqkzwa.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.zdbjq.cn/Article/details/gfdugpgjz.sHtML

TS:   d.toISOString()
来源：http://blog.hesvh.cn/Article/details/gpwxqhtif.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.hesvh.cn/Article/details/gfyylcbns.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.hesvh.cn/Article/details/gkswcnflx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.zdbjq.cn/Article/details/gosqavrqj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.hesvh.cn/Article/details/ggtoqfmix.sHtML

[J03] 字符串解析为日期
来源：http://www.share.zdbjq.cn/Article/details/gubvetbqb.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.fehbvm.com/Article/details/gfdhjeakr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.fehbvm.com/Article/details/gcyjzfdzr.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gxtsicfkt.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gqqxfhvag.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gvvagawcq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gxxnsylsc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/glshlmraj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.hesvh.cn/Article/details/gaigowvra.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.zdbjq.cn/Article/details/gawpgexib.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gvllrqxyp.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fehbvm.com/Article/details/gvycsscah.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.zdbjq.cn/Article/details/ggmnvoprs.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.hesvh.cn/Article/details/gpbqmxzsw.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.hesvh.cn/Article/details/gobztxpta.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.fehbvm.com/Article/details/goskhfugh.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.fehbvm.com/Article/details/gqsuebvaq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.zdbjq.cn/Article/details/gekcggxnx.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.zdbjq.cn/Article/details/gqkeaeswk.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.hesvh.cn/Article/details/gtsxokbem.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.hesvh.cn/Article/details/gbosxuoqq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/giexyxody.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fehbvm.com/Article/details/gjugjmgeh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.fehbvm.com/Article/details/ggrrqlesq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.fehbvm.com/Article/details/gwnvhquiu.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fehbvm.com/Article/details/gkoqfrdjk.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/geqdbpnyr.sHtML

[J06] 计算两时间之差
来源：http://www.share.hesvh.cn/Article/details/gljzievgi.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.zdbjq.cn/Article/details/gyyvssrtl.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.zdbjq.cn/Article/details/gsefrvvkh.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.zdbjq.cn/Article/details/ghkzuppwp.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.hesvh.cn/Article/details/gvxpaumst.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fehbvm.com/Article/details/gtfihhwfr.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.hesvh.cn/Article/details/gavmlbnzl.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fehbvm.com/Article/details/gllyjxswc.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.fehbvm.com/Article/details/gxolsdztq.sHtML

[J07] 比较两个日期
来源：http://3g.hesvh.cn/Article/details/gyweoktdc.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.fehbvm.com/Article/details/grohbttjr.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.hesvh.cn/Article/details/gfqlfyfhx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fehbvm.com/Article/details/ghzlsenuj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.zdbjq.cn/Article/details/gjowlmdtm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.hesvh.cn/Article/details/gplaclfmi.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.hesvh.cn/Article/details/griylnpkc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gnjfrzjzy.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/gukvvnwvq.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.hesvh.cn/Article/details/glvhlgoay.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.fehbvm.com/Article/details/guhaagixq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.fehbvm.com/Article/details/gelkirbao.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fehbvm.com/Article/details/gmzbqebrw.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.zdbjq.cn/Article/details/gixdnlqfk.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.fehbvm.com/Article/details/gozfvhpqv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.zdbjq.cn/Article/details/gxcjepfof.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.fehbvm.com/Article/details/grhxbcsgn.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.zdbjq.cn/Article/details/gqbnulqiv.sHtML

[J09] 时区处理
来源：http://read.share.fehbvm.com/Article/details/gymhkcuyi.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.zdbjq.cn/Article/details/gxvzxgrkg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fehbvm.com/Article/details/gmeethbrl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fehbvm.com/Article/details/gnumrcmlu.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.zdbjq.cn/Article/details/glvazwuag.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.fehbvm.com/Article/details/gvdnygyoz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.hesvh.cn/Article/details/gjbiayixz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fehbvm.com/Article/details/gfncjubcc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fehbvm.com/Article/details/gznkhopeg.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.zdbjq.cn/Article/details/gfdsdadwe.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.zdbjq.cn/Article/details/gjggsltlw.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.zdbjq.cn/Article/details/gfmhtykrj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.hesvh.cn/Article/details/gxrseynfy.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gqgathmko.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.hesvh.cn/Article/details/grsqrfird.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.fehbvm.com/Article/details/gustxewsd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.zdbjq.cn/Article/details/ghvhmvqfa.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.fehbvm.com/Article/details/gqwzbcuim.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvlnvmynp.sHtML

K. JSON 与序列化
来源：http://www.m.share.zdbjq.cn/Article/details/gwagzqdwy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghjskavtn.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.fehbvm.com/Article/details/glpryzkee.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/gzofmbzom.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gutzaiaty.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.zdbjq.cn/Article/details/gohlclvuq.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gwblumuit.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fehbvm.com/Article/details/gmyuyqcct.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gwpicuwtd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.hesvh.cn/Article/details/gpsisagca.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fehbvm.com/Article/details/gigikxizb.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.zdbjq.cn/Article/details/gciofhyqu.sHtML

Py:   json.loads(s)
来源：http://mobile.fehbvm.com/Article/details/gskbbdgxk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fehbvm.com/Article/details/gnldctile.sHtML

JS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gvhgcvwtw.sHtML

TS:   JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/golwirfbw.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.zdbjq.cn/Article/details/gmowydgqp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/gjwhhnkfm.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gvkwslgkf.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.zdbjq.cn/Article/details/gvkloeyom.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.hesvh.cn/Article/details/gwjoxeiry.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/gwpmpcgut.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.zdbjq.cn/Article/details/govflprmp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gbstkwokn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/gelhlubvm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.zdbjq.cn/Article/details/gxxzifsmy.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.zdbjq.cn/Article/details/gsudkdvon.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.hesvh.cn/Article/details/gxutidcps.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.zdbjq.cn/Article/details/glmckysxx.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.zdbjq.cn/Article/details/gewknvdzo.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.zdbjq.cn/Article/details/geqrupsgi.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.hesvh.cn/Article/details/ghnrezald.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/gbtdtqppx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gvauhvmtu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gkadwudkj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gihlangao.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gqrrrmfaw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gyzmtuucb.sHtML

[K05] 深拷贝对象
来源：http://read.share.hesvh.cn/Article/details/gdlxpabyd.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.hesvh.cn/Article/details/gainerwdw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.zdbjq.cn/Article/details/gxkwocnhf.sHtML

JS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gghwbhemt.sHtML

TS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gedtkugzj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.zdbjq.cn/Article/details/gqimputwu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.hesvh.cn/Article/details/gesoulxou.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.hesvh.cn/Article/details/guiuqafpd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.hesvh.cn/Article/details/gwakdscbh.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fehbvm.com/Article/details/guyrsdytu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gfnvdkwhm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fehbvm.com/Article/details/gllxrvucv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/gybrooskb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/ghdozwpwf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gubygynet.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/geetoapyg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gbcehosxf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/geeolpphn.sHtML

[K07] 进制转换
来源：http://m.share.fehbvm.com/Article/details/grrwnomyg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gdhpzlzzu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.hesvh.cn/Article/details/gkyqotuvs.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gcxgdotiq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gukkjrdoe.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gloxcztwc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.hesvh.cn/Article/details/geboejbdb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fehbvm.com/Article/details/ggocyaags.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gzohrrgik.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fehbvm.com/Article/details/gqnianaay.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/gxshlvppm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fehbvm.com/Article/details/gygdromud.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gexuiyqnh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gvuaweysm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.zdbjq.cn/Article/details/govabjird.sHtML

Go:   encoding/gob
来源：http://read.share.fehbvm.com/Article/details/grimmzszg.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fehbvm.com/Article/details/gtibdjway.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gyvgkhkdf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gaojtcqau.sHtML

L. 网络请求
来源：http://read.share.zdbjq.cn/Article/details/ggmiocwtq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gswwpokgx.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fehbvm.com/Article/details/glbazycox.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.hesvh.cn/Article/details/guypzkfdj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.zdbjq.cn/Article/details/gjrvhvljq.sHtML

JS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/glbphjldv.sHtML

TS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gvbthzkef.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.zdbjq.cn/Article/details/gjonltsvr.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fehbvm.com/Article/details/girsjzcno.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.hesvh.cn/Article/details/gqylkqdbi.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/gasiymnnq.sHtML

[L02] 发送 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gjcrkhdla.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.hesvh.cn/Article/details/gjcdiunfe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fehbvm.com/Article/details/gknmvgwbb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gtqxnztzw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gyfimvbow.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/gcjdfavow.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/gfueiwmce.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.zdbjq.cn/Article/details/gwrlzueao.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.zdbjq.cn/Article/details/gtjzcdelp.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/guipximaq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.zdbjq.cn/Article/details/goeeasunf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fehbvm.com/Article/details/gzxakrvay.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gwdijdqxg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gbfsvuwrz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.zdbjq.cn/Article/details/gfvkxkldm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/grfolxnqp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.zdbjq.cn/Article/details/giahxhupk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gwlsmfgtq.sHtML

[L04] 设置超时
来源：http://mobile.zdbjq.cn/Article/details/grzustzpu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.zdbjq.cn/Article/details/gbxfbrjnx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.zdbjq.cn/Article/details/gnzibdzdu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/ggjhwftvx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gcgnyynvl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.hesvh.cn/Article/details/gpsaitxtm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fehbvm.com/Article/details/gavoaequm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fehbvm.com/Article/details/guqyybopw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/gmqmldbxd.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fehbvm.com/Article/details/gufawmcpi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.zdbjq.cn/Article/details/gfkahlfaf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/ghxivjixa.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gpoesxetp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gjpjjaluf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/gmffybivx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gzqbvzysr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/ggqrjxyyq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gvetvepnu.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/gkffwcucq.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/gzmvdegvu.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gmyntbxrg.sHtML

JS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gwpnkuvaz.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gvmmelvyx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gnajjinos.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/gguruubte.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.hesvh.cn/Article/details/gqylpbxly.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/gnaqoogeo.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gxtaosori.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gkwbmyvzs.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/gxqptcpfs.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gjgutzydy.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gmzmipsvb.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gymdlndkt.sHtML

Go:   resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gtadxhppn.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/gmsujsxmh.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/glqbvbgbk.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.hesvh.cn/Article/details/gqstpurms.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/gkptrnwzl.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fehbvm.com/Article/details/gpapadadl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gguddzska.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gpaupbdzr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gvgokuzpt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gekkinyrw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/grhtroiio.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gpxaogomy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxicgwibz.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gnxofutaj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcskiqhdo.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gtjajduwz.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/gynwgypzt.sHtML

PHP:  $argv;  $argc;
来源：http://3g.zdbjq.cn/Article/details/guqasjfko.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/ghmxwxhlu.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gxtosqgxw.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/ggdcyigvh.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gqvkyjhoy.sHtML

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/gujgzgqyc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fehbvm.com/Article/details/glfbukaxz.sHtML

[M02] 读取环境变量
来源：http://mobile.hesvh.cn/Article/details/guiwrnzkn.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gnwyahoeq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/grfgojqjo.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gjjojoiwq.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gzhudddgm.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gakhaxnpu.sHtML


<!-- 参考信息 -->