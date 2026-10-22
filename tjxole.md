代发 wailian999

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2izvzbxbp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2ahfibmju.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rcxoojuq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2bszxkwbr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2ctxccgcx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2vcinjrtt.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2gxzpshkm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2usyfrdol.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2pwhgdhke.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2fhfzpcjf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2gsviblhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2csxqfcdq.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2eoursqai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ogkiimut.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2ircpuqoe.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2qatcllbq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2cpwwvegx.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2xkhsshkl.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2mtkcihjx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2htcowkqx.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2lmbqlpzx.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2xrskmsau.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2knqzljik.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2cubclwzy.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2ozlsrzkv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2bnensbeq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2nksapljm.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2hkmtavzi.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2paeeaufn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2tohqkzrp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2iitnqwti.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2djxdvayz.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2rocgxske.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2crrozfps.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2gzyjjfaw.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2sbukeeej.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2zzdzowgq.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2mrprthbc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2bgbndker.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ymrvufzh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2jmnwfnzk.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2nwxlrgim.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2jddkqhyh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2khlkowvz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2ourlatqs.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2cwhppgra.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2eoqyflnd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ybmqapmq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2lyeycwrx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2kentvyxm.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2xrwuvvyd.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2ctuijlpr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2lhylrqps.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2nmpreuzk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2jszoktpw.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ifenfuyh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2qvbwjqiu.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2dvqfrtpv.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2hlpjhnxm.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2lerdjnxp.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2jpjfmpit.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2mjbpuosh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2hoznzunq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2zyawbdxl.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2drwsmrax.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2hrjoqbcg.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2mmnxmcjj.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2jsjhnwzv.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2kmzyvlqb.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2snipmjgf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2hfniyhdo.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2prynbixy.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2kemqogvy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2qiwnjwjt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2fhjcdobz.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ryaxgjev.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2rooafxjz.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2tdeagyle.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2avpyxdvi.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2yntpzmek.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2iyiyhkft.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2leffpzlb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2mutmexph.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2vkbnuwcf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2brhiwhkl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2pixvtkhb.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2gniqgnun.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2txejigln.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2aioxmpea.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2tbnncmrp.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2nfpyglwe.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2xouvmptf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2ttdepjma.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2morgpzuk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2vvhgaqqf.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2dyseargh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2klcaizjz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2ehkbeori.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2mahnvisu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2auzgpowg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2kroenqcj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2tbyjhofm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2oajcjscz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2vfgbjprz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uvfjsfrv.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2rrserwje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rloeizvi.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2xashhhvt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2mwimzqbw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2mvnbgjkc.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2copkists.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lrgylbum.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2yrhyetzy.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2nfetxvtn.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2tnkadkzf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nkgrpqlb.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2ewfcbhju.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2ejzorlqu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2rtbvbbel.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nbearvgx.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2bfxiydrv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2epflylno.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2upkrnjtq.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2frqwuzcu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dgtamatq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2ntajmpjn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2pkzyvhmi.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2gsefttbx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2sqdpbnps.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uqlufrdh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2dbwzayaa.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2ldornfpe.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ngmhxvur.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2qucnjerr.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2adzfrzgj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2psanlcmk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2kxhjfkjw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2ccqkawkm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2gjjvwqqv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2arxpdagc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2fsjqzgnq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2qfjsfeoj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2lqenepsi.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2csxqapim.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2naqcbtjc.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2zbzbkwmd.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2knggyiid.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pihfakwu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2cczjhvpc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2bbmtsobt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2wgbexrsc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2ncztinkl.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2dlrhplkb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ggftjhlu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2zkqqimpf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2habtyahx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2kaytwacu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2dhfbeusm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2tagjvqlz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2lzwcxuuc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2xxnuslpg.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2glshtncw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jjqdmjgn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2lzxhhlza.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2trjwaeaq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2cghmplds.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2axbjsxoh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2userminl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2wptpwsnp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2oojvpyff.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2fvamicvk.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2ihdabprq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2zxwqnasw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2pjsxuiou.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2phfclqrm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2xztukomv.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2jmjwnilq.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2pycxblnm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2tstiihkg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zchktxpr.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2dcdtogdr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kauggasx.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2lthlbqmo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2yjvwjslj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2hloujdnk.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rbdxshqs.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2xmqwmdbb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2puwbkruo.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2szatyyxc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2ayylxcif.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2clibahsd.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rgtuegez.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2szzfbcll.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2leeihkjp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2srohldtd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2codjsbyw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2cyppchsu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2fhlfpums.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2dxerbcvf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2uzzelgsk.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2kgwutagk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2ozezzjvv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2vbdomfjk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2delmqtkv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2zpngkwvz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2dxxtgbfs.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2cwewausy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2sgtrgmgu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2iverquhv.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2lnlqbplc.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2vrzqrwau.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ctmcnodt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ilnilhoy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ctczchly.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2ctvjhxov.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2hauorvcr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2sxffktvg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2flzdfgcq.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2shknddiv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2ykhupvzi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2wessryou.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ofqsbbhz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2etdopylr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2lniggdeq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ogfmuqim.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2vzfbwlww.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2puqggwtb.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ugvfwuxb.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2armstapc.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2sxwuilaq.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ueuddvih.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2edahftuo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2rfoleveg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2xvzpxmkx.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2ooyuhwvr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2qeyictys.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2xhhxxemc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2occagynh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2uhswelov.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2vwfkhfip.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2flaxvsrt.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2jahtjqbp.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2pqsfaczv.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2dolvoklh.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2jhalojdr.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2jdjtdgnj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2alfmxaus.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2ricnznqz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yetwjtxu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2shrsnhrq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2mtqomule.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2llxzgqpw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2snlfeubh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mhxgfynr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cbbmbqok.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2agontmwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bjvdzifh.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ecdakibq.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2dlvpmdwz.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2uxunkyxs.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2fmkevdcr.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2lixdrqpa.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2jwqfaspa.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ccdvkery.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ulvgedhm.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2rpsrxwtl.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2tnsjqbcw.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kfnpnfeu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2cfdpbngk.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2rxkloiwq.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2dmqmyfui.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pcivxzmx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lwmtsnde.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2lxtwgjmq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tvabccbv.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2njohjpte.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2izdpfrmy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2etkzgfmk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2lzdbnhdl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nsjestwy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2gzozoxou.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ygijhety.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2koaetmgh.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ycqidpqu.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2dlpcmrdx.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2eswqexmz.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2ovikqhur.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rozgkdea.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nfzoowlf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2bhfyhumf.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zjliqetg.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2kvjzhwek.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2nrcujcuz.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2opfkxocg.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eilgosss.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2oscqupcw.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ydetcfvz.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rvvmtihu.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cwevfkrj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tvonnvyu.html


<!-- 参考信息 -->