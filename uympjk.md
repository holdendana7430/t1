代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2wododyyz.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2sgegocwb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2ukkgvnhf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2bxgpsiwx.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2ukkgwqwt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2fvvpvpiy.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2fceqeskl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2yekwdsiz.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2yjrhjjxc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2gvwjsrde.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2mioqjfic.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2lgrajlwb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2vbksmjfn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2yuflzdnk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2locihosw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2abpccpgy.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2yftomqug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yjkizmcz.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2xitjfvdw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2orgwvwew.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2efjlwtnf.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2rpvhcwim.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2pnegkrbm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ptfctmyz.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2yjqldwiz.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2dnhdlefj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2batkysxb.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2xjaokjjn.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2djymtkda.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2zyvysnnu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2jnwtahov.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2trgorwqv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2dbkzddgk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2tbqklwlq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2oaelrfqt.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2ttffphhj.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2lvkzllqw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2twjxpfgb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2rxfkykal.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2rfdqzrgv.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2kumymmdh.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2pkdzgmhn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2uzqgdewt.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2aqeiijhd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2xqvxpfqq.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2tgdoxoqx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2jcufxrue.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2jwyifxjc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2tjpkgrco.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2qfedcmwz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2dkeijjvx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sxfxplpq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2jczyqeyg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2amsztamk.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2nywaaopp.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2kbtjqubk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2reojhshe.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2fgzagkgg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ijywuebz.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2evoydsxx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xywugqlj.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2noppiyvq.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2jpgckjdq.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2kazlmkux.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2hrsrlrfo.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2hcqdxswc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2cpcdverq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2ihghcoug.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2iwvttrvs.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2iaypucgb.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2xhksqtee.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2btxwllop.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2sfprfvbn.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2rfvwfjzg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2mgdlzouh.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2nmgzwrlf.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2aydkwczv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2ghcqakot.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2bvijlqqr.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2dyqiitff.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ovrefitp.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2vhrdzawm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2hdqnclrr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2bscomdzi.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2bmnayssa.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2nlxjaorg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2nedsettu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2mdqucsye.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2zabiyqyf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2tmugbpwp.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2gmrvtoak.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2qvkqnwat.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2yefjongs.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2rnphldih.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2rixrrfor.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2koyxfirc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2qjpgqsmu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2mztimhor.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2bwayenke.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2viwhevys.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2hettbsca.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2obpuiatl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bysequnm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2rabjzowy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2decplnqf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2cjyhzcgf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2wlczymes.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2soamgora.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jkabqket.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2wohklarj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cnhlqgep.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2scfbjlqf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2prynqamx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2hvceytbu.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lvyxysai.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rwlxsdsv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2xdyfoqeh.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cdhdwxrs.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2brouqfch.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2longrlbw.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2awaaxgfo.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2grwwhzhg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2dutksyca.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fakvckze.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2yccwxaok.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2kpjzyjsl.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2kphtfbdl.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2vjdwixrx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rhsfzowe.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2jidptryd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2nhmppzuk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2pavhksoz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2wyefatdu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tizyglko.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2milmtvoj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2owielsaw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2nypxmvzd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2khctwfra.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2xpxsvmcx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2siqoqpot.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2vicbfyqm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2nxqwprun.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2goahbrxh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2sclbqtxg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2yqdmgatd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ajqapqst.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2aroknzjg.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2dnrzxocc.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ajollzfl.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2yixucoyt.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2umrurmru.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ejajfehp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2yfkqopxw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2drvobhno.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2mlvupjmh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2xmepnmja.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2nbecwwmv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2khawqecf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2qlhffifc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bpjyraws.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2dovylfdx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2iukenpuw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2qzjbxqxq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2jebawmgc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2yvlpjpwi.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2kwcrjgis.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qdocpubn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2npemevom.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2tjtwcpdf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yiyfkrxw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tmmxpzmi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2npvngiwq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ysvpnfvf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xbuhwqhr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2hwxqrthg.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xnjdpjbo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tsqowrzq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ippfupvu.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2yfrrcexs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2vtkuhbiw.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2tmlnufvw.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2exbrugej.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2nidgsjuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xqggwqel.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2mfwkixeg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rvvhykta.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2mbmvvaod.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2xjxpicbx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2zayccuxr.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2djdvyppr.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2nzuzjqzd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2zlwynefg.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2tucwxfby.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2okwaajpn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2rxmeqceg.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2cingsybi.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2jixyzlqb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2hlxkmwtf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2abvpmwcq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ibvyopvh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2uedqovro.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2tvjbvqmo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2csdhvxod.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2kyrcvjtp.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2jygmpzce.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2xhsebrru.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dlpbtrou.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2mwcdpqsz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2rphuzicb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2vkbtnbmk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2vozkblml.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2kdwnmkyp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2sefnysqe.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2tghnlbcy.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2zozhltrs.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2auaaggsl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2blkbkrzo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2uzypppvq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2snjvcyki.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2rqjqlrtv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2bvjyyfcp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2jcluncqj.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2spqwuvzf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2zgxbmxrd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2qwqpiygw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2pdkwsvxq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2gixumkov.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2oaeojzsm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ejfxsica.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2uzenpqvc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2myvplvqp.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2ivhutxxy.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2sdgqgnrj.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ynmymjed.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ytrbymvy.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2csacnobc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2lbzigkqs.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2cxsgznnq.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2fjzenajc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ledwumey.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2menlixxj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2dgruiucx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ubbqfchb.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2swcckyiy.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2bnutdcdk.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ofbagucm.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ssbwzlaw.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2vnbykobb.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2eemiunfx.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2kdpotfcl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2ywekorxk.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2ufwyvqtn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fizgossp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wpxdrabj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2prfczohk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2evpmkmty.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ylzdlbal.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mauioxlv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jbufjctl.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ojtsxihy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xfstojhj.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2myahmzje.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2eteqfppz.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ugfsigui.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2nszqzulg.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rijminpb.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2rwhpldtf.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zjsaoqjo.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2wssrwnak.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2lxlquvdo.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2rmvxjalb.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hdfmyrqu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2dwteljam.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2fdnjxhox.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2mlehqdlx.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ygwusorf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jljklkoq.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2jgjlrgib.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pfwfutql.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2oxqhrxnv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2mxbludok.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2euvafnkd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rnagmmkj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2jerimgfa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2epcdniaf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2qpssjhhv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2poibhbkz.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2vpwjboks.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2lnzxpmya.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xhvebidp.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2epfgpuft.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mflcbwys.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2umasxwrd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ojzmpycq.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2qxzfbipo.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2zogcvsnq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2tgevvnfa.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2zrgazpii.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hiafmdds.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2eydnsylx.html


<!-- 参考信息 -->