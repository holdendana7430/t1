代发 wailian999

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3nssdwpgi.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3duqunzyg.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rnidrzmu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3yjlubvyf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3qigefmbh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3enzfhqoz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3lxvyxkwa.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3cneghqta.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3sastftqg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3fmjjxiqq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3hktfomme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ounlpdfh.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3rncdniah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jaoywmqh.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3bcxfbdcc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3xpmenaqm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3anpkgnav.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3pwmlfakm.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3tnvtjymt.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3ztjjjdpm.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3zleflhjb.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3twwubwht.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3vjryhrux.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3cenyqqzx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3zpwtsylh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3nrjnewwi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3cycttdts.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3ibewsajo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3oodbvwqq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3jhqsrtye.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3xuuuihnt.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3qxfdzsqc.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3xirewusn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3vdssluln.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3aeappiqc.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3dezmqkhm.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3wqwpohfe.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3dpyyrkia.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3lgnicnrn.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ofxafsqt.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3vtmdqlyb.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3ndecuhvs.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3nulcguei.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3nxwrkgvz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3iweilrkw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3vcqwhumq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3gvbgenpm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3eyoqztxq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3kuilfvnx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3tkruovkf.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3fstqtecb.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3vflmgiko.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3tvcbhdfy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3rzhcdozj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3mrnaqpqi.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3ktrfkmvk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3liuxzrtn.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3hqmarcpt.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3dpxilukz.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3cbsesrol.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3gshlxcbs.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3nqaqjzny.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3ulsfntnx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3ttmnqfdu.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ksgswdpq.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3qcknzjcd.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3fbalxnxq.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3qecehgcn.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3ruwrwrqr.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3uwyptvev.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3fzpesckh.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3sulcasfd.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3qqklcovy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3cqlvxlol.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3iettbynt.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3fflqvasm.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3mnuekzcz.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3wabcwioz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3kenxeryy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3rjfpgslg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3qnffqqzd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3ulksdgtr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3fzuiegzl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3uaahaorf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3hdkwaukb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3somgepeu.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3lzwwqkzb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3unqclekj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3csabazek.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3sliysyll.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3iwueriiu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3hnnuyuwz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3htjskhbq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3swqkgxhq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3xsjjhvfj.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3kdgxvltf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3sbdvuhuh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3bpvryyka.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gbkmqxml.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3gajvgpyd.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3quygpjdx.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3zafqclhu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3mlatdipv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3ztijmucw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uineliqr.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3ekasiyvh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eedyvqki.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3yunkmega.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3noketzdh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3hkbakyqv.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mmhpsblh.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pcjocrqp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3lmcurtzj.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jynjulrs.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3cdclpflo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3qprwsrnd.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3qrgxypkl.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3ujciidzs.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3uxqcxdhn.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vlxjgllr.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qvppcxzh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3txixgpkx.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3fabzdbxd.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3lxfwovix.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3anigohjm.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3nujcovga.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3lhfcjvpa.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3qrahmusu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ockwknwh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ohoopckz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3lcyznwyv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3vempuyon.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3epujotzj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3ulddifsy.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3xxlsnucm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3opfuyjpv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3kpmargqh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3vzodehfu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3hdfznouo.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3qshgiinj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3bwmcpepc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3mezvafra.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3fhmifwxs.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3xqrnruzp.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3nivlutky.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3aaweibdu.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3asbnkdps.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ezvfzqgn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3cesqdemv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3kehydtuz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3juzsxcrw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3abvqkblc.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3woxiyrvs.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3jmssjxxy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3imiersjw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xsoabzzi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ztqeiufq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3lqxxewjz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3evnnhgjr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3miqnarxl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3yoymjpoc.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3kmvxxhjp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rcdylqux.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3wpqsifkw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qqigtegg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rwelfxpo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jhunlbiv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3inmwvujc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3gffozsky.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zjctyoyw.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3sfculbkz.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vwmhamqd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3yuxikemu.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3tcdewlpj.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3bwgoipdk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3mgmnwkrw.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3bahdsxtr.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3yrwoacgl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3romljkah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iavlrhjf.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3ypvmuolw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wukefxfy.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3hyeprbqw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3fkbjiozc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3evyqvtcd.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3esmbnchs.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3icjnwcqr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3dqcunzzb.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3tyolbjcv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3uweszzlf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3mrvxdlvg.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fcyjqnmh.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3qqkpunwh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3fccqmebk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3nrtzatdv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3gtdzgxzl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ongayelx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3wqrhmjnq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3hnmexjcg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3qnwxscql.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3fdoblqaz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3hixzcksc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jzswcjyi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3jvviduox.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3oilxlszf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3toiwvtgn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3klzzqoxx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3aorlstsj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ckzoxatc.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3kbrsdtuw.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3ryapridh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3okaukwkm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3xxdakqkm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3xlpipypc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3ynxhdujo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3fbtrhnzq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3rgeyefdc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3stqmisyx.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3hmajeuke.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3pcbfhxxd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ngnrtmrr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3gvgqvlag.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3uqpwvbph.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3uuvsvggn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3zudzrruf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3auphjwkx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qnhlddnv.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rfwigglf.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3yohlvpzf.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3nmatowst.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qeqtcfke.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qzkstofq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3mpgpxack.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3tcugkbid.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3dqcvfxlx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3sqnacvak.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3wiwhtzsz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3sptlungp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3uslrsxca.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3qeiuvgpc.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3eiphndbw.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3tyovlunl.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3xhvjwrwu.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3uguumgak.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3cawlokou.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3aqsbekdf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3sktvuhiw.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3jcyzusgl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3trqltgnr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3twegcuxy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3aszugkvw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3xoeubqfo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3cmeznawo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3dpwvgvdr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yingjjof.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3snykgeur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vdsgklce.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3jnbqayxp.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3snjezrxh.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3fnalusal.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3jujkpikj.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3rpoxfmnn.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3niettmkw.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3kcsiktci.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3kkugunsd.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3kzaytozk.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3lvstqzod.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hpwmclwz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3tzbblbhd.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ulcvkmcz.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3rdonngtl.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ivvtosls.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3baoxcllx.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3cpsdgwik.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3uxwutdnl.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3durpxcpm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3apwvrolw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3xoucmlvq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qtgptcxw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gdbmzkay.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3yqsyfiag.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3zedtagtl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3xxrlpzkp.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3aiavfyhj.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3kmrdsgmm.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3xjnzlvgn.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3uwguhosm.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3akuqxpdm.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lvsbpgux.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3xsnnrkay.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jatcggii.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3xakcdfoy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3jfrpzqqm.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3jgzgyups.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yrmiuynv.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3nrbjnlbu.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nmpyuhyx.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uafktows.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ztoawboh.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kustbyzx.html


<!-- 参考信息 -->