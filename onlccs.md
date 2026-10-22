代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2cdxcqbth.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2txivoifm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2frbsytyp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2ybgyvvbz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2kekisjvb.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2pjemyszs.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2nvrosdlw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2ohponbxi.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2peobahqp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2pbtpxbzr.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2skltqdpj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2okdtmtqy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2wgjfqbbl.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2mxsdjlwo.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2zkayzvcv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2vatmxjtj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2sqkbqdmn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2urvgnezw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2kitpgpok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ydkkuzif.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2kbqghxde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2omzwjtgs.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2oaeqlqjj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2cgrrayhu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2qcsemtef.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2xqyzcynj.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2wwksrrgg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2cjtvazii.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2nvuynrvv.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2raizrvtx.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2lkgvbhab.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2skxqfsix.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2dbczjhus.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2vhxrxylv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2cnvclgaz.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2qhnsunpx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2ynvibhml.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2vzfskiaf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2twdjayyx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2bfcgwcwe.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2ogotbzpp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2jiowssgp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2vjmxvamq.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2nxhcjoxr.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2gmetejug.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2nccbtxzr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ltwlsqyw.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2pztmwadi.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2yeijlodg.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2rwuayjoz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2yhilrkjv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2lfdglrkn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2jcnyvoxu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2miovdsyu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2bmrjlxmf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2naogwlcy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2ehywcelw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2crdnbqjs.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2jhgailut.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2hpvdfoox.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2vcgjgzej.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2dcoqjlei.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2vytgvebd.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2dclnqjog.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2aaxzznwu.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2dtruthes.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2smvvvfif.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2izsrepef.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2sgqdhqih.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2jknvjyfp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2qeihlcrw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2xjbrfkdg.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2zpzazpme.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2jdxyrhxi.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2vcgdpyfo.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2adpmqsqb.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2ylvcljdh.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2gquqpwyr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2tvvzlkwh.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2psdrebrj.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2xcwvaywr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2toyfcwgv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2caoajqya.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ncbyqkrk.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ktgeyrwa.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2olekutjb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2irjbuajs.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2kkqxkxkt.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2qkddabyd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2aloaahpj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2bizwjrcm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2twlivzju.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2erooanhq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2uxncfplr.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2kbrubgaq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2jmkbvwvi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2eqbajvsj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2zneakslh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2wxcmmspb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2bilhxeiz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2fcwvthgz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2bycsqnmr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2knvvwxof.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2pedwyuqg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2sjdndkan.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2jxhvsnjw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eeilkkas.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gcopvwzc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2eahocnbl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2mvrjjyjr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2nzrunvfu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2osazthxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wnnatiqc.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2dwbvueez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dtrbkfgp.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2zxeipfmr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2qymulnvj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2dvlbkals.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2yolbzbsh.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2qbvfhopz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2ekvmtari.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2zvekhlgv.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2cwzueafz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zbsbdpyy.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2ogobuuyw.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2rmsdahwl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2mjszpfdn.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2moqetvyh.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lrnazidf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2qbsqeest.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2bltbhqjq.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2itxtffgl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sbjnismk.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2yljvfoiu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2pghjfaew.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2mpfaxqbe.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2gjxsotnk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2paprpgcp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2eyhqdtim.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2wnnoyvoi.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sxjnihcx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2pwgywzvc.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2ppdntfrv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2mnljepsa.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2ytzyrjez.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ikcrtqxq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2isqpyrss.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ihncuocf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2gdppoeef.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2socglooi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ssffrugu.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2vdozlrdc.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2ukwcraop.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2kmaokgtu.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2dtcylhxb.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2auzsnrxs.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2oxsepsov.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2wudbmguz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2dthrnzje.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2kylflnnl.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2pwzuabiv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2frtfenor.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2rcwypvdz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ohnqckbk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2npovaknw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2xutsantr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2wtjcdkch.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2xeiuxpnf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2cewtlpnf.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2rqxkosco.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2cgijrnxh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2zaroewva.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ldoybipm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wzogsehw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2junnabqh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2mdvckegn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2umlnxwyc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2quxlitsa.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2bxczhjle.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2demzdcqp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2wwibqpvi.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xvzxyjwh.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vjxugpzt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2ywcdbvmc.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2fajpgwul.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wumweveg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2fqtturnt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wqhkgxui.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2cpmgbkdc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2idgfgofo.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2hocyfxvp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2nzbdihgv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2isxgeapv.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2tycmmpps.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2yjhhnvyw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2waxgnyka.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2friomocf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2ysaxnflv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2fditdges.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pbqzhcwk.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2wwitfbbb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2jgpyjlbe.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2abeahsiv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2kzhcuqmy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ahgffvna.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2giutpkgg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2auzjjyvz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2hhalnrcu.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2oprdwatd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2thgwuikq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2lfkbfmnk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2gjirxgsb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2buysymul.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2ggsauvhw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2tcfhbfpq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2vattisjl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2equjdayn.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2qeefwjgm.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2gvzmuzjd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2cjezhtky.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2plaxfgll.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2cjprpwhb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2dughgnjn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2keqladlm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2ejyrizon.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2egtilels.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2jcqlneuv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2ngccjzeu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2bapiglop.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ocjbvmut.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2eaxpvsjk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2npeqgeoe.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2gnkwemen.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2bqayopvr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kqdwksvc.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2hnfarzhp.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2rbbghnfo.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ogjwgtpy.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2seggmdhl.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2kaihmzca.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2wgpnteeu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2hnawjabf.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2mzpydxcv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2bwwbkwor.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2trppdpmc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2rpyuykvv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2kmhnptsx.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2bpswcgam.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2hqdgbpmy.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ivobffxe.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2dqrhqyox.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2xxlnjdgr.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ycdaehxx.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2tdehanqn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2oiugibvu.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2rqsdddwo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2tczvaftn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ggjxusre.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2pwerkxoa.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2etncdtdr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2desclrrb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2flknnbhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nbiogurw.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2qmeqweft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ufnxqlir.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2jwbosmpr.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2pkdkqqhy.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2skxrhgwm.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yndmscrg.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2klgoafxc.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2iwaloleg.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2uvpqhgzw.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2bpcnstbm.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2yxfwiwdy.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2cfzcqenk.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qwyzlctc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2lbzteggu.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2mcnaygun.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2dyxffmuj.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qzmhdyqa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tiwjckgc.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2lvwpdkow.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2twxcrhon.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2ezepcgmi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hlowhvyo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2tsdxxsrf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rvmzbxxt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qvkppigu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2uknbrpmd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2fgcaqvse.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2nmtvexhe.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2hfnlymbg.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2cotpsbjy.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2jcfyclbx.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2fuocdmhj.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qmpdrnss.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2swqqptra.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2gogpmkbe.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mlbkfsyt.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2sxplhbac.html


<!-- 参考信息 -->