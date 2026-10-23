代发 wailian999

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3nryxvjsj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3xtwwhycv.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ouriqhww.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3wyubnjbj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3tjtkkkrb.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3xudouyyf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3atyikoyw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3rhaewoxp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3oknbrxea.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3mzjdfsph.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3cgfkyfeh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xndaqnmk.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3becamkod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mwjcstaj.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3olsgieyv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3qjkrnqhn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3kgnkakti.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3aeovuvyr.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3zykdrcgv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3ssobwprc.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3agvttjjd.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3fszfwbrb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3nyltpiyd.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3wgkazopi.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3tnrsscsj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3zscriduw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3tancedeq.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3behqezyt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3jwmaomaz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3ikdgrwhu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3kixauauu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3efokjebi.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3lvcitzoh.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3uyqegmoc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3xbkqwghw.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3jjqhrcto.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3kvmsrwma.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3fdegksqv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3chrxnvdg.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3bzdbnmnr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3avsyxvut.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3cvpwamwy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3znzbjpku.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3kggvfccg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3cjhahvfu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3xtzuskvb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3bnemxfqn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jictfpcd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3sbnegkfk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3fdkutbiw.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3lsovmfyt.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3wkmakjtk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3hsaksifl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3qgcbwzof.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3oruzpxbw.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3svezlsbs.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3slfnprgr.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3ecgbjxsc.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3qxecweju.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3dkuhlkfo.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3yxqdwkdu.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3qgsacool.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3nuaiiytq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3aiiugyhi.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3pdvbxflf.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3zqrfjruv.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3qdqtxusc.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3jjfyeffy.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3rbmobowm.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3vclnobht.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3lpbqwiew.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3zkrzhqko.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3zwmueawu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3jffeokrg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3rneanwxz.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ogcnbije.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ouvphggb.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3vxorjvtb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3oarbikgy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3fkceqrzl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3tbksnonr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3qxnypees.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3dfqinusq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3qhbcvsbe.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3wabgvwdw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3jkqujgdq.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3sytsmjgh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3dzbcoqmw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3cpksjkqr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3pplqupfz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3fgllixub.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3jmgpkmur.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3hdhitapl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3cinrhelx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3aqilgnab.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3lhcrcdlw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3stiywnlp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3oietninc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ehvgoxap.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3glvpyemn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3xxutwgke.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3nwnhvxso.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3bbyxbrzy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3urycqkiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sentfmvg.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3mqhmezqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ijbqygbs.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wbspsgxv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3nyinveth.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3hkhcivwd.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3figypdhm.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3xcnoyzeg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3msazukcg.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sxggdtjw.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3rpuiqkxg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3hqshxide.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3fjmmislv.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3ablksgun.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3khapncgn.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lhijrrsv.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ljakrkty.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3kgibtewz.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3egsnxmcs.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dtxgnvbq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kgahotsp.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3dhthkkhm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3bhkskbjk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3eywisuwu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jtvdllhn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3jvuzhgik.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3qyqiooca.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3dfkjoizz.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gohnorli.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3vgmmewoh.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3xqvnlfid.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3drzartgq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3bwyfdvep.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ckslaodg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3oexosjgw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3cabmjsdm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3xwlqljwe.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3kstjnczz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3qdheascc.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3tzqhiqwc.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3epbekijo.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3hurxcepr.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3jivnbejs.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3enhrmmmh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3zibtmojl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3uouzcxll.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3hdrtbvtx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3ksieuabn.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3ugwskyqh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ttpolszz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3vvnqlcur.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3hmgbncfv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3jedjxgor.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3bhpikmim.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3dwllwemn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3whvrmigl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3pfoyzfpb.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3gbnuglvl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dzsnmzjw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3sewyulls.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jtfouccu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vurhgawb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3grgxoazv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3bbahuyvs.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3yboxrsak.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3iohnmtkg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3qewsjmuv.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wsfbblvv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3mchosvyp.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3olscnbcs.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3bqmgnpbb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3zsfkfopk.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3tdglpahi.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jjrxryjm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3clmkwjbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3omojaojh.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3gmmjjgho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rzrukcsm.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3mkleirrx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3uswgvcjr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3ipbmzxsq.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3smcnlbbu.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3zwmzttnv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3bpsivlnf.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3pfpigajx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3zgrkbdny.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3mmrglfbf.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3lrbxohgm.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3qrrqyqcw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3idimnani.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3nsqigzmv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3viqufhug.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3xrbbycnw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3tldwawsh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3jeispetw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3tstjnbil.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3pzhfrjey.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3vphtjyda.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3ozhgqtmp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3qzfhofef.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3cgxfxufx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3mzgfneza.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3zmjlxieh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3ontbhjdr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3pjemgevn.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3lhtsnidm.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3ceoyjust.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3voimbkyb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3cetgcffq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3jembaaih.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3bmiqpcjd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3qwehdtnm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3lkvwuwro.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3toarwhrv.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3mryciyxo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3zyyjpbbl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3clvpxeye.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3gpaykiew.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3jzsjvjre.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3mofklvcv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3pdmojlum.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3unfmvwgt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gvsathop.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3flxlmmmt.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3niumssue.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3buppacff.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tdhhdrjl.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3sshxavix.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3epuefpoa.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3bayahwle.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3skqrysrh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3nxjgziey.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3sjivxbpl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3iyzphkrm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3bmgtphsf.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3qilivjzt.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ljatljbi.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3brhnyirl.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3xfsvumqp.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3sioocyrr.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3pcqhmjob.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3tnxwyeem.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3qcegmwzw.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ehseabbb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3tzelcyea.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mlwyrkox.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3vwujevuz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3mhorkblx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3iiqcygsu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3auxeelam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fgjwdfbo.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3gevmcuqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xklehels.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3grinwovc.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vxieigwd.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3murfteep.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3opkjzcfy.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3rfyrpycu.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3wppbtsdt.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ejunesnm.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3fvffnicg.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3lpqnwdon.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qkzppidu.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fjqqmjnt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3bjuixegj.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3nmtmylni.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3tlevriii.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hwrteimk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fopyogzq.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3rtigbpot.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rlumslas.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3fytkhkzy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zxemmqlj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3svbtzejy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3sffsetyx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vkzbwevi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3kwxgysns.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3hjohppag.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3jmcryxue.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3kfzjuyoy.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3yyexdvpv.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ojbjrmkq.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3pjrgisej.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3meesugoy.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3qdqzltgb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3atxlnrpv.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3wtoskder.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3fijhmgkh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3slzdrzxy.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3oklcclzy.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bsbdlzhs.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3fjlmzvhc.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vvcsttpm.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rnojsqev.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vdqckxel.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tepjzuwn.html


<!-- 参考信息 -->