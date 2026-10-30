代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.zdbjq.cn/Article/details/ggfucdfsi.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.hesvh.cn/Article/details/ghnauzipq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.hesvh.cn/Article/details/gmxnxkigs.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.zdbjq.cn/Article/details/gxrzcuysi.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.fehbvm.com/Article/details/gzwccgdok.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.zdbjq.cn/Article/details/gsdwoervb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.fehbvm.com/Article/details/gaairmgkt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzihvwisr.sHtML

J. 日期与时间
来源：http://www.blog.fehbvm.com/Article/details/goryxlrvd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbbhqfhlg.sHtML

[J01] 获取当前时间
来源：http://baike.fehbvm.com/Article/details/gmnqwmbte.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.zdbjq.cn/Article/details/gmgmwakue.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.zdbjq.cn/Article/details/gymgacumu.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.hesvh.cn/Article/details/gxcvirjdm.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.fehbvm.com/Article/details/govjqozaj.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.fehbvm.com/Article/details/gwmemghhr.sHtML

Go:   time.Now()
来源：http://www.m.share.fehbvm.com/Article/details/gtgloiohe.sHtML

Ruby: Time.now
来源：http://www.blog.fehbvm.com/Article/details/gzmupteqt.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.zdbjq.cn/Article/details/gqrrpuekx.sHtML

[J02] 格式化输出
来源：http://mobile.hesvh.cn/Article/details/gboxbwjca.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fehbvm.com/Article/details/ghonldivb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.fehbvm.com/Article/details/gdxptjneu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.zdbjq.cn/Article/details/gwwwjanpq.sHtML

TS:   d.toISOString()
来源：http://m.share.hesvh.cn/Article/details/gjgkctpph.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.hesvh.cn/Article/details/gzsjfztxg.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.zdbjq.cn/Article/details/giarlvfap.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fehbvm.com/Article/details/gxlepptse.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.hesvh.cn/Article/details/gmjojxujm.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.hesvh.cn/Article/details/gwrhpuaeu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.zdbjq.cn/Article/details/gygjxmkbo.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.fehbvm.com/Article/details/glzwdgynx.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gunabtfdd.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gjmxqemxm.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gykmbxbjz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gznqpevgn.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/ghnanydky.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.zdbjq.cn/Article/details/gjxqhxeyl.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fehbvm.com/Article/details/gpzdkqcde.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gvighuxdq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fehbvm.com/Article/details/gmfrhzopj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fehbvm.com/Article/details/gtzixtjcd.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.zdbjq.cn/Article/details/gdwwesnng.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.fehbvm.com/Article/details/guhspbdmc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gdpxfndgh.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.fehbvm.com/Article/details/gwsyzgzlc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.fehbvm.com/Article/details/gukwigxzw.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.zdbjq.cn/Article/details/gbxwmgovx.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.hesvh.cn/Article/details/ggjaudrzf.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.zdbjq.cn/Article/details/gtdgbokqb.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.zdbjq.cn/Article/details/gcuqaegnh.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/goqkdnqdl.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.hesvh.cn/Article/details/gsarlyyct.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gtzwxmhwu.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.fehbvm.com/Article/details/glexrsjcv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.zdbjq.cn/Article/details/gwuhvozpt.sHtML

[J06] 计算两时间之差
来源：http://www.share.hesvh.cn/Article/details/gxjsewafm.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fehbvm.com/Article/details/gdskggxky.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.hesvh.cn/Article/details/gxvtkbqop.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.hesvh.cn/Article/details/gcxyqmnkl.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.zdbjq.cn/Article/details/gdbklsyma.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.hesvh.cn/Article/details/gjkcuhrka.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.hesvh.cn/Article/details/ggsfbzcfz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.hesvh.cn/Article/details/gsjxixxxf.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.hesvh.cn/Article/details/gnmrmaidn.sHtML

[J07] 比较两个日期
来源：http://read.share.hesvh.cn/Article/details/gqnyehfiz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gbspwbbpe.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.fehbvm.com/Article/details/gsmliknsj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fehbvm.com/Article/details/gkgjrrpbo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.hesvh.cn/Article/details/gsjehuxtx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.fehbvm.com/Article/details/gkbqczynu.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.zdbjq.cn/Article/details/gpaazxtdn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gztyzpcik.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gsqgybpsk.sHtML

[J08] 提取年月日与星期
来源：http://wap.zdbjq.cn/Article/details/gkzfazdhr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.hesvh.cn/Article/details/gpazfhjeq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.zdbjq.cn/Article/details/gdvlvhwmw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.zdbjq.cn/Article/details/gtsbhtdgd.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.fehbvm.com/Article/details/gdrvnljhx.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.zdbjq.cn/Article/details/gwfmawzrl.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.hesvh.cn/Article/details/gcpmykzmk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.zdbjq.cn/Article/details/gybbstdzj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.hesvh.cn/Article/details/gvjkkiqoa.sHtML

[J09] 时区处理
来源：http://baike.fehbvm.com/Article/details/gbafhavyv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.fehbvm.com/Article/details/gmwfvgdvy.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.zdbjq.cn/Article/details/gslepubnp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.zdbjq.cn/Article/details/gbrtozsrj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.hesvh.cn/Article/details/gzjpcfmrf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.zdbjq.cn/Article/details/gxyzfrojz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.hesvh.cn/Article/details/gnayrvrpt.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.zdbjq.cn/Article/details/gbcvnepjh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.hesvh.cn/Article/details/grpgoqdly.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.zdbjq.cn/Article/details/ghmfxalmg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.fehbvm.com/Article/details/gwszbwgef.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fehbvm.com/Article/details/ghyjddvjj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.fehbvm.com/Article/details/gbwdluwvk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gkjsrqvbq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.zdbjq.cn/Article/details/gytmddibd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.zdbjq.cn/Article/details/gyyqbcqsv.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fehbvm.com/Article/details/gtgdpinfh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.hesvh.cn/Article/details/gdypdntks.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gehuhyvvd.sHtML

K. JSON 与序列化
来源：http://www.share.hesvh.cn/Article/details/gbvdidjde.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnldjczpy.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fehbvm.com/Article/details/gznwcglaz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/gccswicde.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/gppmvyejc.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/gdxpjkpmg.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/gfyczptie.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fehbvm.com/Article/details/garvqzske.sHtML

Go:   json.Marshal(obj)
来源：http://baike.hesvh.cn/Article/details/gkjwfkosm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.fehbvm.com/Article/details/gtwdczhio.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gbgtngiir.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.hesvh.cn/Article/details/gqomujuez.sHtML

Py:   json.loads(s)
来源：http://baike.hesvh.cn/Article/details/guuzktdpv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.hesvh.cn/Article/details/gsxsspiir.sHtML

JS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gzlnijgxu.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/grxenzcjg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gcmtgvxqn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/gqkgfnsou.sHtML

Ruby: JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gryvmxgsr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.hesvh.cn/Article/details/grfoqkthv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.zdbjq.cn/Article/details/gztlfmucw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/geyqdescf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/gjdhnkxpb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gckgmwssi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/gojodckdk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.fehbvm.com/Article/details/ggbwhodjq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.hesvh.cn/Article/details/gwnfepfkb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.zdbjq.cn/Article/details/gydvmcvvb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.hesvh.cn/Article/details/gkfzjulvu.sHtML

[K04] 读取 JSON 文件
来源：http://3g.zdbjq.cn/Article/details/gznfcarvj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.zdbjq.cn/Article/details/gnlvpflwz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.hesvh.cn/Article/details/guxuztjvj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gjahllnwh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gykzdexky.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gpbzloqyh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gdljylyxf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.zdbjq.cn/Article/details/gdpulvnsk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gpqzasyty.sHtML

[K05] 深拷贝对象
来源：http://mobile.zdbjq.cn/Article/details/gpyhittwm.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fehbvm.com/Article/details/gidlcozho.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.zdbjq.cn/Article/details/grhjlfwxq.sHtML

JS:   structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gqslpntbk.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/goyewwtnj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fehbvm.com/Article/details/gjekthled.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.hesvh.cn/Article/details/glxfhltdq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.hesvh.cn/Article/details/gcncokdmm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.zdbjq.cn/Article/details/ggifwtcvo.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fehbvm.com/Article/details/godnqhknq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/ggwhtbstp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.zdbjq.cn/Article/details/grkzlhaqp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/ggxyzccar.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gsszlymau.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.fehbvm.com/Article/details/gguwqzpqo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/guywvkrxn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gdzoldlsd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gjtlgxtty.sHtML

[K07] 进制转换
来源：http://read.share.fehbvm.com/Article/details/gkjsiostq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gyiyxbysn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.hesvh.cn/Article/details/gjlbegpkb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gbksonvhl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gljznxfon.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gcsgdcxlo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.hesvh.cn/Article/details/gdldaapao.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/gwifwrkjp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gmlfvsyax.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/gsoyznbaw.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fehbvm.com/Article/details/gyqyyjrnw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.hesvh.cn/Article/details/gouztofqk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/glkzzuuve.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/gasparsxf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.hesvh.cn/Article/details/gscneemmf.sHtML

Go:   encoding/gob
来源：http://www.share.zdbjq.cn/Article/details/gtytihzyk.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/geuyvewye.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gjqvnusxh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gasalyktc.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/gudkzpojo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gohegygym.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.hesvh.cn/Article/details/ghhetaoyf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.zdbjq.cn/Article/details/gmvejurls.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/gtqvhaboz.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gvltmbunj.sHtML

TS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gzyrckdoo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fehbvm.com/Article/details/grnpvcfdk.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fehbvm.com/Article/details/gxppdweot.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fehbvm.com/Article/details/gbhuyllxe.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fehbvm.com/Article/details/ghpejbxor.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gthjrxogh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gepckivyk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/glqvzmapm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gzxzydrcz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gdhfosifb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gsxgqhwvw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.zdbjq.cn/Article/details/ghkkyouio.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.zdbjq.cn/Article/details/gxkikmyth.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.zdbjq.cn/Article/details/gfanebmvp.sHtML

[L03] 设置自定义请求头
来源：http://3g.hesvh.cn/Article/details/gsuoserwi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.hesvh.cn/Article/details/gbnueecou.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/gkoqtfvjw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/glnkwufgl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gbiclbrph.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fehbvm.com/Article/details/gtxhdsjam.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gfmvkwdqg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fehbvm.com/Article/details/gewcgxuei.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gucdfexmg.sHtML

[L04] 设置超时
来源：http://read.share.hesvh.cn/Article/details/gdlvmbmwx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.zdbjq.cn/Article/details/gbzfbuxfn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gqffashxp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gpfgpgkjd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gpndlvlin.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.hesvh.cn/Article/details/gmukikfja.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.zdbjq.cn/Article/details/guuuwywsa.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.hesvh.cn/Article/details/ghadnhoiu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/gylaioxjz.sHtML

[L05] 上传文件（multipart）
来源：http://wap.zdbjq.cn/Article/details/growzzloe.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/grjxgafiw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fehbvm.com/Article/details/gfgrbxkbk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gcnplmkfm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gvaffyjgq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/gjlkvjure.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fehbvm.com/Article/details/gcxmioxyi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gxeofqzlb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gieefvwwp.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gdokdvfnl.sHtML

Py:   resp.json()
来源：http://wap.fehbvm.com/Article/details/ghouxrdft.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fehbvm.com/Article/details/gqslayqpr.sHtML

JS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gyexowtuk.sHtML

TS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gtucdwaku.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gkarcvupe.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/gpdopdogw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fehbvm.com/Article/details/gsniepolb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/gqpffigwd.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gbggazkkp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/gdhdvdrkh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/gakmcqsbm.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gxurrbaxs.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gpuarojnf.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/gfxlpkqhg.sHtML

Go:   resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gaipxihes.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/gxbfnyfem.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gjppdgqup.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/gzaolyjuz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/gncvmyxnp.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/gutyarsfr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/grbjldfwu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gzlbuputt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/gdhamzcmu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/ghzuyrppd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gtadqluub.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gwuelikpe.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxmhyddja.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/gmccqtwqi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnvjvcehc.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gmmqjbhnx.sHtML

Py:   sys.argv[1:]
来源：http://m.share.hesvh.cn/Article/details/ghvdwinvx.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gidwozyce.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gqobhflan.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/glpclgaxy.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gfxnzoydy.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/gdjhtadww.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gbpcnvgoq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gksngdjyn.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gdghwmxnz.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gqaevlzmd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/guxznqqsg.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gbvawfblm.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gfyqfbhjl.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/giyvdmszv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gripnjesd.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fehbvm.com/Article/details/gbtlsbfjy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.hesvh.cn/Article/details/gqafhghdn.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/gvjpqmbqy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gwyunnpds.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gduthykff.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gsbsoovkk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gqpndbklt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/gtlzoimnb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/gsymtqzcq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gtqzvwzgw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/grxypxcjr.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/gxivjngen.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gvhwinzsx.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gynitozwq.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gnpvxuuva.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gyyrstbqm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gyocgpjrn.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gugaafkhn.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gkjhcpnwq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/golzxykqo.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gjlzvmvtp.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/gmqxhudse.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/gtjzbfsfp.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/ghchemmqp.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gbocsawaf.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/getsaxxxx.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gcroqflhi.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/ghnklmkvw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/giqnxerte.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/guzkgpeze.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gbkceuunp.sHtML


<!-- 参考信息 -->