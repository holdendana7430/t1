代发 wailian999

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3tuhzirxw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3hhrmenti.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3xphfqstf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3ilryeluc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3blnmfmgw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3vgekdqzb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3bbwwhtoi.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3xhvtzxas.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3xovthmqt.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3nupjjwee.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3hpaqyhne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iktvrcti.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3iwxdzqaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tdeijxar.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3zmydcmtd.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3ernvjprj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3vcxxdhjb.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3apoyiaqn.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3xmctfmnv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3eccwfmod.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3yeneifyq.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3uvvesvfh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3zxxucmpt.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3hcabwdjw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3ljsawkkz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3vjvmwjcr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3ehtfwhis.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3lthkszhm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3zvcefjtt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3leykqxck.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3onbnoupi.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3jzlfaiai.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3tsfhflxz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3gswypbae.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3zetfmsvq.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3pdokhlnc.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3aafculxt.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3hcasbcnc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3xvxykfly.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3sgtpayiy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3qgtqqngq.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3wkleukdl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3saadeths.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3xkuaysoi.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3enzijxoj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3mybcglhd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3pfuyuepb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bkwydvfc.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3vacoayvd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3hoezrnhl.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3ppbwhage.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3fppzxddx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3jzyvclpj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3bznfymya.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3xmzduhro.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3fswhhvzo.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3steasbyh.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3wcfxbutk.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3jhemggcy.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3ewuyhcjd.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3fjhzquld.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3ewxlylmb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3dudjrbat.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3zutyrrva.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3bcyaabfx.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3fspmuinw.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3xciomzdd.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3fsahbimr.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3vtrtuwzw.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3wkwryblw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3ixpfjmkm.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3kvjajfic.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3aeezwlia.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3zbwdkuxn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3knuicvad.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3gldoyxmr.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3vyqhamsc.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3iuujiikg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3wsubrhjk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3xfxsvpbn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3sirohjrx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3oigeilyu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3rtylbpby.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3arajqvdo.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3ywdfwnuu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3zxeqgxoz.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3gpofjisw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3tcpsgbop.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3wedzdgsd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3xxpuaxeo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3cuabnpdn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3dwsxrmbm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3ncprespw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3rrlikrma.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3tygvfvbh.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3zqxfofql.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3pmtdzeis.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3sanuefpb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dvfxabsa.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ktasulcu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gfdbblsc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3blsxdbqz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3xcicswkl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xgdayjcd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zqlfdcae.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3rjvihvdt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bcrbsehe.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3cwuqfqkf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3kijeoura.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3jqnvluwq.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wvysgcmo.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3sdbljoam.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3ygxuydoa.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3xhgeyxsm.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3fkropbfm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3nahwzhmg.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3vplzgitj.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ilbmwkbu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3godjoqoi.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3gpyymwaq.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3rqmvubvj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ipaninxu.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3mccffnua.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kqmlxbgl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3htkdpnbl.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3oxbfdgww.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3heputxcf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3bngtmxyh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3cvwtswce.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hugqeexj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xedwhkpu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3egmjjmon.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3nalbppog.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3udfvfzam.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3bhtpgmdn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3knvkqwbn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3ugyaplct.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3hzirgfxk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3uxmfvsld.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3lemfjdkt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3cptrvfxu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3avukrvnv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ksffpbrv.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3iflbvvzp.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3qesmbseh.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3tcynfmbq.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gdddjomp.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3abhmucpy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3kqbaxeqo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3lwzfqyvu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3lkaqjitd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3zufkqgrp.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3bwttkpzc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3azwsrpre.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3mhwuztwa.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3bdejviwc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3fndeokxz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3wkwzdyiw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3nvadadqe.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3jqznktff.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3aelysitv.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3hdsuxqzt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ycgmogbu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3lldkigdx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jajtadde.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3csgccurm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qxgymofn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3vphssziy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3qulsdjxa.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3crfqjvmk.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3jbjvjshb.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3ksvnvnhw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3rsaxjwok.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3puvvjzpc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3cmoxfdwx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3duulnoal.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3fgkdufhj.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wvhebtui.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3bsmjudaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bvvbhrxx.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3pzcyqmzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mlxscsqg.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3iytpixjh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3avyrandr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3kzbfnhqj.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3lyqbewzr.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3dsluunyv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3qdntpwwm.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3jhttddnv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3zypcnyhq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3tetyqooi.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3hyjwclza.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3dkffovkn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3zpjxmqdl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3tjgmrgrx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ppzfmchi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3dtaqvmij.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3nfxldlea.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3xryftfph.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3zvhprpcy.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3tmyhmdng.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3eznjaoyi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nivuijvg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3rxevmyaj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3tkofzeyi.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3zvddxswy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3pcqaisfn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3ptulplzv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3fdpsybcp.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3tyijlcla.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3emerrcoy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3eoxrcjrf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ruolsvig.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ogvmjaen.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ewqtfmga.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3tljuvoos.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3hrdnflhk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3ufdootvh.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3ifycjmni.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3wnpriogh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3ylqzlkpj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3pvherutc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3uznavpyq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3kuhsnsdo.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3xunqprxz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3aykglzau.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wpdurojq.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qyswdpsv.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wgcnnaqc.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qphrgwya.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3kohcmwtk.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wskqqtnn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3rsgopebs.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3hmuhwhux.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3sqwimjwf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3yyzomdvx.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hxxsrafs.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3uujbypzn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3aopnqncx.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3pbvfyjhb.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3wxbkaajb.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3nprwvuwb.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3efbmrvdv.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3gixjdzba.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ynmjnntc.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3tjyzwsbl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3wckhempf.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3laoqtque.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zdmablek.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ceawbjir.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3ehmlvtki.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3jimfxjve.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3nuwjcwrg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3szpjahlv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3owcrdkwn.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3hpxpsjud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ethaazjj.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3rabgruyh.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bugzdyds.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3rambiueo.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3gpjneypt.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3hkngkcgr.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3zllnpinu.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ysmqhrks.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ellyjgzl.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ffwowoso.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3nypyuced.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hednseho.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3fozuofvj.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3xlgppmmz.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3cmvbpwxd.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gnjdblag.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mowitcmm.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3kldcwwjq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zvtshqfi.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3kwsfflgs.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sskadbza.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3lvbakhds.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3hhsjjwys.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3zutlvlrr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3mxwkimhm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3elwqegmr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3jokroovi.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3qcysdbmb.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3rvpxzawo.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3vtbkdqsy.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3zrdwomdk.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wtduktka.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3azmajxvp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3pmbllxpj.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qoeucypn.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3jmqsimnf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3sjssycei.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3sgkvhset.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iluyifqm.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ydlwgsno.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tadjukrn.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3udcmqngt.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tkfwptsf.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aefzcznt.html


<!-- 参考信息 -->