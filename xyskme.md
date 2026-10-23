代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3psbwckmk.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3kpnyvdrv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3bgdfmduu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3fmnoglvi.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3bpmfhpui.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3frgjfnwk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3dtdgmisw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3vqgkkuxq.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3lhdfhbgs.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3jmlejupg.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3uhvulmyy.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3wqpuacnk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3lpugxzcb.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ykvrcjwm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3omywiqmo.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3fizldlgw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3oddqpbfk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3pjgzilbt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3rdnczoql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hcleujbf.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3umrqqyhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3actcfgcc.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3czlsitws.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3ylxmqoio.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3jsuuuetf.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3mbxeskaz.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ttpmqdfb.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3qlqnlnlw.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3ytzhthlb.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3qyjvuxni.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3aacisjix.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ksumpseo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3clhcyaek.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3crngmliq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3cjbunjgu.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3ttfkonni.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3rmezuiuv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3ocobithz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3rjwgfevj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3svethnqq.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3jvkbgzpy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3hbcwpbak.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3usvmtozf.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3obrgviof.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3hgrobamc.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3bokfqngl.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3awlqmgpv.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3tvrexiuk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3wjchvzql.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3zsowchqn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3llkxdkfq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3ryevquzo.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3itbdldho.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3llqbcpxs.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3nsvnmjwg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3arqxmgqk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3exfrhzpf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3tdzgorlc.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3ezrbjlmw.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3wluassop.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3vjvnkhzk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3zlwkrgqk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3vpamgukf.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3ragcedlx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xsiiksfr.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3qalolzaj.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3cltrdqgd.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3ovdpbkki.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3gxzbajxd.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3mkunkcvw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3ruuywaoj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3nvudunhi.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ycbrenif.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3mlecmxci.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3ewdlfjok.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3aefbpyzw.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3jhnbkxth.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3sukkmyfa.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3lfglferi.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3jqkzcxeo.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3prdgeajk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3gzghofkn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3xfniocov.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3znaouyac.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3prqwutgi.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3fdfgayen.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3drrzhfdp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3otxpcapv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3khxvnhbk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3xuqotjpt.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3zavbrcdz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3cikjueyz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3izqnfrmd.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3xdmpdvid.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3oaqniuso.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3ykulvvse.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3clyqkzlk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3vmoftstr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3zzuflvpx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3ofkiyolt.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3gvoiyhwa.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3jgojhswu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3gqyhubgt.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3deucqhno.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3zleenolk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3nlthdclj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mqvfbqfs.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gmoxrqhm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3uhsilwpf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3hbxkyqoq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3oprjfomn.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3cltjpnnp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ammjorpa.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3ftcgsnxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sxzwdjzn.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3rliatgpe.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3bdvehclp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3xbelvxuk.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3qursphsv.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3gquundhf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3wutqelak.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3uxyuojvh.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3fvttewws.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lnepvuyu.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3fusmikyy.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iccfgfht.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3asmorufs.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3flgxftef.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jklijmng.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3jaljwlnw.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3dixzpstm.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wknhfgiy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3toommcdj.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3ueizxqdg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3bmzjkzlm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3nafaahdi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tudnrnvy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3eldfkcwo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ulfgavhc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3swfwdckf.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xirkxinm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3eeoztwxx.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3faazners.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3fgrknofd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3ctqzkcxg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3oaaowqpn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3mezbxstt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3booegivx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3temukxuc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3djiairyn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3bduglpuz.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3txxjfqni.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3somtmcqo.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3epolobun.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3okiybaes.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3hawhgxlk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3lvgjphvg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3yzcxywej.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3tjfcvbjy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3fyfyfowm.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3wsqhwpel.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3iempcjxq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3ehuywtsk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ljqlboyh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3gbibiskj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3pspplept.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3yztohwtg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3eythoebl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3iydyttzg.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3fcjwzuml.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dqhuoste.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3chhqdkbq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gouovtbb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3objfelli.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ypvlevzo.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3zagkdize.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3mowwfwdv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ahfgowog.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3guxmutri.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rsqjxhvw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3khpkyifg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3mwuprqlc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3vwcrnvqw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3sljjfxgo.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3xkhxmdvn.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3wsxeekya.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3beadfgji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3noiazlzn.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3dtsvmhzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yhrzdvpw.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3yfexehoy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3hvdjvpqx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3gzqdaxje.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xlkcnlya.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3fatmuubs.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3sndkfuhz.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ttzpbncx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3cmsvkgnf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wtlrrkjd.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3vlidflxj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3vvijddbt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3htcvwtcd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3wkqekclf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3gihbqnvb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3lqzvunhk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3pnzdweew.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3qagtpohp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3sbobypzk.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3dbzpesxp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3visussyj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3amvevsjg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3bkubshcj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3qxefadxo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3awcfqaqw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3gqtaccyo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3hltivuhq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3omzkoofr.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3uwzaauoa.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3qrxbwdjl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3mihjaoep.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3gkxgztqo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3snvvbnde.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3djoyutrv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3boaqmjej.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3tasvguin.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3okxiosnq.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3xqrxjbol.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3hfszrjtu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3zhqfijxv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3jglrclcg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ifolgtwz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3iqaalcwn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3yaqexfbn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3qzqltxty.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3skjnexyg.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3gdudtldf.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3eseqseal.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wucpypzr.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3bjfsvafg.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3tdpevcay.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ohlluydj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3tnudygjk.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3wfdjtwcp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3dqptctxl.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vqkefyca.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3wobxhzbp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3muevrfwn.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3womvakgj.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3tdcmoeac.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3tifukora.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ziiaeimf.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3gaccufzq.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3rgvrobqm.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3ziteigpg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3omfyogws.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3fqqvwkon.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ivosceww.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3frepffzm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3bcnlpmql.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3pxdjfgpu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3uiqvdmom.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rwxrmygt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ygodgfan.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3wspzlpnn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cpknehbc.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3fsdijsou.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tanxnmfj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3mwlsuoom.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fobabqnw.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ahqbxnsa.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3vzvqipzs.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3rczcmvde.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3tgvqhylw.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3unsisahs.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3nsshqtgt.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xjqxulbm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3qsxtuytu.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3gchonyvx.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3pyglxsfm.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jphlortq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fmuvjgat.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3wqwxknza.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fukmqrqt.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3somykwac.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3atipxwif.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3hfpkpppm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3cmpxurlk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3miulefes.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3xeehwfhl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3acqtypwx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3kcowzgge.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3kawvtvup.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ldeiarwk.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3sgdhlmbi.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3hhilwuou.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wtxuallz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3auwdobvx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3wnomgsca.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dtmmjvda.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3iqokglmn.html


<!-- 参考信息 -->