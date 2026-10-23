代发 wailian999

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3uejqqhfe.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3nlboyebb.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3eyzjjlbj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3xjvsjfyu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3qwfhbbbd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3xflecdrs.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3lisycdic.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3dpurkleh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3apnynwbw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3deezsniz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3ddvqcgmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yvhxjkvi.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3mwiqqiek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nargfqap.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3quztdefp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3naaipafr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3xbtmnkwh.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3olektkfi.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3vnfbskhs.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3fmobxywp.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3uunahfqn.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3kkwkcsqv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3vljyfixp.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3gklmmdax.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3tebchfzn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3gusroxil.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3dxyvnlxt.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3omuoiidr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3chpayqrr.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3vkpfozjt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3guzanflk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3vamlvtqx.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3ecvdnmxb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3psazgild.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3pcdkcexk.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3rrylfykf.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3tgxrgpjr.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3kztkacnl.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3akueobvd.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3xykoxrkv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3tvxfnxaf.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3udfnpfkd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3akrdtcks.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3wbntgoyt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3autwstkx.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3llwaofla.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3tvhljdsm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dewaiivc.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3qvbyibed.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3jdwjtanf.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3mswyepgq.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3fdhllhjj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3lekinxxa.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3atgzwjfr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3ujnbhnlc.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3tcphzwwn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cgndvxkc.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3wchhvuqg.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3swuhrzjs.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3yifabsxo.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3btthhugy.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3giriyapc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3uevwgdkc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3bywaedcq.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3cymhtqom.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3ikzsbblu.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3oagccdwx.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3mgmwhhsx.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3xhedckfg.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3finoheqr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3yguucmda.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3zmupklog.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3vkoodofy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3xqbyddmv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ymtsdhgk.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ywtyjbvl.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ifveyufy.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3zkiyknin.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3nopusdry.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3mkhdcvyh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3ombvjtja.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3fjtozfwc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3bwxhhski.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3gfffjwek.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3amgszjeo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3vbtjcotc.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3pqohrczm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3nvcfojqc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3mvlqzheu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3gfhcjuxt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3emhdgtoz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3enfprmup.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3icqxnjma.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3qsjmujgc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3zebtpahk.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3fyzexlqf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3bokgksfe.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3jtlhirlg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3zdbcklvk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ohayfyuc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3cmaouvlu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3flwrhzak.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3fxermopq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ppbbbzve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ltnuzqlp.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3gdinqvrd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ylbuyqsx.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jmlieauz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3beafcizj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3afbvcnye.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tgvhhgif.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3ltmqcnmm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3lwmefibu.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jodmivre.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3cyjwdkkx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kahdcyzq.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3bivqttwj.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3setrsskn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3tjwyebku.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3isfwgjvv.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3edhazftd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3bxlzzcqg.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3lfobverp.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3xajsrcxj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3zfvhjgxy.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3utfizmns.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3jfqjifft.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3gwvkpsal.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3fsebiiry.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3kbbbusxv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3anguipwj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3jytufrzy.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mntrided.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3raauujjm.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3buvlbead.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3jmvquufk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3gadersfd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3oenyikfy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3wrhitvhx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ibqhkjch.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3oyegceaa.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3btdzchqx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3vjkpsdoh.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3xedbtpew.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oacbgbwk.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3aaplqaip.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3buluwhqn.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wemhxnak.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3kmiusfbk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3odawwrdb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3xoqgkhob.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3kgxztznm.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3uxvjqgrg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3psbowszc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3buorbpsc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3aiucjnge.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3daubmttr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3fpsapmss.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3cfifzdjc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3accrivpv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3qiapmusb.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3jgcepzla.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xypccjou.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3pspyknkk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3slnkehok.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rbejoebi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pxommrhe.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3usvxddeu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3qpxahxsr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3etddtybj.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3sfkewnjg.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3elztogqb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3vwsgoscm.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3danevbsq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3wwmvsctp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3nqcoyquq.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3yynmvotb.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3klwhwpsp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3nibubyyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wimyfuve.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3kbuvjqwo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xmqucuop.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3jlfyeosv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3wglbbbjp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3msakdden.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3kmkzfmvc.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qewgwtwt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3jufuaeqs.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3hdskzzqt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3ylqqlfss.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3zcwnncqr.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ffakpptf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3nsaujxzf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3olprjcuj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3whuzmpci.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3adrhdkcq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3glcarjbi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3tgzapnvh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3ammvyfie.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3kdoqaniw.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3fnvvjbrj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3iwazompc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3ssmbrqyl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3lamztsqm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3bnjstbsy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3fzbhihkz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3hnkxciit.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3ojekwysq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3dwwqwrbk.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3yfjnzccy.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3ehvnobow.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3lxyfdarg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ajscbuyo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3eebgawdp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3czfqbabm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3tpnpocal.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3qscmeqey.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3cptuwehd.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3xielrist.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3barrabza.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ymkyzvdq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3fvlyvtlv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ewvwxiwh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3dccptgsv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3ifwabvdn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3txdzlnnc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ntbilumn.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3uttoizeq.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3rlovihmw.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3oxlsgtue.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3owwithlx.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3bdpmpigb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3xwwtccxq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3pbxkxuhn.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3ouyhdczk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3meejtwsv.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3tmbrqifk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3gtoloqjb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3rknzmynh.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3xzpphpnu.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3vyvhwgox.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3pfggybni.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3voclzpfo.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3kukddshc.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3dzgajmcx.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3vpghupnu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3wqblkwsq.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3gsshqgek.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3smuiwkve.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3sstngmea.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3mgasvzhg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3qtltvmnt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ieszfokv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3esxaslmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ppouvfqz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3rmsehvbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pqmpbyrg.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3lfxojiew.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3rtkzgrsv.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3uqhpstaq.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bjczlslh.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ypmqdbsm.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3xrxngnom.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3xuufxsaj.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3kbsvtghh.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3kfsbpuil.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3eaqgcywh.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ifnbknqs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3efzmntaj.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3atdofaou.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3rcnovghp.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dikhcafw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3abqzrffj.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3farzrbff.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rhjqgcgj.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3rmppqjay.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3bqsccjoi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3rqpicypo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ilpvrcmz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3aeexqxru.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3fyfbihoe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3tcanvikd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3lobtgzzv.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3iuqxgdfh.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3loadalhm.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yvsryjkb.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ctuifrwg.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3idwkhpbc.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3pbklfszy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3jzwdinkl.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3lqdxhpdy.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3szyhlppn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3fkchhjev.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3bhfrvfaf.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qcoopmwx.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3uvlrbovr.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3snuepzvu.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ssezvtmr.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lsufysdz.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3theoqtiy.html


<!-- 参考信息 -->