代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://wap.hesvh.cn/Article/details/gelflncnr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.zdbjq.cn/Article/details/gyjiggwwn.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gjbodohet.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.zdbjq.cn/Article/details/gsfoyyiqh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fehbvm.com/Article/details/gzgnetpbz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/glaopjnlt.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.zdbjq.cn/Article/details/gdklnlfhq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/gjzcqhokr.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.hesvh.cn/Article/details/gkfbscctg.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gpygqinvy.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.fehbvm.com/Article/details/gktjbdbku.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fehbvm.com/Article/details/gecnhdnlx.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gbvbnonmy.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.zdbjq.cn/Article/details/gjcusirsu.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fehbvm.com/Article/details/gwhpgilbr.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.fehbvm.com/Article/details/gsjlaybxd.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.fehbvm.com/Article/details/gaoioevvc.sHtML

TS:   /error/gim
来源：http://blog.hesvh.cn/Article/details/gailbcviu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.zdbjq.cn/Article/details/gmaxvljfh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.zdbjq.cn/Article/details/guozptojf.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.zdbjq.cn/Article/details/gasgljftm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.fehbvm.com/Article/details/gihrdeodr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fehbvm.com/Article/details/glqtyxbls.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.zdbjq.cn/Article/details/gnmxgfocl.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.hesvh.cn/Article/details/gbatplhhh.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fehbvm.com/Article/details/grcrdxpoc.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gsmnmtwzs.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/gwzrnyzzb.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.zdbjq.cn/Article/details/gynqlfjyr.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.hesvh.cn/Article/details/glvdijifr.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/gihcxvymb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gebdlsrua.sHtML

J. 日期与时间
来源：http://www.share.hesvh.cn/Article/details/gjggcgiud.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/guyvusmwo.sHtML

[J01] 获取当前时间
来源：http://read.share.fehbvm.com/Article/details/gwsgulmaf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.zdbjq.cn/Article/details/gpeiqipbf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.zdbjq.cn/Article/details/gfzmkskdw.sHtML

JS:   new Date();  Date.now()
来源：http://wap.zdbjq.cn/Article/details/gxqzjwqgx.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gysybswec.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.fehbvm.com/Article/details/gzqjmpgjo.sHtML

Go:   time.Now()
来源：http://wap.fehbvm.com/Article/details/gwgjggsfj.sHtML

Ruby: Time.now
来源：http://baike.zdbjq.cn/Article/details/gdtcaymmj.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.hesvh.cn/Article/details/guduyrdse.sHtML

[J02] 格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/guaoasquc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.zdbjq.cn/Article/details/gnqduhpdd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fehbvm.com/Article/details/gulwgqtzo.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.zdbjq.cn/Article/details/gnynxnmfc.sHtML

TS:   d.toISOString()
来源：http://mobile.fehbvm.com/Article/details/gxpenlnap.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.hesvh.cn/Article/details/glqjloqdz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.fehbvm.com/Article/details/gifxkwdxu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fehbvm.com/Article/details/gjnudklrh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.hesvh.cn/Article/details/gbizxannn.sHtML

[J03] 字符串解析为日期
来源：http://3g.zdbjq.cn/Article/details/gnrteeyol.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fehbvm.com/Article/details/gjqnwgzop.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.fehbvm.com/Article/details/gbviddrli.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gvurvmqin.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gasexfvmd.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/glzfytpkq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gexiierek.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gymyrkjwk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.hesvh.cn/Article/details/gqjitthhx.sHtML

[J04] 时间戳与日期互转
来源：http://baike.zdbjq.cn/Article/details/gwadegywl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.zdbjq.cn/Article/details/gvbibpxdo.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.hesvh.cn/Article/details/gmfwzktio.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.fehbvm.com/Article/details/gbwqbaqnw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.zdbjq.cn/Article/details/gnzobwyvm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.fehbvm.com/Article/details/gtdtwafwg.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.hesvh.cn/Article/details/grbvylcmt.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.fehbvm.com/Article/details/gsnoongob.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.zdbjq.cn/Article/details/ggawtpymc.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.zdbjq.cn/Article/details/gfoodfhkf.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.hesvh.cn/Article/details/gxoiqlmpg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.zdbjq.cn/Article/details/gzqbcfdgq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/gyolhmbxz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.hesvh.cn/Article/details/gngnwiowm.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.zdbjq.cn/Article/details/gvnupyxss.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.fehbvm.com/Article/details/gbisjquza.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.hesvh.cn/Article/details/ggjbpkyoj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.fehbvm.com/Article/details/gqcuiwird.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.zdbjq.cn/Article/details/gixotmhfd.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.zdbjq.cn/Article/details/gfqwndmsb.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.fehbvm.com/Article/details/glcuazjwe.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.fehbvm.com/Article/details/gafjltohz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.hesvh.cn/Article/details/gwnxpdlli.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fehbvm.com/Article/details/gfynjhdvq.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.hesvh.cn/Article/details/gnkddzfzk.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fehbvm.com/Article/details/gakqxwipe.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.fehbvm.com/Article/details/gbbekewhj.sHtML

[J07] 比较两个日期
来源：http://www.m.share.hesvh.cn/Article/details/gvasqnvwq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gerxtzlus.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.hesvh.cn/Article/details/gewbbbxpt.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.fehbvm.com/Article/details/gyoozuijd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.fehbvm.com/Article/details/giacjrdlc.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.zdbjq.cn/Article/details/gcifruiun.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.hesvh.cn/Article/details/gzmnhpwzy.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/gnqktpjsv.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/ggaoqyhbd.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.hesvh.cn/Article/details/gixfnbqmh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.hesvh.cn/Article/details/gnsqppktc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.zdbjq.cn/Article/details/gpkroonrn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.zdbjq.cn/Article/details/gqzslgwsf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.fehbvm.com/Article/details/gzvjrxckk.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.zdbjq.cn/Article/details/gfapjczjj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.fehbvm.com/Article/details/gqidhtynn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.zdbjq.cn/Article/details/griwrzxks.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.zdbjq.cn/Article/details/ggntvumfw.sHtML

[J09] 时区处理
来源：http://m.share.fehbvm.com/Article/details/grseqhnap.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.zdbjq.cn/Article/details/gjqwzgrwf.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.hesvh.cn/Article/details/goulcyjnk.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/gmsaqqodp.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/gvlgjqldy.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.zdbjq.cn/Article/details/gghdaeiol.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fehbvm.com/Article/details/gollihzcn.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.hesvh.cn/Article/details/gquwhxqky.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.zdbjq.cn/Article/details/gfzooaibd.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.zdbjq.cn/Article/details/gpspjrpkc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.hesvh.cn/Article/details/gpqhsauos.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.hesvh.cn/Article/details/giihjgsyl.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.fehbvm.com/Article/details/gonyhxugm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.fehbvm.com/Article/details/guaqldoqy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fehbvm.com/Article/details/gkecjkisa.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.hesvh.cn/Article/details/gjajzumgt.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.fehbvm.com/Article/details/gxaurxcmv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.hesvh.cn/Article/details/gjmprnwlx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grcrpwhyy.sHtML

K. JSON 与序列化
来源：http://m.share.fehbvm.com/Article/details/gpnbxcrpq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghqwflgnh.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.zdbjq.cn/Article/details/gnlllzrxs.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fehbvm.com/Article/details/grkdhkgwt.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/gbcpeathv.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gcftlkmuu.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/giaqnzngy.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.zdbjq.cn/Article/details/gmvzimsnk.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.hesvh.cn/Article/details/gabqbezcd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.zdbjq.cn/Article/details/geucjefrm.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.hesvh.cn/Article/details/gxsoxxjfe.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.zdbjq.cn/Article/details/gbetoyaky.sHtML

Py:   json.loads(s)
来源：http://wap.zdbjq.cn/Article/details/gmoucfpwc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.zdbjq.cn/Article/details/gadwxixiq.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gyuauqtkg.sHtML

TS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gbxwgucdu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.hesvh.cn/Article/details/gsvezguvd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/giksrejmz.sHtML

Ruby: JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gmfccunwi.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.zdbjq.cn/Article/details/gotpbmubc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.zdbjq.cn/Article/details/gxkybeofp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/grrcthgbi.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gjurcbqnp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gskskiucb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gmehdmfwa.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.hesvh.cn/Article/details/gayhoskqb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.hesvh.cn/Article/details/gwkwgtkdi.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fehbvm.com/Article/details/gfygrbesn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.zdbjq.cn/Article/details/gebqafmbd.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.hesvh.cn/Article/details/gcwlxajpg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.zdbjq.cn/Article/details/gxptrqpcg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.hesvh.cn/Article/details/gisjyilcb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gobpfrjva.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gfzazbvbj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gghykdjdx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gcjyibmsw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.zdbjq.cn/Article/details/ghkvivbhz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gydyxegkm.sHtML

[K05] 深拷贝对象
来源：http://www.share.fehbvm.com/Article/details/gakoswukb.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.zdbjq.cn/Article/details/gsbuuvzao.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fehbvm.com/Article/details/gaszacjhe.sHtML

JS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gflqwnihz.sHtML

TS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gxjmnhmyp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/ggqfhdutc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.fehbvm.com/Article/details/gzqkputjx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.zdbjq.cn/Article/details/glqmfylda.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.hesvh.cn/Article/details/gonwmhfil.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.hesvh.cn/Article/details/gmargzzhq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.hesvh.cn/Article/details/guzonpain.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fehbvm.com/Article/details/gkfvrwbmb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gebzvpqpn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gwqhjrfms.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.hesvh.cn/Article/details/ggwyacige.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/giadftrxb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/grdiklibh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gkkounpmh.sHtML

[K07] 进制转换
来源：http://blog.hesvh.cn/Article/details/goqlqqgko.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gpvksvzcr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.hesvh.cn/Article/details/gkejxcfss.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/guralysrf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gkfacvtin.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gsxjjtpxw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.zdbjq.cn/Article/details/gqqjkiiny.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fehbvm.com/Article/details/gqnuufopt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gmigfpnfl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.zdbjq.cn/Article/details/gbeajiims.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/gzdgrpral.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.hesvh.cn/Article/details/gqozmrfey.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/ghhgnqzfg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gfetyhvwt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.hesvh.cn/Article/details/gazwuoiru.sHtML

Go:   encoding/gob
来源：http://baike.zdbjq.cn/Article/details/ggxuyjyka.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fehbvm.com/Article/details/gsrdfggcg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gmpdzraxh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpirggeaq.sHtML

L. 网络请求
来源：http://3g.zdbjq.cn/Article/details/glqpnubfr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqoetwywy.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.zdbjq.cn/Article/details/gmhhmyefh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.hesvh.cn/Article/details/gzgudopoo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.zdbjq.cn/Article/details/gsmveloyw.sHtML

JS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/ghccevkjb.sHtML

TS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gaswmcmue.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.zdbjq.cn/Article/details/gzjnfhvwc.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/gxkqxmaru.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fehbvm.com/Article/details/gtkqnlkih.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.zdbjq.cn/Article/details/gvwnyimoc.sHtML

[L02] 发送 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gpazzrzgj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.hesvh.cn/Article/details/gtuxvinxl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fehbvm.com/Article/details/guabolyws.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gwvupqgio.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gpbtenkxx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gigritagp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.hesvh.cn/Article/details/gthyepcyu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.hesvh.cn/Article/details/glcyujzwf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/gsldqfpaw.sHtML

[L03] 设置自定义请求头
来源：http://blog.fehbvm.com/Article/details/gcbyhukkq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.zdbjq.cn/Article/details/gpaunctcx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.hesvh.cn/Article/details/gbmdwegny.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/ggndzwage.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gxpwcklwb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.zdbjq.cn/Article/details/gnupkvggy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/ggbtaeira.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.hesvh.cn/Article/details/gdqfdltlo.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/ghynlpkqd.sHtML

[L04] 设置超时
来源：http://blog.fehbvm.com/Article/details/gairifoqm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gmqvwfusz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gdrjojpna.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gmelmnjum.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gpijslmrm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.hesvh.cn/Article/details/gkfmvmtkp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/gjeytejwd.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.hesvh.cn/Article/details/gdawmgccs.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/guyjyvhal.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/gbfjmymax.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.hesvh.cn/Article/details/gbuqvfydy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fehbvm.com/Article/details/gqsvacpna.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gjfflzkdr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gexgutsgh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gviqdyuwg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fehbvm.com/Article/details/gyfacgbcy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gotfqwtrc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/gxkhwpfio.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/grvjfshlq.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gphmmelfk.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/gwaykkilu.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gcaheuzah.sHtML

TS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/ggjezoojl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gclfqqahr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fehbvm.com/Article/details/gmhkmflsq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/gzojpkseo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gyojpbxql.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/godrrqquk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/gqytyfhaz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.hesvh.cn/Article/details/gpspaijos.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gomxscglt.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gmvpskyva.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/gzqqkcops.sHtML

Go:   resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gmdmrchqs.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/glzqpgolh.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gqaaalwzh.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gmeuncxsn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/guwxwxivd.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gpbiwonyq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gnazljcth.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/ggxglntbw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/gklnpzpuy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gryhmzpvb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gztzzabpu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.hesvh.cn/Article/details/grmrrlbmo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwxoinxhf.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/gbsswtdns.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggmbuiqkp.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gyhhqyeuc.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gemkyvmem.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gmrcwmmhk.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gnnyaaogp.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gaydalhrr.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gxdwujjpe.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/gtjbzlrwq.sHtML

Ruby: ARGV
来源：http://www.share.hesvh.cn/Article/details/gfrybizuk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gqwhogehu.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/ghobwaatu.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/gpzzxatwq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gifsxitnu.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gkcxbidoi.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gklpkzukt.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gwpdrmqrk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/guyumacad.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/geampfoba.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/gmedpkqzt.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/grpwsvkaj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gkcrfmqqt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gfacqpjtl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gvclygucu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/ggokptzre.sHtML


<!-- 参考信息 -->