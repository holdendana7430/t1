代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3paqimjit.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3gurapucg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3hlhnlcoz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3nfsukdqd.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3avpzplpr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3hualsiue.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jvxxbqzz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3fxwqnemj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3fqgagdad.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3nfefpncv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3agtjqyit.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3jznqcibb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3iusqxnxh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3poocfvdz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3usmuqdcj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zbsognxc.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3exzbfbvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3risqgfgh.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3guftzqvs.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3bmydxlgw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3iwgczxvu.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3wwrwguad.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3qnpygixr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3fjtraenl.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3hknxdgjo.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3mwiwofed.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3tscpvjdx.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3yjgtstbs.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3wuaprsef.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3deccdxfg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3cjpczvzg.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3dptoqxcy.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3fxjsuuzx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3hdvovumh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3firlpmsa.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3dtjcezrr.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3otkbdemo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3berfzfow.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3ljixguel.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3xgyhofju.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3sgzbfagn.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3iyhnywhp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3buahxbwr.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3czpsbwcu.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3qijnotye.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3azuquvsd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3bqvkjenp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3iyteveme.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3gotdaqie.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3jijesvtx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3xwzdmfxw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3wdqpscma.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3zymdtecw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3sfqxgvho.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3geuooenk.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3xoliyelu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3rmxevnrz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ygswydou.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3hikotild.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3oizrbljl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cksgnpve.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3toamjidl.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3kctaxseu.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3xuvuohid.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ecxubtjh.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3urdwesuz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3ptdqzgld.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3oetojlbw.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ywbaywlj.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3ztodalrz.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3osgosjvq.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3ebbnqgqt.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3inodfnzm.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3zotqhkqq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3qknlpbdh.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3auujwjmg.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3ttfmaicr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3avrcxcqh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3ohvnfsap.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3uqxdlpfv.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3yowqpcyu.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3pvrhmyit.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3oqcccqcp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3rgmidrjg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3nqwqhsxg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3yzxomoef.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3ksmlswtf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3lhivbgjk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3uxdfjigo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3lmrjgddv.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3ggjuwzwk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3gkztsbll.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3dlyhsnsz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3iubikqph.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3iodafcdv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3lsxvaowk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3sjmeltlm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3rmuqnlhz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3cvhgpoac.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3ewtqstqw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3uthnxxjd.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3jevwgxfr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pcgouunw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3srqntiak.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3dapnghmd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3dqhdbdta.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3yxlwzlnh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3iauagspd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3crvxkurn.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3vcfitezm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wvfsnwbt.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3flvwonhc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3lznhxzzd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3gcpcynnc.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ztyfogae.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3sipqmadt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3rphlknkh.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vuutrcgh.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3jpyxjeca.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3hvswcvrb.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3yncyhhwc.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3tbynauks.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3aqgyqugg.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3zunleinq.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3pqjybius.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3iiphorcl.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3flqgetxi.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rpztgbnm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dynpbrad.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3dwveqlnz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3lctebufn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3ztgiudev.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ygfbzfdz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ogdfewzm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3mcoljkct.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3ppxuvxms.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3rkfoajnv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3xeuuouad.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3mgarialt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3fayooveb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3nqqtslxu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3njjblfht.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3jhvoofvn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3pwcfutjs.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3givvirye.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3jpethzew.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3wvkwsify.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3rhauqqwr.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3naxquwjk.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3bpxjuatt.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3vfpjcwnv.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3qgrgbsax.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ijkuezys.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3azgtufus.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3cbpygjhy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3pbktbato.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3bmohkdbq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3nsyyydny.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3xhrxlhus.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nhjurguq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3tqdjaegm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3zrnuopjx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3cvqtfgdx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3kjwuqedo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3eqhxajax.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3padmjdbr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3sfdgerxb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3laouaorh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3esfvnbnh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3onseavrg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ykdpjwoy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3ggbwrrna.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3jpownnik.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3nlxjqroi.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3dcvzeqnq.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3mpiopthj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tdaheqiq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3frzogevr.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3cvuaqylf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3zieafxau.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3fnajfelf.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xntxhahc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3peaymbsv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vudutera.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3hbhvysgh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dxcvjllq.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3colhfqrn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3wjneidzg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3eqjgafrn.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3axvayszt.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ckvkpvwi.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3rntnxbsj.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3xnvnadop.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3asnrsnef.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gunydhso.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dftjhbtf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3yuroqefm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3xajjuled.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3osyzyodq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3eebipten.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3dzxuvahm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ixtgzomi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3bawjxjko.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3qornezvw.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3rkeswpkv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3nldrtsdm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3voxzagru.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3muapeeum.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3usueuvke.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3pzwtqnlc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3jaormqyn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3dzxkfhyy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3pbxwgbsp.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3oqirbhyz.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3bycreyzd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3pbxbisfu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3vilruqnn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3lyedlxca.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3gmpbavat.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3cuimrtik.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3dpgtxvco.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3oirpmtrc.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3yhqenreg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3pyhltcob.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ajrlebzm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3fpdqmluq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3tvgniree.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ededgoor.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3dsontywp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3efdxhrjk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3grbfufpm.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ocskihpk.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wuouaeys.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3cmjippgn.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3sveivhfe.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3oeygtwcr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qjwlmjqx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3xejgbzlf.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3mjluktfh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3dgkcmukq.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3nafuhlmt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3zsgsnsdt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ssrldowz.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ilrrsnqn.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3kkeppzgj.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3gwpedsdt.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3jawlyscn.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3flhktfdr.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3jthyrvtn.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3yjfavzqs.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3kmugynkc.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ejgjdofn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gbjhnuyc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3orylloqa.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3ntxrjysy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3wjpfzmjp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3xjpgftij.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vhwtqdlx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3udjhmzkt.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3gqkjpvbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iyficgdk.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3bxmcyylq.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3qdkbkodm.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3bhltwxon.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3jkkgycqb.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ewckosec.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3oufuzhjc.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3bddmxgfu.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ouzbazds.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3jacaobfj.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3rvjfjuch.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mlvamlyd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3grxpmvkm.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3yuzvcgyr.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ldspsbgf.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dgzcplbf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3yprgfbtv.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3zjzytlzw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3covzfrtg.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3qomkvitc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3zrpjxuor.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ckglnest.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3vopexhdw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ugdnxogw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3agpdzcts.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3rxequnut.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3divfrcmq.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3maqppkhk.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3goihunsq.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3skwzebbg.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3lpbrlhwv.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vlqzeirp.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3hfpfyfjj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3afuusydz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3arkclssz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3mzngwgjf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3eooeptkj.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3fpheosyf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jldryjqh.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3vtredsra.html


<!-- 参考信息 -->