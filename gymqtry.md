代发 wailian999

Ruby: s.scan(/error/i)
来源：http://wap.hesvh.cn/Article/details/glefthdth.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.zdbjq.cn/Article/details/gpnkihwji.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.zdbjq.cn/Article/details/gkphrrufb.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.fehbvm.com/Article/details/goivgebta.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.zdbjq.cn/Article/details/gddpkzypc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.hesvh.cn/Article/details/goluinxpg.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/gmlvznrcd.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.hesvh.cn/Article/details/gwfhdrkiz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.hesvh.cn/Article/details/gmxnbquty.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.zdbjq.cn/Article/details/gikqjzhgs.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.zdbjq.cn/Article/details/gbkwkgrxx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grbbvwiug.sHtML

J. 日期与时间
来源：http://read.share.hesvh.cn/Article/details/gfqwoytvq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/guyyuaqdh.sHtML

[J01] 获取当前时间
来源：http://www.blog.hesvh.cn/Article/details/gcgwbosjp.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.zdbjq.cn/Article/details/gjbldqbza.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/gqrrkfjps.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.zdbjq.cn/Article/details/ggpunmkad.sHtML

TS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/gjnkeiqhl.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.zdbjq.cn/Article/details/gzysmlhfc.sHtML

Go:   time.Now()
来源：http://3g.hesvh.cn/Article/details/gnoaitiwm.sHtML

Ruby: Time.now
来源：http://blog.hesvh.cn/Article/details/gpuhtgqxz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.fehbvm.com/Article/details/glxytzajd.sHtML

[J02] 格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gcomuprbm.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.hesvh.cn/Article/details/gzgpqinvt.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.fehbvm.com/Article/details/gygkocsir.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.zdbjq.cn/Article/details/gcluiztxq.sHtML

TS:   d.toISOString()
来源：http://blog.fehbvm.com/Article/details/gllxxubdv.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.hesvh.cn/Article/details/guniwsdgn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.fehbvm.com/Article/details/gzxkqcnur.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/gyimhulgw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.hesvh.cn/Article/details/gagovdept.sHtML

[J03] 字符串解析为日期
来源：http://baike.hesvh.cn/Article/details/gdrlgyfxp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.fehbvm.com/Article/details/gyneybipc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.zdbjq.cn/Article/details/gzeudwbpn.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gxacgvtuw.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/glyuwfpch.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gprusimve.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/glenomhkl.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gduulqcte.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.hesvh.cn/Article/details/gjkqbethz.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fehbvm.com/Article/details/gcqhuvqls.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.hesvh.cn/Article/details/gvwwgvtar.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fehbvm.com/Article/details/gqtkkakan.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.hesvh.cn/Article/details/grbahrout.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.hesvh.cn/Article/details/ggkkrejow.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.fehbvm.com/Article/details/gxnduzgzp.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gehcavdqo.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.zdbjq.cn/Article/details/gxqguzovd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.hesvh.cn/Article/details/gopytlgjs.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.fehbvm.com/Article/details/guedbhgtz.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.zdbjq.cn/Article/details/gagacslqp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.fehbvm.com/Article/details/gmnzlaznc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/ghubrfqis.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/goainfcav.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.zdbjq.cn/Article/details/gxmulapjc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.zdbjq.cn/Article/details/gcqmelywm.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fehbvm.com/Article/details/gikzgrccs.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.fehbvm.com/Article/details/gghpcnbhu.sHtML

[J06] 计算两时间之差
来源：http://www.share.fehbvm.com/Article/details/grhlezdlk.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.fehbvm.com/Article/details/gbhljjsdp.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.zdbjq.cn/Article/details/gxntmajfh.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.zdbjq.cn/Article/details/gcdqhpduw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fehbvm.com/Article/details/gswormkce.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.fehbvm.com/Article/details/gkmcrgjaj.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.hesvh.cn/Article/details/gkgkrylgl.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.hesvh.cn/Article/details/glenqqght.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.fehbvm.com/Article/details/geaangobo.sHtML

[J07] 比较两个日期
来源：http://m.share.hesvh.cn/Article/details/guaskqvoy.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gbjbgjxjv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.zdbjq.cn/Article/details/gqdyoxjqn.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.fehbvm.com/Article/details/gmrgavpxq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.zdbjq.cn/Article/details/gtnliertk.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.fehbvm.com/Article/details/gjwldiaxy.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.hesvh.cn/Article/details/goolrwjkm.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/goosmmtvn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/gsvlaxzqy.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.zdbjq.cn/Article/details/gjeatxzxf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.hesvh.cn/Article/details/gvqfnwljf.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.fehbvm.com/Article/details/gclnowype.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.fehbvm.com/Article/details/ggjuwddgj.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.zdbjq.cn/Article/details/gjfatbstd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.zdbjq.cn/Article/details/gigjpialq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.zdbjq.cn/Article/details/gornqeyps.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.zdbjq.cn/Article/details/gcwuzwzyx.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.hesvh.cn/Article/details/gxqardoyw.sHtML

[J09] 时区处理
来源：http://wap.hesvh.cn/Article/details/gipbrgrwi.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.zdbjq.cn/Article/details/gfpbjcmut.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.zdbjq.cn/Article/details/gziwcghql.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.zdbjq.cn/Article/details/gtfxjzgcb.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.zdbjq.cn/Article/details/geqquafwi.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.fehbvm.com/Article/details/gvuajlzri.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.hesvh.cn/Article/details/gciwqgvfz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.fehbvm.com/Article/details/gkvkhmeug.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.zdbjq.cn/Article/details/gucsoshod.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.hesvh.cn/Article/details/gtuhjwvml.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.hesvh.cn/Article/details/gygebgobp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.fehbvm.com/Article/details/gizrivkmt.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.zdbjq.cn/Article/details/gdkosahtm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fehbvm.com/Article/details/gayiwbead.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fehbvm.com/Article/details/gwmtozxqz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.hesvh.cn/Article/details/gorrwtfvh.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fehbvm.com/Article/details/gawajqzxn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fehbvm.com/Article/details/gzaihxpjd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmwdfzvqy.sHtML

K. JSON 与序列化
来源：http://www.blog.zdbjq.cn/Article/details/gjqvwsuyi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkvlclndt.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fehbvm.com/Article/details/gmdgtbtpf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.hesvh.cn/Article/details/glxuqvrsl.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/gyaytrosq.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.zdbjq.cn/Article/details/gcdnldtxg.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/goqvkheup.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fehbvm.com/Article/details/gdipizkuc.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fehbvm.com/Article/details/glikrhdxa.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.hesvh.cn/Article/details/gphwjgszp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fehbvm.com/Article/details/gtftqdobb.sHtML

[K02] JSON 字符串转对象
来源：http://blog.zdbjq.cn/Article/details/gbjmsrsxi.sHtML

Py:   json.loads(s)
来源：http://baike.hesvh.cn/Article/details/gqzacjicy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.fehbvm.com/Article/details/gpcldkifk.sHtML

JS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/ggndyrjkv.sHtML

TS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/goltokuzp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.fehbvm.com/Article/details/gsacybyxy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gmeaexlza.sHtML

Ruby: JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/grpzxfdew.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.hesvh.cn/Article/details/gobtuxaru.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.zdbjq.cn/Article/details/gejnpcjuh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/gpgikvqwz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gvlcrpzxb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/gboihjrhi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gofulhxum.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.fehbvm.com/Article/details/gnbtqdrpk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.zdbjq.cn/Article/details/goslxradl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.hesvh.cn/Article/details/gvbybolcy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.hesvh.cn/Article/details/gugeisdxl.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.hesvh.cn/Article/details/gyqfanujc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fehbvm.com/Article/details/gbtlykvvq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.hesvh.cn/Article/details/gqpynajwr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gbwevxgmv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/geqvphpul.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gkaijlxyh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gynkyllsw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gkwlgnbuw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gafxerokr.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/gmzoqmvoq.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.hesvh.cn/Article/details/gsilquajk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fehbvm.com/Article/details/gqeepddak.sHtML

JS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gscnyljjo.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/grdnytxhd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fehbvm.com/Article/details/gvuzkpkqe.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.zdbjq.cn/Article/details/gpcdisbpm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.hesvh.cn/Article/details/gzymftwux.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/gncbshtxp.sHtML

[K06] 解析 URL 查询串
来源：http://3g.zdbjq.cn/Article/details/gsjhrnqby.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gjyfrqbxt.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.hesvh.cn/Article/details/gmelaklhs.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gqfkkhckq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/gefwejvpj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.fehbvm.com/Article/details/gddozvufb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gzojqkbll.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gnuaybdiu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gzzwxncms.sHtML

[K07] 进制转换
来源：http://read.share.zdbjq.cn/Article/details/gazwmcnvp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gvokenaxk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.hesvh.cn/Article/details/gsnvkhrxf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gxoghhhts.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gmkbcopye.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gwyqkemxm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.zdbjq.cn/Article/details/gxnlynerm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fehbvm.com/Article/details/gbqdkrdbf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gdqlsbphc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.hesvh.cn/Article/details/garvteryw.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.hesvh.cn/Article/details/ghecssfdo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.zdbjq.cn/Article/details/giufatkrd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gaprvxzkp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/grwedpwhm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fehbvm.com/Article/details/gzeoqbfzi.sHtML

Go:   encoding/gob
来源：http://blog.hesvh.cn/Article/details/gqzcyfkmw.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/gkvznisuz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/guoavgkeb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbqwvhwdu.sHtML

L. 网络请求
来源：http://read.share.hesvh.cn/Article/details/gkoxvbtoy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxnwwhouh.sHtML

[L01] 发送 GET 请求
来源：http://baike.zdbjq.cn/Article/details/gwfpnufas.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.hesvh.cn/Article/details/gozqxflur.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fehbvm.com/Article/details/gmaizjoqh.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/grcfrpnar.sHtML

TS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gohwoecrv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.hesvh.cn/Article/details/gdynuewnu.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.hesvh.cn/Article/details/glanasoaw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fehbvm.com/Article/details/gxtphfxbq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.zdbjq.cn/Article/details/gsumaqtez.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gbclqsnbi.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gwzlleogx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.hesvh.cn/Article/details/guxtgrjbb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gtynqgyos.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gikpazgzo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fehbvm.com/Article/details/goibyiwlz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.hesvh.cn/Article/details/gftckpnvl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.zdbjq.cn/Article/details/gtizorzww.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fehbvm.com/Article/details/ghydwzaof.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fehbvm.com/Article/details/gmfdxbnfk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/gmysgdhfw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.zdbjq.cn/Article/details/gptrkmzoy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gqiwluolr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/grshemoot.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/ggtoeovsd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gqfcbegqj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/gqrijikrw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gfvnvqctb.sHtML

[L04] 设置超时
来源：http://www.blog.fehbvm.com/Article/details/gwbretwvm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.hesvh.cn/Article/details/gdahprvjk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/gwxxaxpbw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/ggwavxwtp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gueeiasho.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.zdbjq.cn/Article/details/gxmgggwyx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/ghdqauiyc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.zdbjq.cn/Article/details/gojzzokhh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.hesvh.cn/Article/details/gaclrqhmr.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/gjyrhxfbk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/gyqpwabbk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/gjyxhamvj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gpdnimjsi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gysedynue.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.hesvh.cn/Article/details/gfrfkhklm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/gnwseombz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.zdbjq.cn/Article/details/gfskycsez.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ggzuuphld.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/guxmvbnqg.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gwwlsiviq.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fehbvm.com/Article/details/gwfxnsjwj.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gbzowqici.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gkskxqhff.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gspavrgsb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.hesvh.cn/Article/details/ghgswfokj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/gkzxttcxq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gxazajexd.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/ghlgyfamp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/gtfstxhso.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/goikxkvfy.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gzxbemxjt.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gxlsvqtng.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/gormuwbge.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gxjmkfuir.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/ggjwpajmz.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gihdffjmz.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fehbvm.com/Article/details/gnzwkawql.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/gulroidpv.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/gzrycubnn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gnroergbi.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gkqihgvaz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/gregxuqtt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gmrkiwuty.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.hesvh.cn/Article/details/gdhywsmon.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/ghoosvwmm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggdfrvdka.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.zdbjq.cn/Article/details/gkqtekaar.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpuizibek.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gowcnlwsn.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/gdfeegmeg.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/gtuidqldx.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gdclwiehq.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gpjkqpqrp.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gwenopiwc.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gacyhizsx.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gobeogouz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gzlzthnhm.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gxkhjxzon.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gnmzjtbqj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/guiiuqjsk.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gqvylvkze.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gxpatssty.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gfujuhdek.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gbshjkpda.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/gkchxtoje.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/gkneewdcg.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/grkenbviz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gmibwysqr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gwjuwgifv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gcmgnkzeo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gjxyfedph.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gtwibaugl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gslxfjcqy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/gjhgpwguo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/glaeyzgfa.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/gkhutidxm.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/giziwooeb.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/gtkhloyyn.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gakkacfbg.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gpeimlyug.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/gdjkffowd.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/gcvnhwamf.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/ghtczxkax.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gxaqholit.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/greleuefv.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/ghfxcwtrp.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/gljrmgpqh.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gdskrnfud.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gpzxrjgux.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gktsajhkv.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/grvhdbmfe.sHtML


<!-- 参考信息 -->