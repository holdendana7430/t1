代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://baike.fanxiaobao.xyz/Article/details/gfrzwpbsz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gnvhpphwl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtqaxwjj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.fanxiaobao.xyz/Article/details/gqcdypzbp.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fanxiaobao.xyz/Article/details/gyidqwmua.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.fanxiaobao.xyz/Article/details/gglgignqv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.fanxiaobao.xyz/Article/details/gigzppmck.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrgubczf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fanxiaobao.xyz/Article/details/gueahccvg.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqedokwg.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlidvpfz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrhwyfid.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbksiahf.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.fanxiaobao.xyz/Article/details/gyszpdajf.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.fanxiaobao.xyz/Article/details/gloldmtsz.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpnssmzp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewsymogf.sHtML

TS:   /error/gim
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpexmfud.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqgnrkts.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfelpuho.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gulplgexq.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.fanxiaobao.xyz/Article/details/gslucpvsh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gaogvpbrz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrvqcsys.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.fanxiaobao.xyz/Article/details/gdqzwqxio.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fanxiaobao.xyz/Article/details/gchcruorj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fanxiaobao.xyz/Article/details/gvxvhuoca.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fanxiaobao.xyz/Article/details/gowqpinht.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.fanxiaobao.xyz/Article/details/graurrsjc.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.fanxiaobao.xyz/Article/details/gzqditkjj.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhipeyqn.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gczboscwc.sHtML

J. 日期与时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gfeayshsd.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gzxixeaza.sHtML

[J01] 获取当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcrpdsyr.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwjjenjm.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.fanxiaobao.xyz/Article/details/grsntouuf.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxogcymdw.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqwpvsbo.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpoppzxx.sHtML

Go:   time.Now()
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgkuhvum.sHtML

Ruby: Time.now
来源：http://wap.fanxiaobao.xyz/Article/details/gsufxvabh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.fanxiaobao.xyz/Article/details/gjtoqpjlq.sHtML

[J02] 格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/guivwtskg.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fanxiaobao.xyz/Article/details/gckuhubgs.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyjcdvrv.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fanxiaobao.xyz/Article/details/gxipxzgug.sHtML

TS:   d.toISOString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcidfmub.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsjqlmsq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbmpyvpi.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnpkrbem.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpswmvgxg.sHtML

[J03] 字符串解析为日期
来源：http://3g.fanxiaobao.xyz/Article/details/ggnydsvek.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjocxcly.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.fanxiaobao.xyz/Article/details/grtyajzon.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.fanxiaobao.xyz/Article/details/gkyhmxemh.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnishytkb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzymewaub.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.fanxiaobao.xyz/Article/details/gqgfsjcdf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.fanxiaobao.xyz/Article/details/gjmzcokox.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.fanxiaobao.xyz/Article/details/gduqpojso.sHtML

[J04] 时间戳与日期互转
来源：http://wap.fanxiaobao.xyz/Article/details/gufqqotds.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcgjkaek.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswcaxszj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrrrvbkw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.fanxiaobao.xyz/Article/details/glsiqmmvu.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.fanxiaobao.xyz/Article/details/gotuhoxze.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gviorwleo.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.fanxiaobao.xyz/Article/details/gltcmdedu.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqlvjehd.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.fanxiaobao.xyz/Article/details/grhxjwqfx.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsbrozbi.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.fanxiaobao.xyz/Article/details/gthlyxorx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fanxiaobao.xyz/Article/details/gefnfikbl.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fanxiaobao.xyz/Article/details/guuiaucvn.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncwdvozl.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.fanxiaobao.xyz/Article/details/gmsfnfajh.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnpriyzz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fanxiaobao.xyz/Article/details/gebexfuvj.sHtML

[J06] 计算两时间之差
来源：http://blog.fanxiaobao.xyz/Article/details/gyhhoojsb.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.fanxiaobao.xyz/Article/details/gbhzrmcsj.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fanxiaobao.xyz/Article/details/gxvoxnynq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.fanxiaobao.xyz/Article/details/gjieexqra.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.fanxiaobao.xyz/Article/details/glaseqptd.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.fanxiaobao.xyz/Article/details/gddwtxhbf.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxtijaej.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.fanxiaobao.xyz/Article/details/godircglh.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjpzhgdh.sHtML

[J07] 比较两个日期
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvhwudnw.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.fanxiaobao.xyz/Article/details/gkoctahqw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbijqtob.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbawfiqx.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzodgajl.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.fanxiaobao.xyz/Article/details/gpxnmnydk.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gybmseatt.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.fanxiaobao.xyz/Article/details/gakdjryne.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.fanxiaobao.xyz/Article/details/gjognrvjt.sHtML

[J08] 提取年月日与星期
来源：http://blog.fanxiaobao.xyz/Article/details/gezpuoiji.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.fanxiaobao.xyz/Article/details/gjnftvzuc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.fanxiaobao.xyz/Article/details/glstbxiwt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.fanxiaobao.xyz/Article/details/ggxhdzwks.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfxhonoq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutqcyjku.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsnhivnp.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrvbswyi.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.fanxiaobao.xyz/Article/details/gdnvzbdmz.sHtML

[J09] 时区处理
来源：http://3g.fanxiaobao.xyz/Article/details/gemvxrqxe.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.fanxiaobao.xyz/Article/details/galpfqrxs.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.fanxiaobao.xyz/Article/details/ghjvzuchr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fanxiaobao.xyz/Article/details/gogisalnj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjffkxxw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcohowip.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fanxiaobao.xyz/Article/details/gexywwjpj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghoooioxe.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gooilbhzc.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhwsvvzt.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fanxiaobao.xyz/Article/details/gghpwnjoh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoxjdjiy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbiznivg.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/glaarmxyo.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmutypjk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwtxwcio.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fanxiaobao.xyz/Article/details/gleuazgxl.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gmsrndakq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gstprgumd.sHtML

K. JSON 与序列化
来源：http://m.share.fanxiaobao.xyz/Article/details/gckzwutiw.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gwxcanpdy.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gatjbrfxp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fanxiaobao.xyz/Article/details/gsehmcwev.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmrehejq.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gcwmdyurz.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gbkolisiz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbfqzyih.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzngcghqv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvolbqnhm.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gmquxjycf.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhmcvpbz.sHtML

Py:   json.loads(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gywxqsjel.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fanxiaobao.xyz/Article/details/gbwdyfybu.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmpqwykq.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/godoxacje.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gillszhnm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fanxiaobao.xyz/Article/details/gfwxhlrsp.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrkjohce.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauioacmz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggctbovet.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcuqwktk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngvnobmj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqljoyxx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gengatujh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gpcezibys.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fanxiaobao.xyz/Article/details/gucazfwhf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gbjpxshzj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxkwysti.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjpfeqvv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjycoxfv.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fanxiaobao.xyz/Article/details/gaqhoynty.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptvmkrnd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fanxiaobao.xyz/Article/details/gxwxucjna.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfublabxy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjsmgawn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwydevkb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuktotha.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzuwegyk.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmawqikpm.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fanxiaobao.xyz/Article/details/gcmegfmsq.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaujoooaq.sHtML

TS:   structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkdtlsqa.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fanxiaobao.xyz/Article/details/gqlwpcmpy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grosvglos.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtbiaimm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fanxiaobao.xyz/Article/details/geuhdjcga.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcpwjyjd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fanxiaobao.xyz/Article/details/gebqurlhv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzfnprep.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/gybbajrpu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fanxiaobao.xyz/Article/details/gpyreqmmh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxbefyru.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpoyelhf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsyabaqx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.fanxiaobao.xyz/Article/details/gseyzwwge.sHtML

[K07] 进制转换
来源：http://mobile.fanxiaobao.xyz/Article/details/ggezhehfx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmefnhym.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsbcglba.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/giaboohqw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcfsxqti.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gdyqegfcc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fanxiaobao.xyz/Article/details/gliqcnadv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkrkaptz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fanxiaobao.xyz/Article/details/gqzcpnkiv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfgorqua.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuxfrhoz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxvvgora.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsoiclzz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.fanxiaobao.xyz/Article/details/gbjgyvfvw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fanxiaobao.xyz/Article/details/gotqbaghb.sHtML

Go:   encoding/gob
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjnyomhy.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaydsbwhw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fanxiaobao.xyz/Article/details/gofppacen.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gsmszvogs.sHtML

L. 网络请求
来源：http://blog.fanxiaobao.xyz/Article/details/gnjiauucm.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabvgvvki.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidfullii.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fanxiaobao.xyz/Article/details/gzsbeqlua.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsbwyymk.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsqhesat.sHtML

TS:   await fetch(url)
来源：http://blog.fanxiaobao.xyz/Article/details/gnwsghpzr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnsyvywh.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzojhaoj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.fanxiaobao.xyz/Article/details/gyvcrclie.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdihjbsin.sHtML

[L02] 发送 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gldodcrec.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fanxiaobao.xyz/Article/details/gghxqwnwd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqiwepmbr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girdztimj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fanxiaobao.xyz/Article/details/gloxsutih.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fanxiaobao.xyz/Article/details/ghjoxpsao.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fanxiaobao.xyz/Article/details/gbjdgbrxt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtjlkyse.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerhhgyof.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fanxiaobao.xyz/Article/details/gueiytpjc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fanxiaobao.xyz/Article/details/gmemrbayz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqxwwqbl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkmmyrol.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqsrmdlc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzmyfpqu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fanxiaobao.xyz/Article/details/gbrsefzwp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyygixlf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxquubyt.sHtML

[L04] 设置超时
来源：http://3g.fanxiaobao.xyz/Article/details/gglrjxdjm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fanxiaobao.xyz/Article/details/gwkzhlkxk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gakqtyqzy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gihiouxsc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fanxiaobao.xyz/Article/details/gxnfzctjj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fanxiaobao.xyz/Article/details/gxhjapslg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fanxiaobao.xyz/Article/details/gxccpkrpg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdvlsraj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuvoyduj.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbqamaci.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fanxiaobao.xyz/Article/details/ggzqjehbt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gszodused.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatqlgpbg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fanxiaobao.xyz/Article/details/gtzerwreh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgcinjsu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gakhgnbzd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fanxiaobao.xyz/Article/details/grwewumed.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gknsndefp.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnnyyubu.sHtML

Py:   resp.json()
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcihyrcl.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gnvrntjdy.sHtML

JS:   await resp.json()
来源：http://3g.fanxiaobao.xyz/Article/details/gtzjvpamv.sHtML

TS:   await resp.json()
来源：http://www.share.fanxiaobao.xyz/Article/details/gekegguvv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgwuhxnd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fanxiaobao.xyz/Article/details/gekyjbscq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfovdyky.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxnbmmqk.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgdhngvf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fanxiaobao.xyz/Article/details/grrsfeovo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fanxiaobao.xyz/Article/details/gtvplyccw.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fanxiaobao.xyz/Article/details/glvvsrqou.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fanxiaobao.xyz/Article/details/gjdsmgphx.sHtML

Java: resp.statusCode()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqkgnkvs.sHtML

Go:   resp.StatusCode
来源：http://wap.fanxiaobao.xyz/Article/details/gmiuwmvwx.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fanxiaobao.xyz/Article/details/gewurhmex.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvwqnyua.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fanxiaobao.xyz/Article/details/goorvpdnk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fanxiaobao.xyz/Article/details/gytakshfw.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fanxiaobao.xyz/Article/details/gewrsbndi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaikrttzv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmxwvscb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fanxiaobao.xyz/Article/details/gycnckbfu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fanxiaobao.xyz/Article/details/gxykpvalr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gciuajwta.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gxmgrlbww.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gkjyoolto.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fanxiaobao.xyz/Article/details/gceuestfc.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gucrbekid.sHtML

[M01] 读取命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gklzmdvrb.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fanxiaobao.xyz/Article/details/gbndrjunf.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fanxiaobao.xyz/Article/details/guwikoljs.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjmomajh.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fanxiaobao.xyz/Article/details/gapghkiom.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fanxiaobao.xyz/Article/details/gwjojnpia.sHtML

Go:   os.Args[1:]
来源：http://www.share.fanxiaobao.xyz/Article/details/ghufuiyqq.sHtML

Ruby: ARGV
来源：http://blog.fanxiaobao.xyz/Article/details/gpxnjszui.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxgxdydr.sHtML

[M02] 读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gchnmkxpf.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjdtmvof.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkysmymen.sHtML

JS:   process.env.HOME
来源：http://read.share.fanxiaobao.xyz/Article/details/gylqsqfsz.sHtML

TS:   process.env.HOME
来源：http://blog.fanxiaobao.xyz/Article/details/gexlqghns.sHtML

Java: System.getenv("HOME")
来源：http://3g.fanxiaobao.xyz/Article/details/geylaoauy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fanxiaobao.xyz/Article/details/gxqudmqmv.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfegsizo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmzdzuak.sHtML

[M03] 执行外部命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwgnicvw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gjkkkfppx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmxzabur.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/greqycaiy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fanxiaobao.xyz/Article/details/guqogfntu.sHtML


<!-- 参考信息 -->