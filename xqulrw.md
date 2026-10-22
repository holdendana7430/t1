代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2ehimvpzc.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2mofsavfj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2mekeztgx.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2qwjoxfpx.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2qibelygk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2fatcepvm.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rvgeckeh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2smqwnkex.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2qilkfapo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2qihqxvsd.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2cyvoywrr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2zvbscujq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2vettyjsk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2fiiueazn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2rydpwpra.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hywoodio.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2xifygroi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qsfxtmjz.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2setthcuz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2wnwtupxb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2cpskqcmm.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2ajxynslz.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2rvocwtmm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2qomcatja.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2suwngagq.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2odrxybza.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2qtkkoaqd.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2buwtcqby.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2btdfeqxn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2eaglkzrv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2zdncpzib.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2uhuercnx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2ggaqshpc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2errjwzjh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2xiaxbwrr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2xutmidlc.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2zvqtxrvr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2wtfqgrbx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2uyrkglao.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2fvlilymz.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2iynhvrxg.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2rpzpykbl.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2yjqmyvgm.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2alptooac.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2wknczoqw.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2hsnvvecd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2yrleaqku.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2jnauxeln.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2eqzkqxlu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2ciotyfnm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2wwclzybq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2eylymcut.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2dcfmfhnb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ncdltedo.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2xttzfgio.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2mvumenzk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2fxgesiuk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2umvnnows.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2armktabz.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2mxgpyinv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cmqkezrf.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2pcrcfosz.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2mjonlrlz.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2vzakvyvu.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2jfnqxnln.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2ngqpjbef.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2rulbxwhm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2xbperxkc.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2kluduvmm.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2ymbazoch.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2qtoqcbbz.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2czoibicb.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2otkehopv.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2vulqozeo.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2kvakmhfi.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2lfswzihk.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2llkcvxdu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2qodfstxd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2aqrwajzd.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2zmhezjfr.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2egpitwks.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2buvocptp.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2uslaexpa.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2hawiwtxk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2omdxqfdt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2jbngpftl.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2bpmvnrzv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2bqdjpfkj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2scavahzo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2zrdnrzqc.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2lywbeequ.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2vrckbjez.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2mjnsgpct.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2ajnhjuma.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2psobjiee.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2qroqirkb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2vwgpanqc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2fngcidoy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2lxhzbthn.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2uwsgcivp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2tlcnwxse.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2rnlazleu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2isqcekla.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2jkwjwhub.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2ciegnehg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2syeurqsb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2hjhkjukm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2dawlipbu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gqribcya.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2dzrqlrcn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cxoaidgk.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2sroleiyl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2efexould.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2iunrfygi.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2iufmtwyn.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2axycuspo.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2vjwlvede.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pxueclue.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2pslkjfqz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2pzwylwln.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2bknwricd.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rbfgouhi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2togqmber.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2etwvhrrq.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xnkpjokf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2uzdslwcv.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2dqnplcxo.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2nujmpfgu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2famqmslj.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2wvvqsvqb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2uvanbqbv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2czodousp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2phpqmtno.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2trjxgcjg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2rqwlyfoy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2tlrrsrwc.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lsjvwbpt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2xhvseiuj.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2duoqjrlh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2zxglmovg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2xtvknmfr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2twueefgb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2gvzfrciu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2bpsslwld.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2laulubcw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2pmjiuytp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2eqaqstsi.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2nuknnxta.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2otozbnto.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2evabvdnq.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2hvaqwvkh.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2euuvpyer.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2mmmpdonh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2mpvsfnct.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2mnnzwwzw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2kxltvyxe.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2rbjccvvx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2uvrbecyz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2xwpxkbvv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ocehmnzr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vgqmrvos.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2iuuugzsz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2gpadmrge.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2iacymria.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2xjohxweb.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2nxylrcfi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hervdofw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2qizjyauz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kzvbdqgm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vfzaqdph.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nxkymiaq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2siejkpbu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2jpzmqrcd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mrxdeats.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2zjajznvt.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2yivouygp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2afyelngi.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2jkrzuccr.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2qyrsugbn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2kdauddam.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2umzhjfhm.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2aghkakou.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ycjrvrcs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nlbfraou.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2sjsmnuur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dhuiqzne.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2ytplhgqj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2lqrzjblm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2nhoufmwo.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2hllwfdrw.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2irnukymp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2oupkxwxq.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rurpbbnu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2qzouknvx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2yhrhfeny.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2abnxnbqg.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2axatzvhc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2sivhbdyk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2rjuxerdi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2qklqvszo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2wcwfrxue.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2kqddpcqv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2fvjvdefk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2vlabgwya.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2pfpwqbui.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2lxvsxuva.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2khjgftuq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2rjvattjy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2jectcuir.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2qxuuyrih.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2quhjiynz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2xetgsahd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2loissxha.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2hqewqlxy.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2vgwvbitj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2xwsoxwjy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2uwomxdkk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2mwqooiqx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2lsvivqtv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2yrnmdkpa.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2ttapncyu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2nwatsguy.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2towtqkjr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2djwtewly.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2etagbmft.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2epeyhnni.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ubfazpvr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2wzrgloub.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2reykusga.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2mloknrqh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2aicpivjb.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2oxahsamn.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2difwbxll.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lcrmwoud.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2diormswf.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hgbqonmo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2uuadzusm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2ynqeddeo.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2wszkokxq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2zzwtmsty.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mijtjiey.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2ptxithci.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ovhbxsci.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2fjnqibvi.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2qvhvkhzn.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2tyjjyvpm.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2trfwddvd.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2tbmfhzho.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2gkxqckkl.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2mzcvsist.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2jbdpeiah.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2ooqwxqgc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2arjlfvdm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2mcypcqxm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2dtwcnoct.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2nkvgnpxw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2flshknok.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2conizbus.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rpqhxdtt.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2tjvcunwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2snzmhqrn.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2uuqebrtu.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jzgsedbs.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2bwflwbmh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qmrvyorx.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2zbxujswc.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2lwkfvhik.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2pwmckrua.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2zobszprv.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2movmcrsv.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2leyejxbx.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xxhjtzrc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2gshwqshd.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2lnnoachh.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2fagasecu.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gmgmszjm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ajgmsfpz.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2btwenqwc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ccrhlyzm.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2labuksvh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ehqujaiv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2nuvdepvm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tiwxvlzn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cvjmunxa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2wiyfxjpe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ubqdyxpj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2uqvaxivo.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2rlxcbpuo.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2imxtdhgs.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2njhltcuh.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2meduiqss.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2prxivqwa.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2esjkvhwy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2najhfxuc.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2jumfwczd.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2kpdxquod.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2txhtltko.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2gkdrqaik.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rsvuzgxj.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2vnjndoem.html


<!-- 参考信息 -->