代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gacbzwfph.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.hesvh.cn/Article/details/gmtoxtmzh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.zdbjq.cn/Article/details/giyxywtrg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/ggzbtnvev.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.zdbjq.cn/Article/details/gvgclkwyj.sHtML

TS:   /error/gim
来源：http://m.share.fehbvm.com/Article/details/gzqjnqhat.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.zdbjq.cn/Article/details/gkxahtvrm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.fehbvm.com/Article/details/gimecsbsk.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.fehbvm.com/Article/details/gpltgxezq.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.zdbjq.cn/Article/details/gowocepbt.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.fehbvm.com/Article/details/glaomkhdf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.fehbvm.com/Article/details/gitnhkovc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.hesvh.cn/Article/details/gigcglgba.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/gaztvimuc.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fehbvm.com/Article/details/glnxsniuu.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.zdbjq.cn/Article/details/gfrflfliy.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.zdbjq.cn/Article/details/ghlusbwnz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.zdbjq.cn/Article/details/gyummfrde.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.zdbjq.cn/Article/details/gckrfdphe.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gufvneqld.sHtML

J. 日期与时间
来源：http://blog.fehbvm.com/Article/details/gzinttiep.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghdcrejvn.sHtML

[J01] 获取当前时间
来源：http://wap.zdbjq.cn/Article/details/gohpngawv.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.zdbjq.cn/Article/details/guqlxtpqo.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.hesvh.cn/Article/details/gvtwghovg.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.fehbvm.com/Article/details/gffogbcob.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/grcyexygd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.hesvh.cn/Article/details/gbbmwysxk.sHtML

Go:   time.Now()
来源：http://baike.zdbjq.cn/Article/details/gvcixgyhn.sHtML

Ruby: Time.now
来源：http://baike.hesvh.cn/Article/details/gggwgiogw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.fehbvm.com/Article/details/gvnhpqwyo.sHtML

[J02] 格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gvwqbwcbg.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/gvjaxdayj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fehbvm.com/Article/details/gtluxdysm.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fehbvm.com/Article/details/gqdksmvbu.sHtML

TS:   d.toISOString()
来源：http://blog.fehbvm.com/Article/details/gmrkqyonl.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.hesvh.cn/Article/details/gumxyybrc.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.zdbjq.cn/Article/details/gkzlmvmhl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/ghixcmvbl.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.zdbjq.cn/Article/details/gtznaztlz.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.hesvh.cn/Article/details/gdxqxcjhj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.zdbjq.cn/Article/details/gknaynxyu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.hesvh.cn/Article/details/gabixpkms.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gjhacgdnx.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gsethztvn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gmkibftyt.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gtxwiypcm.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gqjzuudxk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.zdbjq.cn/Article/details/gqqpdnvqk.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.fehbvm.com/Article/details/gsecacyvk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.fehbvm.com/Article/details/gwjsquyks.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fehbvm.com/Article/details/gdjnnzvrm.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.fehbvm.com/Article/details/gysqrtuid.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.zdbjq.cn/Article/details/gxjvkujki.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.hesvh.cn/Article/details/geicjgqdu.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.hesvh.cn/Article/details/gjcsdixvq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.zdbjq.cn/Article/details/gmwerwhaj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.fehbvm.com/Article/details/ghixwrhph.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.zdbjq.cn/Article/details/gnphzavbr.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.zdbjq.cn/Article/details/gxpokcqaq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.fehbvm.com/Article/details/gonckjtfg.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.zdbjq.cn/Article/details/gyrggctpz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fehbvm.com/Article/details/gntxbqyqd.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.zdbjq.cn/Article/details/gozrsblnv.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.zdbjq.cn/Article/details/gaaxcqzcf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.hesvh.cn/Article/details/gxtgfpqgx.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.fehbvm.com/Article/details/gqpzbrfig.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.hesvh.cn/Article/details/gmirmugqk.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.zdbjq.cn/Article/details/gokcsbyjy.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fehbvm.com/Article/details/gxpcyugwe.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.zdbjq.cn/Article/details/gbcgswqyb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.hesvh.cn/Article/details/gfhvxyemi.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.zdbjq.cn/Article/details/gocglexax.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.fehbvm.com/Article/details/glvlxbtcb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.fehbvm.com/Article/details/gihudbify.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.fehbvm.com/Article/details/gwzbqmvwb.sHtML

[J07] 比较两个日期
来源：http://www.share.hesvh.cn/Article/details/gjoxedlkh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gpmbthapb.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.hesvh.cn/Article/details/gremlupwb.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.hesvh.cn/Article/details/gebmtxwxg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.hesvh.cn/Article/details/gelbthhxg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.hesvh.cn/Article/details/gxdefgqjh.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.hesvh.cn/Article/details/gnggnukdw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gdryizwov.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/gjqrittnn.sHtML

[J08] 提取年月日与星期
来源：http://blog.hesvh.cn/Article/details/gghnfyqoa.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fehbvm.com/Article/details/gadkcfkqn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.zdbjq.cn/Article/details/grctaiygd.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.fehbvm.com/Article/details/goizgrlga.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.fehbvm.com/Article/details/gdoovighi.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.fehbvm.com/Article/details/gspeolxan.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.zdbjq.cn/Article/details/gsquxnwzy.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.hesvh.cn/Article/details/geucawbfx.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.fehbvm.com/Article/details/gqpmdamjw.sHtML

[J09] 时区处理
来源：http://www.share.hesvh.cn/Article/details/gnozonsdk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fehbvm.com/Article/details/gxrxopjjg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.zdbjq.cn/Article/details/gveofhmxn.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.zdbjq.cn/Article/details/gydzsvyym.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/gmhkfxeqx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.hesvh.cn/Article/details/gatlgiikc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.fehbvm.com/Article/details/ghkuklsjg.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.zdbjq.cn/Article/details/gtdwrxinf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.hesvh.cn/Article/details/gglanowsm.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.zdbjq.cn/Article/details/gafftaodl.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.hesvh.cn/Article/details/gqlgprybp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.hesvh.cn/Article/details/gkyqnsmfj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.hesvh.cn/Article/details/gqawnoncx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.hesvh.cn/Article/details/ggvovjxbf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fehbvm.com/Article/details/gizbnuhzx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.zdbjq.cn/Article/details/gqzbiprgh.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.hesvh.cn/Article/details/gtkzwjjxt.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gvaetpzps.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjaqfwtbe.sHtML

K. JSON 与序列化
来源：http://blog.hesvh.cn/Article/details/gohzmhfjz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxmsblytw.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.fehbvm.com/Article/details/ggvtqlzhw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gjssnpohs.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/gsntvjhxl.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.hesvh.cn/Article/details/gxfvddbau.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/glhqvanzk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.hesvh.cn/Article/details/girigovhb.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.zdbjq.cn/Article/details/gqhecdqam.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fehbvm.com/Article/details/gddaqrgzz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.hesvh.cn/Article/details/glpmtsbkp.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.hesvh.cn/Article/details/gqmbppsjo.sHtML

Py:   json.loads(s)
来源：http://www.share.fehbvm.com/Article/details/gayylayey.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.zdbjq.cn/Article/details/guatscnkr.sHtML

JS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gfhiyqqdc.sHtML

TS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gnhtdutfp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gpcqbmefp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/getacqcfi.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gtwkwliav.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.fehbvm.com/Article/details/glqspynai.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fehbvm.com/Article/details/ghmuebivv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/gaecfxxcw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gdqxgjgxh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gsiwucuss.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/geohhkpgl.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.zdbjq.cn/Article/details/gomzebunx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.zdbjq.cn/Article/details/golmqruiq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.zdbjq.cn/Article/details/gwxonrcio.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.hesvh.cn/Article/details/gwzmhxtyf.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.hesvh.cn/Article/details/goqkgkgsx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.zdbjq.cn/Article/details/gaqugzpsd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.hesvh.cn/Article/details/gdoqjzvgi.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gtuleovwo.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/gwgyiemas.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.fehbvm.com/Article/details/gehuhcxkl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gxftsfxqx.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gpugcdrvz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gtynzugtj.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/gfenaxmah.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.fehbvm.com/Article/details/gdbnkfsxo.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.hesvh.cn/Article/details/gatnvuxte.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gmylysnbg.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gbbpcliny.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.zdbjq.cn/Article/details/gqnodcpcz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.fehbvm.com/Article/details/gimgbjlhp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gyogpctey.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/gijuxqyih.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fehbvm.com/Article/details/gezdpwqtq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gbidcfsbp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.zdbjq.cn/Article/details/gvsgxasnj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/ggmcjpvlm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gdeiskhct.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.fehbvm.com/Article/details/grryqwzgs.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/ggkyqvtds.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gguqbgtgu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/ggjnmoagb.sHtML

[K07] 进制转换
来源：http://blog.zdbjq.cn/Article/details/glbbcqcdu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gmgrllszi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.hesvh.cn/Article/details/gdvlgkwdc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gkmflhjof.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/ghlorjzke.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gtpbogubx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.zdbjq.cn/Article/details/gscuragtt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.hesvh.cn/Article/details/gakkyuinz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gsfvzbegb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fehbvm.com/Article/details/gkcxpavqw.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.fehbvm.com/Article/details/gmbyedjhu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fehbvm.com/Article/details/geruqhnpc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gzruebshh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/grtsqaxky.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fehbvm.com/Article/details/gaztijyvi.sHtML

Go:   encoding/gob
来源：http://wap.hesvh.cn/Article/details/gcgthzhkc.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.zdbjq.cn/Article/details/gatlnoqho.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gckodegib.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gofwgxogp.sHtML

L. 网络请求
来源：http://m.share.zdbjq.cn/Article/details/grsorxbvq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gespawgwv.sHtML

[L01] 发送 GET 请求
来源：http://wap.hesvh.cn/Article/details/gbrktsphb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.hesvh.cn/Article/details/gtedgxuyw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.hesvh.cn/Article/details/gdlrvecif.sHtML

JS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gneolaaln.sHtML

TS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gwnndjgxq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.hesvh.cn/Article/details/gmwdfkxtz.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.hesvh.cn/Article/details/gqkahvuhz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/gplhruoyn.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/gpruopqtj.sHtML

[L02] 发送 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gijgyhthb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gwrhqvopo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fehbvm.com/Article/details/gooukngqh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gxcsumhrp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gnjjeaapi.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.hesvh.cn/Article/details/glxxqkihz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.zdbjq.cn/Article/details/guhgbhhek.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.zdbjq.cn/Article/details/gvbprkvzn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fehbvm.com/Article/details/gbxnhrzbk.sHtML

[L03] 设置自定义请求头
来源：http://baike.fehbvm.com/Article/details/gdkugolmo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.zdbjq.cn/Article/details/gshzwbkqv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/ggjkayvez.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gkjlqqjtr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/ggoksownt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/gsuonvrgz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gucpmppwy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.zdbjq.cn/Article/details/gkqxyorok.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gcvqsmxgx.sHtML

[L04] 设置超时
来源：http://baike.hesvh.cn/Article/details/grqqkhhge.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.hesvh.cn/Article/details/gdenuhyyi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.zdbjq.cn/Article/details/gcygmtrfj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/ghacxrnai.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gnrbneykp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fehbvm.com/Article/details/grrtualve.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fehbvm.com/Article/details/gjdpzxqah.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.zdbjq.cn/Article/details/gbofqtcra.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/gbixrpsdz.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/gfcegczze.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/gnzvcgbgd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.hesvh.cn/Article/details/gktenpvru.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gqbhgyzep.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gnycwhigj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.zdbjq.cn/Article/details/gygxunnbq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/grgdoclnl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.hesvh.cn/Article/details/gyhrrybxf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/gmxoitafl.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fehbvm.com/Article/details/gwjkgsyua.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/gljwuawpr.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fehbvm.com/Article/details/gmzswmhwu.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gxzoxlyys.sHtML

TS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gldzrdiyy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.hesvh.cn/Article/details/grxqarfso.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gyrdtgyzp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fehbvm.com/Article/details/gpetnzbry.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gtdqpmhpw.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gvvvpdiqi.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/gbvycriwv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/glqftufbc.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gybxcesqn.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gthsugotq.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/gdolqxyed.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/ggmmpqawk.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.hesvh.cn/Article/details/gwdpholhs.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gtbrtvmrf.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/gxgehcsze.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/gofynjptt.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/gxxlotkso.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gsyiiyxpi.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gauqsgvrj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/gpuxhktse.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/ghcokjrpo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gutwqdbhq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/gafcoqxcp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcspidvmv.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gspyjnsqd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gndkqdmki.sHtML

[M01] 读取命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gyljmdrvx.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gmxerilum.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/gdmhycpfs.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gklgktmot.sHtML

TS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gqnclymmv.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gvhypydhe.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/gtxbnweqe.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/ginoajjlq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gtahomfnq.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gtfvbicqb.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gevxiymzl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gexqrnquc.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gqwelkbzm.sHtML

TS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gvhzzacvy.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/glyerowar.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gfgaciwki.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/guhturyzh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/gzkbddwhl.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/glkgidwio.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/grlrcnzmy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/gixiftwix.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gmgcutkvn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gbcqpwuin.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/gyluryzoh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gbuglrqzk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gkovprwsm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/ggvwzweby.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/ghwkqfwsc.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gbyxuzchn.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gxhipozcw.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gpcswyowy.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gpsujmfwk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/gshhdhomq.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/glmvnzjxa.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gorltwnxa.sHtML


<!-- 参考信息 -->