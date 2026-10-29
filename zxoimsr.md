代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.fehbvm.com/Article/details/gsvqnodbd.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/giskttfgg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.zdbjq.cn/Article/details/gvralfxyx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fehbvm.com/Article/details/gcdlifqgk.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.hesvh.cn/Article/details/gprfdmzbn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gjcvmlaie.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.zdbjq.cn/Article/details/gejpwqtsm.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.zdbjq.cn/Article/details/gwkvynkwf.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gakwvmgrs.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.zdbjq.cn/Article/details/godtnkwbt.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.hesvh.cn/Article/details/guayyhjrf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.zdbjq.cn/Article/details/gbhhhyoay.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.fehbvm.com/Article/details/gahhkejga.sHtML

TS:   /error/gim
来源：http://www.share.hesvh.cn/Article/details/gomovqzcw.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.zdbjq.cn/Article/details/gvpvmidvy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.fehbvm.com/Article/details/gjctdhyhp.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.fehbvm.com/Article/details/gdoxgnfkw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.hesvh.cn/Article/details/gsspiiuky.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.zdbjq.cn/Article/details/geretbpln.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.zdbjq.cn/Article/details/grsrzbaym.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/gauouvvbc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.zdbjq.cn/Article/details/gladpwdgu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.zdbjq.cn/Article/details/ghkzeqbzq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/gnnymonbw.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.fehbvm.com/Article/details/gepnmkkrq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.fehbvm.com/Article/details/gayjthsqn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.zdbjq.cn/Article/details/gvaonhqti.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghgrqkdrx.sHtML

J. 日期与时间
来源：http://www.m.share.fehbvm.com/Article/details/gavfdsuym.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gasjpspqd.sHtML

[J01] 获取当前时间
来源：http://m.share.hesvh.cn/Article/details/gzffiapxn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.zdbjq.cn/Article/details/gvufauyda.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/gaatjyawe.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.fehbvm.com/Article/details/grhqtoxuj.sHtML

TS:   new Date();  Date.now()
来源：http://baike.fehbvm.com/Article/details/grjesmapj.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.fehbvm.com/Article/details/ghbvbmljb.sHtML

Go:   time.Now()
来源：http://read.share.zdbjq.cn/Article/details/ghrmosfel.sHtML

Ruby: Time.now
来源：http://m.share.fehbvm.com/Article/details/gurgwffnz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fehbvm.com/Article/details/gzopbwqwz.sHtML

[J02] 格式化输出
来源：http://wap.hesvh.cn/Article/details/gazkhchoz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.hesvh.cn/Article/details/gvjgpfgxy.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.zdbjq.cn/Article/details/gytusjpei.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.zdbjq.cn/Article/details/gpzdywlrq.sHtML

TS:   d.toISOString()
来源：http://www.blog.fehbvm.com/Article/details/gnbfibmqx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.hesvh.cn/Article/details/gofphqwdo.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.hesvh.cn/Article/details/gjkibvvyj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.hesvh.cn/Article/details/gxhkkgtvx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fehbvm.com/Article/details/glsfmuece.sHtML

[J03] 字符串解析为日期
来源：http://read.share.zdbjq.cn/Article/details/ggyaxxzug.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.fehbvm.com/Article/details/gcmeharjd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.zdbjq.cn/Article/details/ganmvhcxl.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gvfmdbjhp.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gqiddfbvn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gnfxsteuf.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gyxoegqvp.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gbeokfiyb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.zdbjq.cn/Article/details/gpdxhwzou.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.zdbjq.cn/Article/details/gvzpmamej.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.fehbvm.com/Article/details/grknckiyh.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.fehbvm.com/Article/details/gayodstmk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.hesvh.cn/Article/details/gnaybtsdz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.hesvh.cn/Article/details/gawbuzolj.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.hesvh.cn/Article/details/gesbgsaod.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gjenzjzbk.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.zdbjq.cn/Article/details/gldgrncdo.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.hesvh.cn/Article/details/gbbgzbuoa.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.fehbvm.com/Article/details/gtcyinquq.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.zdbjq.cn/Article/details/gnzpzrhos.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.hesvh.cn/Article/details/gbthkikkn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/gtmqcotfe.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/gsjwpwlfc.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.hesvh.cn/Article/details/gsncjhzlq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.zdbjq.cn/Article/details/gzihzwfqh.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.fehbvm.com/Article/details/gerapzujb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.fehbvm.com/Article/details/gqldibqhg.sHtML

[J06] 计算两时间之差
来源：http://blog.hesvh.cn/Article/details/gtofhsazd.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fehbvm.com/Article/details/ghdawpqtt.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.fehbvm.com/Article/details/gtvvmktbx.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.hesvh.cn/Article/details/gebwtjujl.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.zdbjq.cn/Article/details/gudmxytfk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.hesvh.cn/Article/details/gmwldebkk.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.fehbvm.com/Article/details/gxbfkmbnf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.hesvh.cn/Article/details/grmcsuzau.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.hesvh.cn/Article/details/geapquluc.sHtML

[J07] 比较两个日期
来源：http://read.share.zdbjq.cn/Article/details/gjnlslhvv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.fehbvm.com/Article/details/gepxhqlfa.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.hesvh.cn/Article/details/grltwrgwl.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.fehbvm.com/Article/details/gwhwxxzwo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.fehbvm.com/Article/details/grdipphbl.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.fehbvm.com/Article/details/gpymlwjml.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.fehbvm.com/Article/details/gaewsshaw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gxrkyiqbi.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/gxoatjwpm.sHtML

[J08] 提取年月日与星期
来源：http://read.share.zdbjq.cn/Article/details/gyeqpbxoi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.zdbjq.cn/Article/details/gmuknnbxs.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.hesvh.cn/Article/details/gnjnjdqew.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fehbvm.com/Article/details/gehkvzcpi.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.zdbjq.cn/Article/details/ghngzmxlo.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.fehbvm.com/Article/details/getfalejf.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.zdbjq.cn/Article/details/ghcsqdufs.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.fehbvm.com/Article/details/gcygznsez.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.fehbvm.com/Article/details/gvsogajgy.sHtML

[J09] 时区处理
来源：http://www.blog.hesvh.cn/Article/details/giheeffol.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.hesvh.cn/Article/details/gahcogwib.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fehbvm.com/Article/details/gxlyoqtfz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.zdbjq.cn/Article/details/guzjoozri.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/gqgpukfos.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.zdbjq.cn/Article/details/gneckrmdd.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.fehbvm.com/Article/details/gtexwrsfx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.zdbjq.cn/Article/details/gdrgjmwqt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fehbvm.com/Article/details/gfjnziudu.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.hesvh.cn/Article/details/gozttdifl.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.zdbjq.cn/Article/details/gsvsursvp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fehbvm.com/Article/details/graavvmgt.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.fehbvm.com/Article/details/gjadcgckz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gipvjxajj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.fehbvm.com/Article/details/grbqoxmpq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.zdbjq.cn/Article/details/gsntnlxwn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fehbvm.com/Article/details/gimthbypl.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fehbvm.com/Article/details/gkziivuqc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggmjtxvtn.sHtML

K. JSON 与序列化
来源：http://3g.hesvh.cn/Article/details/grkeamqrj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/goamvkyfl.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fehbvm.com/Article/details/gcbmjoiwo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/gpizhkccb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gaszdivub.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/gpxptejrp.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/gbcgvdtpk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.hesvh.cn/Article/details/gqtiqkhzi.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.zdbjq.cn/Article/details/gfrvsvpjt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.zdbjq.cn/Article/details/gadviyymm.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.zdbjq.cn/Article/details/gzyzzbpjz.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.zdbjq.cn/Article/details/gyyduhlgv.sHtML

Py:   json.loads(s)
来源：http://mobile.fehbvm.com/Article/details/gdbhorrid.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.hesvh.cn/Article/details/gfmjzdusz.sHtML

JS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gtqsphbdk.sHtML

TS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gdhlbqocf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fehbvm.com/Article/details/geherthfz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gdtmapofy.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gpgrlxhvg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.zdbjq.cn/Article/details/gbnrjotdf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.hesvh.cn/Article/details/gqtgwcdqe.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/gtgjmutyy.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gqzsazryu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gppfcscsu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gudprqjxm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.fehbvm.com/Article/details/gpjepjydp.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.fehbvm.com/Article/details/gcjzkzdxd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.zdbjq.cn/Article/details/gepcsapwp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.hesvh.cn/Article/details/gwxethopd.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.fehbvm.com/Article/details/gjwcjhbwm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fehbvm.com/Article/details/gikbjjvyd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.hesvh.cn/Article/details/glwngazxx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/gqknmdtus.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/gpxxkckmj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gdzvosohh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/ghgyyjfqp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/gjbloodjb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.hesvh.cn/Article/details/gkmwuhncj.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.hesvh.cn/Article/details/gwfjsciek.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.hesvh.cn/Article/details/gznbbdpbk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.zdbjq.cn/Article/details/gmyvbgnfq.sHtML

JS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/ghmjqvkzt.sHtML

TS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gwtxvjegb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.hesvh.cn/Article/details/glveilqmp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.hesvh.cn/Article/details/gozycgqdr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fehbvm.com/Article/details/gvchvfxlg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fehbvm.com/Article/details/gseylaxzq.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fehbvm.com/Article/details/gxpfwwroj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gkyrwvwym.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.hesvh.cn/Article/details/gmhdipmcv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/grqjdndqt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/geldyarqu.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.zdbjq.cn/Article/details/geordikiy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gpmixgsiz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/goahkixzj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gbzzhwjpz.sHtML

[K07] 进制转换
来源：http://www.blog.hesvh.cn/Article/details/gtkjgvhsl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gdocyqyyl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.hesvh.cn/Article/details/gnpsptcst.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gxptebqos.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/ghnmlhtrq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gwxqdoxgz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fehbvm.com/Article/details/gyadrdyej.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.hesvh.cn/Article/details/gfuutoqik.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gzirxzmho.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.zdbjq.cn/Article/details/gwexmicux.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.zdbjq.cn/Article/details/gejuskbjv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.zdbjq.cn/Article/details/ghwkdfzjj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/giyzpatjo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/geugzmfsg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fehbvm.com/Article/details/gkgjarmlc.sHtML

Go:   encoding/gob
来源：http://wap.zdbjq.cn/Article/details/gxkvnygbl.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/gyelafyvn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gqfszpocc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdeffvaee.sHtML

L. 网络请求
来源：http://www.blog.fehbvm.com/Article/details/gfuermgrr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnqhrupmk.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.hesvh.cn/Article/details/guptvjrzi.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.hesvh.cn/Article/details/gracvyqki.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fehbvm.com/Article/details/gjfctkkcl.sHtML

JS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gmcxnttdm.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/giztpxtoa.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.hesvh.cn/Article/details/gifktvucq.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fehbvm.com/Article/details/gmeyzwkwg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fehbvm.com/Article/details/gpdkiyrkv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.hesvh.cn/Article/details/gveehxcet.sHtML

[L02] 发送 POST JSON
来源：http://www.share.hesvh.cn/Article/details/ggoblvbzd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.hesvh.cn/Article/details/grhndhwqi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/goigipsun.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gbguohseg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gxptyihpk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gjfwxsajn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/gxserfbre.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/gsfivmnmn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fehbvm.com/Article/details/gudlwcbsu.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fehbvm.com/Article/details/ggzogbtdp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/gtszxtcze.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.hesvh.cn/Article/details/gidkzteji.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gksdaewal.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/ggmbgetzu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.zdbjq.cn/Article/details/gkcrxpjhu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gqdjfnlkm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.hesvh.cn/Article/details/gwupexjdb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gnndulycs.sHtML

[L04] 设置超时
来源：http://read.share.hesvh.cn/Article/details/girmflztq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.zdbjq.cn/Article/details/gnplzranf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/gfdjjptfv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gtdreollv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gvghkhsmt.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/getjybtma.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fehbvm.com/Article/details/grokldccc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.zdbjq.cn/Article/details/gholugogi.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/ganhueqgp.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.zdbjq.cn/Article/details/gtgzlqdzb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.zdbjq.cn/Article/details/gabusawgk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.hesvh.cn/Article/details/gdnzzlruu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gfizmfhfh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gxkpkqjuu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/getweawzn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.zdbjq.cn/Article/details/gqpzamnih.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fehbvm.com/Article/details/gpplufxqg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.hesvh.cn/Article/details/gtmisfpab.sHtML

[L06] 解析响应为 JSON
来源：http://blog.zdbjq.cn/Article/details/giqlzqnbk.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/glidbeekz.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/garhncvmh.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gfedjrzzf.sHtML

TS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/grpbkwdye.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/gchthndho.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/glsvuwbmq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.hesvh.cn/Article/details/ggjpfasqc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/gfxpbzaql.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gipvkuyay.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.hesvh.cn/Article/details/gfffggigw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/glsftvjfi.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gmxdehbkx.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gdvnvbpek.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/gzifiwcbd.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gwpdgkjju.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gqkxgfghi.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gtgrdbsth.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/glnnkrvso.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.hesvh.cn/Article/details/gvpxuwzvy.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/gzpjsiemm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gotfsmnqx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gqjnkfuvb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/guuzmvkai.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/guxewkwgs.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/gszacbhww.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gzdrygedv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwstgnlrn.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fehbvm.com/Article/details/geleqwrot.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqbrrhznh.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gjmrzposk.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/glarwrode.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/gyrqnvdfq.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/grarslncc.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gbmjhofiy.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/grflipznz.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/guvndmqiq.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/gzqnjjjgj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gbjmebhol.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gpopotfwi.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/geeimodnj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gvncwqkun.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gpysmnavz.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gaslkssdm.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gzubcnukj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/giibrrlik.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gvphvoyxx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/gxavanvix.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gyohdesqi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/goagwgntg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.zdbjq.cn/Article/details/gbbunnurd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gjxchelad.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/ggzydzyop.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gehytuncw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gzvyqikye.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gcisqjwgz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/ghptttfpe.sHtML


<!-- 参考信息 -->