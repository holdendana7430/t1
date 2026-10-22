代发 wailian999

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2qvkdmwdd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2njnwdrrq.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2eqoakmob.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2vpqjliwa.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2uxtxohrf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2vslsncjb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ttrpkkpk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ljhotohr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2xlnmxzfd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2dqxflxrq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2rcufgatj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hmgaxvkm.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2cjfoqkbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2srsbbrza.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2faewicge.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2tfahshvl.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2zfvjrhlx.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2mlmpixrc.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2ppiqiyqf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2lkaqwslw.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2vtafbfbx.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2xmlzqigh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2kgjfrjqp.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2jglnhijy.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ekhxjnmv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2efwxssnt.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2hcobkicj.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2yzwnwskc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2sgozelml.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2idtmufzm.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2qygpkaav.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2pqgzhjdr.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2toqchrln.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2goxkgfwo.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2pyjlxhfr.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2shnfahzd.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2yklwpxvx.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ezybicbn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2jzrpdjlf.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2kkiomemm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2yejaaofh.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2dqskkrvb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2nlmbhscr.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2chbxofjn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2nptldtrt.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2uxattwiq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2jbavbyjc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2ovdwdeue.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2yfqysgom.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2ajkqlhzq.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2waydblst.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2aquqfcnh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2xfkhovci.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2lbrvbkie.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2djwrgewp.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2envcrvdj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fvgtzznt.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2oeqgapjv.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ytletglm.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2wcdwsbbn.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2kotdtbxv.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2xvvdyiej.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2jrxexzps.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2zeqsccfd.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2xoeochvb.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2ycmeqkvj.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2xdkjmsah.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2nbwwkcmm.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2hcfubwsi.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2boqircgm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2adyaumym.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ydbwcbmb.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2qukiuylw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2frbutaav.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2aqdfnfxg.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ttesbkfk.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2jnysmbkt.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2ghdjqehk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2jdyeybup.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2bpnqaekv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2tksyqtlj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2tqwdbuvg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2betllkyr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2uracvlwf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2oawiqezz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2xlzxtyou.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2eettojos.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2dnoyfckq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2riykafwh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2cwsglygc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2ofirwarf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2ycunqwnq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2owssnlxd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2zqhiklmm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2mdokekae.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2atzkvnex.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2tocedlwv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2cnuszsed.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kebyrizi.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2uhjgpqsx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xxcoikkm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2altxtycb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2gwbnvyyl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ksuzqtvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zvbtxldd.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2ybxhkonc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bbyxtnsj.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2jlsdfomx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2mkowiouw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2vzxzsheh.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2jvgluuaa.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2rjwrivfd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2jxmsaaif.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xooecckq.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2qpzbschj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2xdlqzovo.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2vrvrsike.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yjvfmrsp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2fntaqauf.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fjrpnkqa.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uwrlyubf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2rwvdetig.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2cusajwms.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sykbsctu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2rleypowu.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2enqwudpd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2udwzjyis.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2bnvrkmqi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lbctzaqt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jnntnqjt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qvzjulqr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2kbsdyxzc.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cqozfadj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2qjtypzah.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2euqwxexh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2swossees.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2wkhkmtkj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2hsqackqh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2nhvkvgxu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2iasycpqa.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2nldbdwoh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2sgzdbfch.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2sgfikczc.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2ytppcxdq.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ltuufbkn.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2milvedus.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vhusesqm.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fhgznoyc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2mcvejkes.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2jczlvhuu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2gkpxakcn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2ztrznwfn.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2gfieptni.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2hcfpgdkj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2skdtuuek.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2xdiirmoq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2qzrnhxkw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2sfzpjmju.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2fagviwcu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2nwdxudse.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2fqlnnnyj.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2xjlentam.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2cmhwugul.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2qaodqvxr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2npujxktr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nkzcvwcd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lzdxbjhm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2xuxcfztt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2fascpfqg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ewsdtnjf.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2gmpynhjb.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2dxdfptsw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rabywnzq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2wyzbvupx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2dydexztb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2cwwumoin.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2egbyhiju.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qnpkynap.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2gghsvygy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ambljbmo.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2vzkttbnh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ksiziqec.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2kylbrklt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2tavxcrco.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2virgxubq.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2shwvndzk.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2fcbuuebg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2znirkobh.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bvvltpxt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2scopqogl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2wuheqmtw.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ozmpbrll.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2msctgmti.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2udsfamqz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2xpnymups.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2vvixburx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2svmillfk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2wijueonr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2aklwvvnz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2tbqvqywt.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2aspwqjbd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2qyqkcubz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2smuduyry.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ethegost.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2khlaywwb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2cwvrofud.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2smdsextp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2hfxhczjm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2wmvlpbrg.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2xzzrztiu.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ezrepyaf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2qpszjpzo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2myykmtar.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2xnejkxme.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2pwdvxkiq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2jundxcus.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2smbdwkxf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2qjwwmphi.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ugavxtks.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2qpauajzz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2cwrruxmu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2sqevkpje.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2pfyadeft.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2smguvkeo.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2tlxunmhq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2skyziqqd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qshbwtjn.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tovyfijk.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2jlxzywij.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wkinfyoj.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qevbvgyb.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2smruylqq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2szgeajhy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2tyzpjgvy.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2jkvertjj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2xktvrcbe.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mltqzmma.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2hfjohsdh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2bcepaign.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2cxynfikh.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2hsxtyjpw.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2cvvnzste.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2cwwesycx.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2ectbyplr.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2nuubzuxm.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2gfgfppki.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2plfvwpdc.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2alczpxly.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dazxfmjb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2zfpufhzf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2mczxqprv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2pjkntmjb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2auteodqi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2yfmvemns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pptqqjtz.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2frrmarid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fnewzwai.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2tygiqmfk.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vuosnlmh.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ztdvofxm.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ecyuysqm.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2swarblnd.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ovcoooiy.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wqxcwbqm.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2smxbydav.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2oyqdxxji.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xfrepavj.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nggbyrfo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2dsudbtzg.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2maqdlshs.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2rmxwyoue.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2beutkygu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cgyitrbp.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2eujbqkql.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rrscttqo.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2ldwmbhka.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2eeldwvzs.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2yuyvowox.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ppugrdfz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2uibgqqju.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2rtlejvrn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2avikkuxg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2xzayqakt.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2aaiaogqq.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2stcgrssr.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bzgxrtho.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2pnnumpnx.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vqrgrvfo.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2xiiunpeg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2qqjzjzkc.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2rusjlcgf.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2hpvvaofx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2mfpztkek.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2ahgkvqte.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bzulitir.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2nloqtoxb.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zlxibvvb.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lwodqxvj.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2teftrjxu.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zzxqgkfr.html


<!-- 参考信息 -->