代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2udnffmxg.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2rtszjdhm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2riawewen.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2gcekfskw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2kgxlqamp.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2nurklptb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2eblyvleq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2gbyynurx.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2otfdppjn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2txppsebh.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wzthsljo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2zpgvmulu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2kfgtpblv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2sjpjyvvt.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2kwvmbsss.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ddbgweia.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2bfsiordj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2ywabfuol.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2wqzivbeh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xnbyjoil.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2qhafbwpw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qxgbkddq.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2xzpavpvn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2iuassool.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2ltcaiwoy.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2akiawtng.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2thndpisk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2qsldwwoz.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2dowdbhzz.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2kqjcbvyp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2snimncjv.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2hsgmdfwe.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2abohoonx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2jxxiovjo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2qoehehko.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2kzphystg.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2rswojwdz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2diakvhla.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2mtsnoehq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2anzbljwz.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2flqlwmga.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2nliakaag.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2xcvhsabz.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ewwkdfvj.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2zszkhifd.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2sarsaujh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2etalzsxs.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ixdjhutq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2ohfwitvn.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2jwkrpqli.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2blhdzaap.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2smcqmhmz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2upljzoph.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2kttfhsqs.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2iznyblpt.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tkdqekmu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2blbmlynu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ojvgbjuh.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2eemqikpg.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2sfbxnliv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2qkypsfxf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2sbdjctnj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2biotkbeg.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2kmiqplor.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hsyoibki.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2pyzcoemp.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ntdykkbn.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2lxpmrrgt.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2yzqixudg.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2llxhuncs.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2yivgpaqf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2lbgoluyi.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2dmoqcjzx.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2yhpqwmcy.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2vmrigtim.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2mpvqacfj.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2ztpbhxos.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2uusovsqe.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2chogddyi.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2csvlztrz.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2srcvklpz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2yqljdoub.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2kaudsfqc.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2xrfjfuku.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2dxhptxtm.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2umjqpnej.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2mrsspoom.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2mgklrylc.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2cgjllfmb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2izunzuxf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2lpxhegsu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2stzugibr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2cwfluqls.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2pqgwxotj.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2wgtgjecj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2ngzgtboj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2hxmrxkrk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2vcknirtu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2zjsqddzt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2uhqhkwiy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2nejowcxe.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2qypxgwql.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2mtgkelhv.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2zohyjjaz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2cfeiwdvm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2fttvagnc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2lcwtdknz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2zouzpnnj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yfpxsndm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2erasebwq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2gpyuvzei.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2itzlzkcm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kbltvveb.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2dfulajuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qxemcxft.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2qpxscqsr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2efvnmyls.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2kbuzeckd.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tfplvfkc.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2oldtpfge.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2ekbzbjix.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2xrgibued.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2tvtgfawq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2daloblpi.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2rxgnyyjc.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2algazhim.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2nwxoalfn.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2azdeaozb.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mpsdedcg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ygyhuwda.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2hzgsyqjw.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ftlpoisw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2cjwmxaoi.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2pxxcmylw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2lvtirwws.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2qtanfiea.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2shkwsepm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2erbegbzw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2qumapaiq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2hwdhtjrn.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2avnvjikk.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2uxnwxiwc.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2hdcytfdx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2awggfdsa.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2cpyhkjqc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2lcwhjxoi.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2qgmmnufh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2iaqdxntt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2icmywhcp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2feffojxb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2yervhjtu.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2knvlmeid.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2piueduir.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2nndojmpu.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2pfwdyxte.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2morsbshj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2rvvrogoo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2lgbbjiok.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2lpfraeul.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2jyyptrma.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2pexhcpzc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2pbdsclcb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2bllwzlbs.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2fhcczhly.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2efwqykwe.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ufrunznz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2tfcuekdu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2mehmpgnx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2jbuouzok.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2dppdmkbm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zqsnzehh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2epeqitvo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2elkttxzh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2eiqeljcn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2twrcoiek.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2lpstgrxi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2arikkiqe.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2pdzfywjh.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2cmpjbkod.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xcknzqwz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qzipvlle.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2fwgegvum.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2iwdhjncy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2aptoffiq.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2owhihnip.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2vuhrhfkf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2qyqmirxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zvkedrxw.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2kppvqgrz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bplpqamn.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2jkkcyydb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2hcatekez.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2bxlykzqm.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2reoozzsf.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2cgycedio.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2lgtmwpec.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wfyljobm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2ogpusioj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2gxbohwai.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qcejxsma.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2eqjveuxd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2mzpdwyhl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2yapvirns.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ulhjjkjd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2lhitprzw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ffdyfvwf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2xhqafbpa.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2bscmfjkc.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2rntzczet.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2aeudqqeq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bcnhmtgq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2bokothwg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2uxibpwis.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2qnerwtdt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2pbapgkcj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2zxrfisng.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2hnlkbjpo.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2kbnmhmky.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2wahzmxnl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2bvswfakm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2cxnmuzaz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2jxzqykav.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2xktuukjl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2szxspxzh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2schixday.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2lgqdfqne.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2iykiceaz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2dntgsrqy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2fbexdplu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2gvthssqn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2tgbpzutw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2kiwuosyq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2zxkhbloe.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2cfbuqpsg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2anjzretq.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2irmzvsbo.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2twstzivq.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2kwxuwlsk.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ymlleeks.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zsaoxqvm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2admwivlj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2tuevsayk.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2pzbiottv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2uhxtewkc.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2phsgzisp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2jhdeajqm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2fhspyjek.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2zdkcyszy.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2zwrzbblp.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2nulaiovh.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2miqfpyuh.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2xmzhzhwd.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2konhujnc.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2unvgiczd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2ommrkmyx.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2khcisovi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2yrzpaxfi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fzbryojz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ncbclggf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2rfbrlojq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2sputjjef.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jcltqiii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rzvwajae.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2cowrdvvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2opxkppsw.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2eqjowokp.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2rjwnmqfm.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2pdjyjjer.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pglfdooz.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ltikgamc.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2yqkhpjlh.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ivfgkvgj.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2cgmraezn.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2jthfvwgw.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2prwgcfez.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ubgeczcy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2anncbgcc.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2dflxoans.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2qmkrfmga.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tchadipt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yhhlgitq.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2rzcyzukf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hqmsctsz.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2rtqkwicp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2napdrtvy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ueveppds.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2cbzypafq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fdrkupqd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2fdqjwfme.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2wkkkbpnn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2jtynmjzn.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2jgctxpeo.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2fudklvgm.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2nweduxfi.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2vohunzkk.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gphybxua.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2nnxpelfb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2eughrpev.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2njiqsouf.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ryqyfrzj.html


<!-- 参考信息 -->