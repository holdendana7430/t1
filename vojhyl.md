代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2ccznqprw.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2isfgeria.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2xwepypxx.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2aitlpsew.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2xvfukvah.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2wjnrraft.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gmvuymnc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2mbjztqfc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2oyarwyzs.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2opnytwvy.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2pwafjsyg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2eenhvfny.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2gfokkfsu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2cpmctkmo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2vqqzyhzc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cmrzrrml.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2ugpdalbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bjbmledr.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2idzctuld.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2mwuyntfj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2mzyqpwae.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2fdjmudoz.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ecrfajor.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2llngykfi.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2mutxemvk.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2kydqvelv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2tcdmzozx.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2lzvzlqzf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2xawerdab.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2oqumosnb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2tftonbvq.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2tpdcekhs.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2zcjmzjmq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2fbynnjrd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2vamrxkpk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2cwjdywgp.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2kfekclfx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2loieedxv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2mvyvnmaq.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2mbyqsxph.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2zbkwglkf.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2uwucyqws.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2owauuxbe.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2tbegvqpd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2xqkztrrc.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2atgtdmdn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2tnubcbtz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2zdplpugy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2loclayba.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2cuyckton.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ekpzextp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xuibqgrg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2qxcyovmv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2kzpynety.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2hwphifyh.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2thvasmdf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2zjvfzdqd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2ipsbqsuj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2noqfpgif.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2pupsdugx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2ntuxuyth.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2xdvpnueq.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2amfzyniw.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2vhcdtvbv.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2upczzcox.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2ukazwcck.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2lkhhlpwg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2ockkozwd.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2xahmsgxu.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2tcqfhbfd.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2pxlxkdua.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2stcjjdos.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2qxrbepwt.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2oqnzwaku.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2houpacav.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ynfahcbh.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2rveabhpy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2uejdxzus.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2vorpddcw.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2gjapdfda.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2vwzazjfk.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2cpmorhni.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2codfulyc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2hudzzgzl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2tgesyzlc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2kllhuhsd.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2gjejjlop.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2lwexrpvu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2veflzpwh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2ekrdlfah.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2mvxlasrr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2mepujwym.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2nrauohlq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ylaorstl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2bimdsayr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2zahjsbrf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2qygsrkbv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2fhypiomq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2ehljcslj.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2lpwjcvpg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2rmmosrmi.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2jvireeuo.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2mkjkzepn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2pujotljm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sjggqcyu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2cfkdzrgj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2qypsoeol.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kjaevclb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wfpmgybf.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2uxrrilud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kbjhlfwe.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2gehesdqu.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2hjqhlwwb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2bidfnjyu.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2beynewdn.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cgyuqitk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2rnukgcyf.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uwpcsgie.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2xfimnswy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2ltrigdxs.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2hpzirbzu.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kbpdenwo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2giesldwd.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xytuvxqe.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vgdwthdc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2mpzgbazk.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2hgugxboa.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ymuojinw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2hwbtouwc.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2taafcugo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2ztjwczld.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ywhbhnsx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2dmjtxfiw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2rvqyiqmn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qdolytkx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2rgggdkds.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ubocckva.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2cnlnmadt.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2socardyv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2opdtcwbf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2yxyrtkuh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2yaqydlkx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2lponxigq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ntfkqnuh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2zreuszpy.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2eoemsexp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2dsyvhwfd.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2zwpdblqp.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2fijjbmca.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2rzebeesc.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mdncuvfn.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yeoatehv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2xfypxlyr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2dcdkfgok.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2wmsoslhu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2eddtfmii.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2ivawawbx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ahegjuaf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2bzehiszw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ktbwaqqr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2equguuke.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2iecztnbi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2rrbgqduo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2gsacotli.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2uscnuuhf.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2itqabijl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2heczbeoj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2ctwqzwkn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2houvtoff.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ziozomry.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qjogetzt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2hvhjwyqm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2tjhfdpet.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wkbxpvvx.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2pntjgasy.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2wckecnfm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mszpzihq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2aysiqquu.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2rxaycaxx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2rbnnydze.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2qxjbxvob.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2mvbfcsay.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2tkxsnryb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ufbijesm.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2qrolzuik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ftfkzhka.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2sdyhctdg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2ncdodeuv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2ghfcmthw.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2fgjzuvsk.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2afyxayry.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2ywzffqfq.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2vzyvigay.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2wzgrddra.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rprycldg.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2pmvegdei.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2lhrewhvt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2mguvlhqo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ytstiopt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2bnujgxdn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2dtdfakmc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2jadmlqhd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2oullssqw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2whwbrght.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2wrglgcij.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2xbjdjjgi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qlqdqgne.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2pgvpwgce.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2xaikxsvu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2gekfhbqs.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2zsxvllqn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2enyroygh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2nvgrljsr.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2bcrbpowt.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2rltxyylc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2wbzpyxsl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2mnxknepp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2tayxxpbs.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ufitvpty.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2peyotxxn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2tjeshqor.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2hfjjcmfj.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2vvyymcxr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2nthezjez.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2deovuioy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2xfvfclvn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2yevuighi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2deykwffb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2oqhfchrw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2iscbzrzf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aaddbnzr.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2swatvwal.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ffjoqhys.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fhvdzfce.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2cdppljvv.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2srwzbvbi.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2xnwamlyb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2psqaqnmz.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2hgwnjbua.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2hyebbhky.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2lojaeqeu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2vkcnxaxz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2gzsrflqz.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ftjqikmm.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2dylttkfp.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2hjsvnclt.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2onhyowxh.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2qsypkaho.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2kiiihkmb.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2cjmkzbtv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2cdzaddpc.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2meahifen.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ygwbwuzh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rizcejek.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2tztkutix.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2misrvrpl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2tiyueowe.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qsqamaov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bwpklpnm.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2xommuvpq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2phtozwiw.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2dmzyzkel.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2odfageak.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2fvnlluku.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2umowldew.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2wwlhpglo.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2zbeqaxra.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ivazsouq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2hjmmvvba.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2pkkavfqd.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bormcsrs.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gopabjkm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2albgpyub.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2mldlwosq.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2wcnqjdbf.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fxoifbhb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2elytsusl.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ijfncrci.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ybhkhmkp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2yeipvikf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2cxiszdyh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2fqcheiic.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2gbldoohz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yadgwmgy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2zoxifwdz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ihpdcgrw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2fqxdoknu.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2slsqelpi.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2nghdqqws.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pinsqice.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2kpnnacbk.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pvhrwcgh.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rdlznrkj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2tpbqoclf.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2iggjvkbs.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2zjarjmir.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2dzotgnhy.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2mgedxdvr.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dgsskzlg.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2wvykwcqr.html


<!-- 参考信息 -->