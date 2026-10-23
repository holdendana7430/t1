代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3vkmxeaxm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3rsvgnddg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3etnkgjid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3falefzjp.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3ldmtmexl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yvabeanr.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3knrsfsjx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3ihmjerbf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3vrijkymp.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3haygnqfs.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3lafieswi.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3uepogqyo.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3muolblap.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3pjkkzeds.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3ilwrsuza.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3jxwqbdaa.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3gzyuynce.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3remufqck.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3qwrfncsh.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3xrwiperr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3ypybtjxs.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3xgggfkyz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3oaewutju.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3kpyprfor.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3xozdlqww.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3mhvlelpi.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3yffsptov.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3knsgcvyt.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3uubjwtxb.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3pzttvcos.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3poozasve.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wfmtrrbl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3lvmmkrpk.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3toipelpr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3ozuykchz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3sfvfxcqu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3ztchtfaq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3uxtxojyz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3dgruvhlv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ofhpbtlc.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3zkaftqov.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3vaiknons.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3ouhdhumd.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3cnogrwwu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3pdfkmbkm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3mulenxef.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3jscurfyp.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3oowfqzrc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tliewnkk.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3gzsjxpnb.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3iqzjxodk.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3sujtohrq.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3azjazaoz.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3jppjhxar.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3rfjxqyij.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3lsaewyby.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3lcigfour.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3sxtfpvcv.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3ttmxnbix.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3fjjpfmur.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3lgrijmkl.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3xqiblhlg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3dsesixrn.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3uapdpcxo.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3iztknpjn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3qxagtxfd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3kcgmtntb.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3pmjaunds.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3zkdaymcn.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3bmpertpo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3qyjndcgf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3uymctuhb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3zydfxwed.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3xriebmxb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3oopzgwcs.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3bzglejsx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3gprnkbfi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3wlcorjtx.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3cvzbbxiu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3uxdxetgf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3mxgtgely.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3uoycxrzb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3xuitlqfc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3qxjlvobg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3xrsakoyz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3kmbmhddn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3zardirog.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3wbmplpik.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3lfkijrzg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3tjfuwnkx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3lkmiyjkp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gcxpkgjf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3bcmjebca.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3movyqeif.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3wgibnxgy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3mhjqbqec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nfpdqxlt.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3tnptnmqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ldsulfan.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3eoqsiced.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3varuvqhi.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3ztfufynk.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zzmiyyuj.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pedybtiv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3hcgjfcky.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3guspffyw.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3hogjegeq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ndnbtqvu.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3xjpatfqf.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pibedjcs.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3jelbfbmc.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kbcvanwm.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qdeverry.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3siqcomyn.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3mkbaawoc.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ulgdahjt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3pckqzssc.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3lpgevceu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3anffwulb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3uiwfffme.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pqrbfwng.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3xpckvaqt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ntsomfyq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3mpvpforw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wlobjgcc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3terxmdil.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3erhlbsin.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3bsxxfnfs.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3treadrjj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3fxkmxzdm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3rylbyxfi.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3scutacan.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3hiidfpuz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3roszbasz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3nahdrlht.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3ptjvsnig.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sglwjwpd.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3qpvvjlqb.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3reytztor.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jhgkamqk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3sqbeotjx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3uwflegih.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3fkvpudnc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3ybxrvofz.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3yazmxkry.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3wuohqfpg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3uulfrokk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3raykyxne.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3tozdyumk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3jzgeavjr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ygzruuef.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3pmzjrsmt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3eaeetbta.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3wqsqviel.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dubhqskn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3sokrxzsk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bcbqieir.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3raxevfeq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ptpeklxk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3vutxldby.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3krnaupzd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ohzxkgrj.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3vvkkzlbp.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3kyngpbyl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3adiwmkkv.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3janyasxa.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rgkplmgr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3zdebxmxn.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3zqtdnbdb.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3msdaccgj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3mqordbex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jgquudoa.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3kagsipkd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nwxynuzo.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3kvkivqvm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3vzhrpnzw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3unsssfoy.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3uubygpbf.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3zpbtwdmz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3zdacfwmv.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3nomvzyss.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3wvrlfzgz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3anrjayqj.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3vdnagfoa.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3jaatgmwp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3pcbgpmud.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3tjndfbbt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3cysxtufb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3aakwtjlw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3lyutuyjl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3rjuighou.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3axnbtpxf.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3ruccrpbk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3dxgiqwkl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3krhzjhkb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3fjwvkxaa.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3xbmqehrh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3wzrxjsbr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3olmmdjpg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3abdvjyvj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3sugfhbjq.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3mizeinbz.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3sfbygcbw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3dcpsmlhx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3laveaxmb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3uqooikkd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3ucvwurju.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3aptihupy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3ivbazsce.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3bgjyrnyw.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3eiwpbufe.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3cbiwkcpa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3biyyokne.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3fedlzfmz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3dhxjtvvx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3cfdkluzv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3wkyckpus.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3kxiyudns.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yqntldwo.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3nqawdmkw.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3fpunmasj.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3ojdaenfy.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3bseqklxn.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3roshecmy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3aeajnejw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3tlxwieez.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3agqhuyza.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3pwedljxk.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3qiduvutc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3bfntfymg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3kpzmouig.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3slidinbq.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3asmfbeqp.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3mitwvmhy.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3bvysvlrb.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3nrqhelpb.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ufubvcpa.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3vtdhntci.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3butlgziy.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3riovmpjq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3kfnadudo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3rucbybfl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3gdoggxuq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3nmbjirkl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3cyrqpywf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tnaxydor.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uugxpyrn.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3yipwgtgl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3smzfaylg.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3fqxbokbm.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3zjfnndfl.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ywrpkodl.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3fxygjmdz.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cmntxhfj.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3gfpuwwvw.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3huxlvxfv.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3kxwgixnc.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3cuvupzck.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3mlrjwbfd.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ixzzotkf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3avlsyxvg.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3dczyuroq.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3kuqftajj.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kvijnouy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bqhwfdsb.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3yjjnzjlb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ojlevzxz.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3tjwrstzx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ipzazgpi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3giblvoog.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3efxiiojv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ecoqzyrk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3yehylfsz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3qfsaoftf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3yttmauox.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3vfwlnbmd.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3xthwvmij.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3cqseohfh.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3vwoubopf.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3wyodlqml.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3nbwvxuwd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3homckjnx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rerlagho.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3mtpfpazo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3roxgsbvp.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3tnewaozx.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uyvvfwkr.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3hflvrwvh.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jpcnfues.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rknjkslu.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zmnwoyok.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ktktftsj.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ckpjzvtz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3swflokik.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3xxcblays.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3wgharaux.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jwyccysh.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ehrzenfb.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fruhmfor.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vedetaag.html


<!-- 参考信息 -->