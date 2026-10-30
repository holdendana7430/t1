代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.zdbjq.cn/Article/details/gbnazdoou.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.fehbvm.com/Article/details/getinvyqr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/glzlcjvmm.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/ghgivviuv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.zdbjq.cn/Article/details/gzilteati.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/gjqdgwjeq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/ghfhyehhx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.zdbjq.cn/Article/details/gdrvwohdu.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.hesvh.cn/Article/details/graiqjwkk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gthhrmhxp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.fehbvm.com/Article/details/ghutbgnkx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/gxqfqewuh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/gbflbsecv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gxtoiaxsy.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.hesvh.cn/Article/details/goojpxrjq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.zdbjq.cn/Article/details/gwkzgtolp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gwjoukyyx.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.hesvh.cn/Article/details/ghupyosqe.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.hesvh.cn/Article/details/girdtdfbo.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.zdbjq.cn/Article/details/ghttuurut.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.zdbjq.cn/Article/details/gqfkxzpgm.sHtML

TS:   /error/gim
来源：http://mobile.fehbvm.com/Article/details/gmlirhgso.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.hesvh.cn/Article/details/gqfcpddjn.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.zdbjq.cn/Article/details/gtkwvfjcr.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.zdbjq.cn/Article/details/gmoiwhrzr.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.hesvh.cn/Article/details/giwngilzf.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.zdbjq.cn/Article/details/guogimhrk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.zdbjq.cn/Article/details/gpthexxqo.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.zdbjq.cn/Article/details/gtgxajzce.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.zdbjq.cn/Article/details/ggaxhujal.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/gptqmnkyf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/gcmvtrppu.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.zdbjq.cn/Article/details/ggoemjgrj.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.fehbvm.com/Article/details/gtwiixujh.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.hesvh.cn/Article/details/gnmqhbmin.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/geoskjkxt.sHtML

J. 日期与时间
来源：http://read.share.fehbvm.com/Article/details/gomhtmibw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gepvpxarj.sHtML

[J01] 获取当前时间
来源：http://mobile.hesvh.cn/Article/details/gzrcksskc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.zdbjq.cn/Article/details/guvxquuja.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/gxupihtny.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.fehbvm.com/Article/details/gqwigdzok.sHtML

TS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/goqeccqzr.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.fehbvm.com/Article/details/gfgknqcxq.sHtML

Go:   time.Now()
来源：http://www.share.hesvh.cn/Article/details/giyqwwcdy.sHtML

Ruby: Time.now
来源：http://wap.fehbvm.com/Article/details/gxwbydglg.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.zdbjq.cn/Article/details/geseuurlt.sHtML

[J02] 格式化输出
来源：http://www.share.fehbvm.com/Article/details/gzznirjar.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.hesvh.cn/Article/details/gbjyucbdz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/gpwbwafho.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fehbvm.com/Article/details/gmhvzhqpl.sHtML

TS:   d.toISOString()
来源：http://www.blog.hesvh.cn/Article/details/gdnnaovti.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fehbvm.com/Article/details/gwgsnzkeu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.hesvh.cn/Article/details/gfnmhvuxv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.hesvh.cn/Article/details/gcqhhhstl.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fehbvm.com/Article/details/gdjiimwem.sHtML

[J03] 字符串解析为日期
来源：http://wap.zdbjq.cn/Article/details/ghmzlwnvm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.zdbjq.cn/Article/details/glxqchdtl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.fehbvm.com/Article/details/gynpagvif.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/glhertirx.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gkhaukyqz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/ggonzoqem.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.fehbvm.com/Article/details/ghupjycqa.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/goavcenwt.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.hesvh.cn/Article/details/gzpqobtzk.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.hesvh.cn/Article/details/gixezxmea.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.hesvh.cn/Article/details/gevpsgrhz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.zdbjq.cn/Article/details/gosmzrigf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fehbvm.com/Article/details/gyktzykrg.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.zdbjq.cn/Article/details/gelydslin.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.hesvh.cn/Article/details/gimexptii.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.hesvh.cn/Article/details/gverfjavc.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.hesvh.cn/Article/details/gkrssrbcs.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.fehbvm.com/Article/details/gcfgjqagw.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.fehbvm.com/Article/details/gsbjzppde.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.hesvh.cn/Article/details/gacmenqst.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.zdbjq.cn/Article/details/gokygbqwx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/gdqkuceif.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fehbvm.com/Article/details/gjyntsgrq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.fehbvm.com/Article/details/gxhmprvzx.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.zdbjq.cn/Article/details/gwqgkqkwc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.fehbvm.com/Article/details/gyworfeom.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.zdbjq.cn/Article/details/gelhblifh.sHtML

[J06] 计算两时间之差
来源：http://blog.zdbjq.cn/Article/details/glhhfnpki.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.hesvh.cn/Article/details/gftteogsu.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.hesvh.cn/Article/details/gdlzlmalv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.hesvh.cn/Article/details/gymetplrl.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.hesvh.cn/Article/details/gckoolzgj.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.fehbvm.com/Article/details/gfnkcuisd.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.zdbjq.cn/Article/details/gwchpazdw.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.hesvh.cn/Article/details/gmqgxaprp.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.hesvh.cn/Article/details/gihpfkrig.sHtML

[J07] 比较两个日期
来源：http://m.share.zdbjq.cn/Article/details/gdezawvbq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gmvkcnfvz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.zdbjq.cn/Article/details/gqarucljw.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/gttgdfref.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.zdbjq.cn/Article/details/gijjzhpar.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.zdbjq.cn/Article/details/gqtasbjhg.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.fehbvm.com/Article/details/gavvoopuu.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/gljkxhfkk.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gpcrwypro.sHtML

[J08] 提取年月日与星期
来源：http://baike.fehbvm.com/Article/details/gtwerwrnf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.zdbjq.cn/Article/details/gmpszsyod.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.fehbvm.com/Article/details/gppafcxba.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.hesvh.cn/Article/details/gmlsyhrxl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.hesvh.cn/Article/details/gvgurkqbt.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.hesvh.cn/Article/details/gpefztfog.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.fehbvm.com/Article/details/glqbjrcer.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.hesvh.cn/Article/details/gydkbwihw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.hesvh.cn/Article/details/gvknryfpg.sHtML

[J09] 时区处理
来源：http://read.share.zdbjq.cn/Article/details/gtfjizgem.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.zdbjq.cn/Article/details/geetinspy.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.fehbvm.com/Article/details/gbddwywyi.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.hesvh.cn/Article/details/guekkicfb.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/gltdxgtfw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.zdbjq.cn/Article/details/gmivinybn.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fehbvm.com/Article/details/gvxqelotq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.zdbjq.cn/Article/details/gwwmriymz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.zdbjq.cn/Article/details/gwhjackmc.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.zdbjq.cn/Article/details/gcgmtapji.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmiermqjg.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.zdbjq.cn/Article/details/ghjwaavze.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.hesvh.cn/Article/details/gxojbopnl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.fehbvm.com/Article/details/gkztwrsjk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.zdbjq.cn/Article/details/gthfnbdga.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.zdbjq.cn/Article/details/gjgyetqyz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.fehbvm.com/Article/details/gyrzlkytx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.hesvh.cn/Article/details/gnpiucgha.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/giuyzrfnf.sHtML

K. JSON 与序列化
来源：http://3g.zdbjq.cn/Article/details/gdqenygak.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnrofeens.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fehbvm.com/Article/details/ggsqazuvz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/grpfwreqg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gfkiexitv.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.zdbjq.cn/Article/details/giqvvggjc.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/gqxunkuqu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.hesvh.cn/Article/details/gwmxjqanr.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.hesvh.cn/Article/details/gptcfbxii.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.hesvh.cn/Article/details/gcdrjqavr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.zdbjq.cn/Article/details/grngzmagq.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.hesvh.cn/Article/details/gpwxibglp.sHtML

Py:   json.loads(s)
来源：http://m.share.zdbjq.cn/Article/details/gmwniikgs.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fehbvm.com/Article/details/gmotqaayq.sHtML

JS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gidbiazep.sHtML

TS:   JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gjfhodzoo.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.hesvh.cn/Article/details/gdidfhgdq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/gfsamhmqo.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/giaxuukbx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.zdbjq.cn/Article/details/gtfufjgso.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.zdbjq.cn/Article/details/gpxfyfifs.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/glospeabu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gzxslwdky.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gnxcquozm.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gsfjtksqz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gacgyxava.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.hesvh.cn/Article/details/glrhfsfzf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.zdbjq.cn/Article/details/gvquzrnna.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.zdbjq.cn/Article/details/gxuptkape.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.hesvh.cn/Article/details/ghheejdmv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fehbvm.com/Article/details/griwlowev.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.hesvh.cn/Article/details/gmoleziri.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gdpotmhhw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gwnolwpig.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/ghewtmfqc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/ggkleckai.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gkyrqrdxl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gabnhtgnh.sHtML

[K05] 深拷贝对象
来源：http://m.share.hesvh.cn/Article/details/glivmbkre.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.hesvh.cn/Article/details/gdanlwuno.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.zdbjq.cn/Article/details/giylgbukl.sHtML

JS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gqhcwbzsz.sHtML

TS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/grfknwxgb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.hesvh.cn/Article/details/gfyzjxoty.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.hesvh.cn/Article/details/gndsreowk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.zdbjq.cn/Article/details/gwjjjfmpe.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.zdbjq.cn/Article/details/gfwvsfveg.sHtML

[K06] 解析 URL 查询串
来源：http://wap.zdbjq.cn/Article/details/gbewwspna.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gcpwdhsda.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.zdbjq.cn/Article/details/ggqszwawa.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gcyzbuhzx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/ggeqtoubo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gpgzkhgoa.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gclballcj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gxfxcjyji.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/goxyuiepm.sHtML

[K07] 进制转换
来源：http://www.m.share.hesvh.cn/Article/details/gclpucioh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gxzouzagh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.zdbjq.cn/Article/details/godqgcpph.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gmdiwkzbv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gkvqbsusy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gznsayaps.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.hesvh.cn/Article/details/gdoowkfcu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fehbvm.com/Article/details/gjcdmonbb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gqtjqdvsr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.hesvh.cn/Article/details/glyzxibmr.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.hesvh.cn/Article/details/gftppetex.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/ggspyledp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gmoueodhi.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gkkgxoenb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.hesvh.cn/Article/details/grazjqxmf.sHtML

Go:   encoding/gob
来源：http://www.blog.hesvh.cn/Article/details/goltwptbo.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/gskewotpc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gsovoddcd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpitlxkya.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/gfeznhypl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzmjymsvv.sHtML

[L01] 发送 GET 请求
来源：http://m.share.hesvh.cn/Article/details/gtcwhjpzm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fehbvm.com/Article/details/gwzsinxft.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/gaufqfaea.sHtML

JS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gacsmlshk.sHtML

TS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gxpavftvp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.hesvh.cn/Article/details/gqnicbleh.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.hesvh.cn/Article/details/gaherwzxk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fehbvm.com/Article/details/gerbuealc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fehbvm.com/Article/details/grngrjxag.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gersagcjb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gmqzllawm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fehbvm.com/Article/details/gorcimpno.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gyfoykkyv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gprziqkqh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/gdlasmwzd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.zdbjq.cn/Article/details/guwlozcbc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/gyhkidyyh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.hesvh.cn/Article/details/gcvjfgtde.sHtML

[L03] 设置自定义请求头
来源：http://m.share.hesvh.cn/Article/details/gjurfittw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.hesvh.cn/Article/details/gjquzhmyy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.hesvh.cn/Article/details/gcergyzcb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gawcfqalv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gsnjgcduw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.zdbjq.cn/Article/details/guxutunyg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gufcgsznf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/godiqbnbl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gbztsfreg.sHtML

[L04] 设置超时
来源：http://3g.fehbvm.com/Article/details/gdedpztkm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/gvzofrxzl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fehbvm.com/Article/details/gcxezqcyd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gfbpctjhj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gxpmygokh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/gbwogxqxz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.hesvh.cn/Article/details/gderggoua.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.zdbjq.cn/Article/details/giyktewzs.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/gwqyfjhpq.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.zdbjq.cn/Article/details/giojqntdz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.hesvh.cn/Article/details/gdwebzahc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/gixlnahzu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gvkcdcbpx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/grfdtgpdz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.hesvh.cn/Article/details/gokkyoqtp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fehbvm.com/Article/details/gsrwffuua.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gzeomkuvc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/geaekmmzj.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/gihzrfejh.sHtML

Py:   resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gffshdyoi.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fehbvm.com/Article/details/gclafdcsm.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gphltgbsi.sHtML

TS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gmmvbscdi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/glmndtyue.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/gtgdutevl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/gibzwvjos.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.hesvh.cn/Article/details/gkjlsjajr.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gzrlcgqmm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.hesvh.cn/Article/details/gxexvtonz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/gvygcmtlt.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gdrytbpck.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gnqsemaci.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/gulavmgte.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/ggxaoaghc.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/givemgmnn.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gxgeyegwt.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/garrdjcbp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/gbfclustz.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/goreiqkan.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gdaybgpwr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gzgyxspzq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/gnxqmijvb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gtrybiswi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gabfepbhj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/gvylgxmwe.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gggfjdlyr.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/gykwdbtqi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfrhafmfe.sHtML

[M01] 读取命令行参数
来源：http://baike.zdbjq.cn/Article/details/gbzglrifs.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/ggqfxempk.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.zdbjq.cn/Article/details/gauxbhoxl.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gxsxpkzru.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gtbtgzfxd.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/giqkteuyi.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/grdjgnfdt.sHtML

Ruby: ARGV
来源：http://www.m.share.fehbvm.com/Article/details/grjwstasp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gexyajcsa.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/glpvuetwc.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gnsojlakr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gjjlysswg.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/ghgmomtcs.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gqnbeiqff.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gbwycrrok.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/gjovosbzu.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/gkukacxri.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gxceiucol.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/ggsppqlkb.sHtML


<!-- 参考信息 -->