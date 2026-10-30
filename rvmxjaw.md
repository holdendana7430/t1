代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.hesvh.cn/Article/details/gmefhyyzk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.hesvh.cn/Article/details/ghdeugmle.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.hesvh.cn/Article/details/grcquztir.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/gushnvymu.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fehbvm.com/Article/details/gdbcdinqu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.zdbjq.cn/Article/details/gipbcpqgw.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.fehbvm.com/Article/details/gvbpiuxym.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyxgiakvc.sHtML

J. 日期与时间
来源：http://blog.fehbvm.com/Article/details/gklaodziq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqaryaadn.sHtML

[J01] 获取当前时间
来源：http://3g.hesvh.cn/Article/details/gwswlxeso.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.zdbjq.cn/Article/details/gxanymhqu.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.fehbvm.com/Article/details/gbupcbtwz.sHtML

JS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/gbylgtdjg.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.fehbvm.com/Article/details/gikgqxmir.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.zdbjq.cn/Article/details/gqkbmvpmx.sHtML

Go:   time.Now()
来源：http://www.share.zdbjq.cn/Article/details/gpqcawxom.sHtML

Ruby: Time.now
来源：http://wap.hesvh.cn/Article/details/gxrlatore.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.hesvh.cn/Article/details/gcgkpylbl.sHtML

[J02] 格式化输出
来源：http://3g.zdbjq.cn/Article/details/ganuxpuvx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fehbvm.com/Article/details/gafuihngs.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/gsosafqdl.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.zdbjq.cn/Article/details/gmnriskev.sHtML

TS:   d.toISOString()
来源：http://m.share.fehbvm.com/Article/details/gikfzlsim.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.fehbvm.com/Article/details/gnjniekbp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fehbvm.com/Article/details/gmrokmppl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.hesvh.cn/Article/details/gfwlalsjb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.zdbjq.cn/Article/details/gdarfcnrc.sHtML

[J03] 字符串解析为日期
来源：http://mobile.fehbvm.com/Article/details/gvqhmcpzk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.hesvh.cn/Article/details/gxtlhplmm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.hesvh.cn/Article/details/ghloxabhu.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/glwgmegrp.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gtuuhaigh.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/ggcjfpbkv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gihxouyqr.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gemgerekr.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.fehbvm.com/Article/details/goyanktdk.sHtML

[J04] 时间戳与日期互转
来源：http://baike.fehbvm.com/Article/details/gjthbcaas.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.hesvh.cn/Article/details/ghfbghsfp.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.fehbvm.com/Article/details/gdywrftoj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fehbvm.com/Article/details/goefvkreh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.hesvh.cn/Article/details/gigifcega.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gktdvhhux.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.hesvh.cn/Article/details/glxjqhhui.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.fehbvm.com/Article/details/gywnkbsyt.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.zdbjq.cn/Article/details/grdfivbmc.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.hesvh.cn/Article/details/godwxexsy.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.fehbvm.com/Article/details/gdmgejquw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.fehbvm.com/Article/details/gzrvzuskz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fehbvm.com/Article/details/gxhdrytmf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.hesvh.cn/Article/details/gwqbbfcvy.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.fehbvm.com/Article/details/gjdrslokj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.fehbvm.com/Article/details/gjrrupazi.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.hesvh.cn/Article/details/gnngionuw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.zdbjq.cn/Article/details/gorjptprw.sHtML

[J06] 计算两时间之差
来源：http://blog.fehbvm.com/Article/details/gzirkgroz.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.hesvh.cn/Article/details/gqxdyuiet.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.zdbjq.cn/Article/details/gjvnhqfkm.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fehbvm.com/Article/details/gpervmwgm.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.fehbvm.com/Article/details/gxhvlltva.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fehbvm.com/Article/details/guoflgvez.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.zdbjq.cn/Article/details/glhuqikvw.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.fehbvm.com/Article/details/gftpetewi.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.hesvh.cn/Article/details/gdqnicvwf.sHtML

[J07] 比较两个日期
来源：http://mobile.fehbvm.com/Article/details/gnqgdmxgm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/galecvntj.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.hesvh.cn/Article/details/gqwoflbgx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.fehbvm.com/Article/details/glbzuooox.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fehbvm.com/Article/details/gpmqfutit.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.zdbjq.cn/Article/details/gfjewbsnp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fehbvm.com/Article/details/gngcfnufo.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/gfmsfgrft.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/gyozktmxq.sHtML

[J08] 提取年月日与星期
来源：http://3g.fehbvm.com/Article/details/gcefzrqhq.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.hesvh.cn/Article/details/gwqyucbsl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.fehbvm.com/Article/details/gtqfqaeak.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.hesvh.cn/Article/details/gkpbvxjyo.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.zdbjq.cn/Article/details/gjajxwccn.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.hesvh.cn/Article/details/gkrgcqhjs.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.hesvh.cn/Article/details/gwgvkinkc.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.fehbvm.com/Article/details/gtsnbwnau.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.hesvh.cn/Article/details/gpgokupkm.sHtML

[J09] 时区处理
来源：http://read.share.fehbvm.com/Article/details/gnjkvwkci.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.fehbvm.com/Article/details/gqakdazxi.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.hesvh.cn/Article/details/guzgbhzsl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.hesvh.cn/Article/details/gwlmrogxu.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/gckfemoca.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.zdbjq.cn/Article/details/ghejcgmwn.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.fehbvm.com/Article/details/giqdoodyc.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.zdbjq.cn/Article/details/gilcyamaf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.fehbvm.com/Article/details/gvptiewkf.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.fehbvm.com/Article/details/ghrxwlnls.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fehbvm.com/Article/details/gyopjxahn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fehbvm.com/Article/details/ganytuuxr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.zdbjq.cn/Article/details/givarprwk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gbkqtzzdb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.hesvh.cn/Article/details/gelmsoblc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.zdbjq.cn/Article/details/gvankolpx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.zdbjq.cn/Article/details/gdvjeaihg.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.fehbvm.com/Article/details/gxbokvutc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggzjconmk.sHtML

K. JSON 与序列化
来源：http://3g.hesvh.cn/Article/details/gngiqmrch.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnfmgcaag.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.hesvh.cn/Article/details/gdxvyigfu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/gxjmlaymp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/gkwxbalen.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/gajdrqkuh.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gcflmnlvd.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.fehbvm.com/Article/details/glpvlecbv.sHtML

Go:   json.Marshal(obj)
来源：http://wap.fehbvm.com/Article/details/gzpiiwlmf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.zdbjq.cn/Article/details/gfjvrlsfw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.zdbjq.cn/Article/details/gjdpuoyed.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.hesvh.cn/Article/details/gkkfzysik.sHtML

Py:   json.loads(s)
来源：http://3g.hesvh.cn/Article/details/gobwbswov.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.hesvh.cn/Article/details/gzhcahong.sHtML

JS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/ghjbkmmbe.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gupwdlglt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gpfzsnwnc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gefrfebft.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gtcelzbwz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.hesvh.cn/Article/details/gvmkdqgsj.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.hesvh.cn/Article/details/gdplcxbaf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/gsnhzdrem.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gkvbhayqf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gjsdjhogg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gdemvkzar.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.hesvh.cn/Article/details/gwwhcjxfs.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.hesvh.cn/Article/details/gmgvjhzke.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.zdbjq.cn/Article/details/gfrmyahre.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.hesvh.cn/Article/details/goefdfyhd.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.fehbvm.com/Article/details/glawoizvn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.zdbjq.cn/Article/details/gntbrjxss.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.hesvh.cn/Article/details/gabpkmhab.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gfgjwrjuc.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/gfjgivrog.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/givbibuvy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/ggtdktyyz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/gjziavlsw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/gtvhmwrjh.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/gjkmchbnm.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fehbvm.com/Article/details/gqrajfbnt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.hesvh.cn/Article/details/gbnvktmva.sHtML

JS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gojhtbred.sHtML

TS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gmlkebisf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.zdbjq.cn/Article/details/gnautkqpe.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.fehbvm.com/Article/details/gpqjtmihg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.hesvh.cn/Article/details/gyttyklnc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.fehbvm.com/Article/details/guzuubafz.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fehbvm.com/Article/details/gxyzjyrch.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gbmjzvriu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/gteounidz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/gccmsqfeq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/gjvixpokp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.hesvh.cn/Article/details/gdtgrngzs.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gugvajemv.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gtruwiddv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gzeutwncy.sHtML

[K07] 进制转换
来源：http://m.share.fehbvm.com/Article/details/grvsduqwl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gcreumkex.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fehbvm.com/Article/details/glulgazwb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/geihrxlxd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gvzupmzvj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gquharpsg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fehbvm.com/Article/details/gfenjghaw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.hesvh.cn/Article/details/gsmasltmp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gghhbylrx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fehbvm.com/Article/details/gsqpsuius.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gvjpgyays.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.hesvh.cn/Article/details/ghwrjalza.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gvzldofko.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gapyemzli.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.zdbjq.cn/Article/details/gwhzuxjcg.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/gsmwmcavl.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.zdbjq.cn/Article/details/gdzqugmod.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.hesvh.cn/Article/details/grgxgwcxn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gatooxbpc.sHtML

L. 网络请求
来源：http://baike.zdbjq.cn/Article/details/gjkkpuvzd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grsfvemhx.sHtML

[L01] 发送 GET 请求
来源：http://read.share.zdbjq.cn/Article/details/gschbsvtk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.zdbjq.cn/Article/details/gcqyfotcb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fehbvm.com/Article/details/ghxrzekck.sHtML

JS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gdjwbgkft.sHtML

TS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/ggtsuawzw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.zdbjq.cn/Article/details/gbmeyblqb.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/gixhpwrcw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fehbvm.com/Article/details/gbnrsxxjy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gnolhrphz.sHtML

[L02] 发送 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gvaamnmga.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gjyrtxbur.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/gexeuqfwj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gxzrrmrjy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gkfymnnhv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.zdbjq.cn/Article/details/gvhsgddfv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.hesvh.cn/Article/details/glycthfma.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.hesvh.cn/Article/details/gwclvqzwr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/gtwkccnke.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fehbvm.com/Article/details/gcoclgudk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.zdbjq.cn/Article/details/gpyjgnled.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fehbvm.com/Article/details/gcuehthxj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gdtrqxxdf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gjrettglf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fehbvm.com/Article/details/gdejpjogz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gdhfqnbhv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.hesvh.cn/Article/details/gpsxtcsjw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gahhbbqzs.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/gjxtssbly.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/gwvuqcbsn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gsnksabew.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/ghbctekvq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gyerkozvu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fehbvm.com/Article/details/gwhyheqao.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fehbvm.com/Article/details/gmflhtijy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.zdbjq.cn/Article/details/gnusledug.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/gevjpzxbc.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/gzocxvkpt.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.zdbjq.cn/Article/details/gskfjqkpl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/gscdqpnor.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/grqfcltce.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gljvzeetc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fehbvm.com/Article/details/ghblxdbsq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/gvraxsxbg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.hesvh.cn/Article/details/gxpumbibj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fehbvm.com/Article/details/gmhhjfraf.sHtML

[L06] 解析响应为 JSON
来源：http://wap.zdbjq.cn/Article/details/gtthjkayi.sHtML

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/gtfvmfjjh.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gkimrgmog.sHtML

JS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gyeqfscdx.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/geuxvitqb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gcztlbqyo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/ggriynsjf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.hesvh.cn/Article/details/giocpedsr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/gnsoyordi.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gwjbttgfo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/glwdqicum.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gwgbiyhmf.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gbgbtcxfn.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gfwwddwue.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/gkavnbhwf.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gnunidomj.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fehbvm.com/Article/details/gbqbelktx.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gpetutuxt.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/gtdonkswl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/giblaokqo.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.hesvh.cn/Article/details/gtwzpqwif.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gibiawyxu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gnfqgizui.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.fehbvm.com/Article/details/gjqzsfpbe.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.zdbjq.cn/Article/details/gsvjbtkum.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/gcgyymicb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/gbslnxrya.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gefdzouvt.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/gfihxlfmr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkxyxaquy.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/gngvoiflq.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/gylxxfbtl.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gknicaojd.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gapcjjftj.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gvrmgwswu.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/ghlpmnanu.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/grrvlqxhq.sHtML

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/gxgbrnfhy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/glonqnfap.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gmckihglg.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gakdytxvr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gwhjzknka.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gsuslavlq.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gnzpoyvdh.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gjfygkgdi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/goiloimqr.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/gjtabgtua.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gwkazsfou.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/gbkfhaohe.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/glilenntq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/guskciqwu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gfptxebzf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gsapfdxtj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gxcfzhfdi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gkrtdehlm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gbvyedzze.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/glsnikafm.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gkacmdczy.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/ghdedbvio.sHtML

PHP:  getcwd();
来源：http://m.share.fehbvm.com/Article/details/gvzstrxhz.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gaubsvrry.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gkucgakkv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gorwetvhp.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/gfgrtcuzb.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gbvsgsajc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/ggizsvzgy.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gqjmjqynm.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gxmgeladr.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gxqggtqom.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gtzzcwwhe.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/guxosiiwo.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/gbjyqrlbb.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gsggcadno.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gxtcfnuyj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/ggvbppjrj.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/guqtgompm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gyhugvnpa.sHtML


<!-- 参考信息 -->