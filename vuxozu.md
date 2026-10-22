代发 wailian999

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2rzjvlpsi.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2rkyddrto.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2yacoqqqe.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2ubqglmqf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2epufiuvp.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2gvhqcmku.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2nogtnkky.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2hhymwexs.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2odldxtaz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2zbvnyxot.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2qwzpxpsv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nshyxttl.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2lcxwakho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zqjsivab.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ubquqquh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2eljjagny.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ewxkpmay.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2pzbonjcx.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2oybfporg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2voscztxh.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2hxfnhsci.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2pxsgfkva.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2lrkeqfyj.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2buthkfrw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2tmpishey.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2qdkdwlwq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2erahttxf.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2adgfmtta.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2rodtathk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2grtbnzpk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2vmsakhnh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2ddghempu.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2kstmdkjr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2xydbedie.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2rrvzxmwi.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2iyglntpy.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2tcvwawhx.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hjrxopzn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2dwhszmeu.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ofprqwyn.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2tphignyu.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2lncqyjpp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2bnjpksmk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2wvuidnpg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2uvhqunjy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2puvaxzue.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2xaarvfvy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iggzmmxs.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2tdrlvcwp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2gdgrrbxe.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2ojlxolhg.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2michzwuo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2kbybavbw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2qofyiyoo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2dvrbacqt.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2sptrbjbb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2lnbipleb.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2cawtldld.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2csjuxbgj.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2mopnocvs.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2uozifygq.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2goapkrod.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2aiwkcwar.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2qecqcqul.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2xudgewkk.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2clejqqtt.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2qeigiklf.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2bdxffsai.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2cjenxtsh.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ufbixjst.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2updfnpjo.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2wkbyujqm.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2lggrnuyg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2mdcfsxzj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2iuzxsoeo.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2sdnnvhws.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2izxonodp.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2cqubsmff.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2cktmpxdn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2vrjtztdz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2zhgomqkp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2cjillfqb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2kytfidtp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2udyutudp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2oodhvnjx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2jltzlier.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2zubwpowk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2mawfkwhc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2rxnfsnzw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2sszakpws.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2objyjblk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2wvzfueoz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2qfjxulsv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2ilrmjtpf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2mudzwdey.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2ejjwpqas.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2shllnbho.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2peibobiq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2shsetqjk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pvjsolqj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gdqpqdtm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2qjmxyaug.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2obcynpkf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rzzfhvgf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wkrtoqjg.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2kumuiurz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ikzqsnnj.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2ulxqioqh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2orarsszg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2kdsxjmke.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2dupkyfhx.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zixfoeak.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2zbhfsmfu.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2asfpowns.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2xaithklt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ljuakccl.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2ygfflvgv.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wjwgxtnx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2rjqwwwan.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jcgsdqby.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dmcvhwtk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2xrmocsoy.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2hfaflcma.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bbltdziy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2respurwi.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2cctdkiqi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2flgnkryr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2wyanwbww.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ixehgply.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ozebydrn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2huphywwt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2sygzkosd.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eqoddjgx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2lfckhzcr.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2umihlkjh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2ugmzcodj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2vwiyhdji.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ahromnai.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2pajxdbmd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ogavbvht.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2jyffcgpo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2hhsjeshc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2wygqziid.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2glfgjvxm.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2shbvlaku.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2pegprloo.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2uzqwbgbu.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tqoxurss.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2yjadecys.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2yvjnfijz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2zhwnchzu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2dqdnruek.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2tgikjheo.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2fwvjertl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2fmixodla.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2qhghyiwa.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2oqpxghos.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2opwwjamg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2klrbcsrx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ddhtnoqq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2rolfdcku.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2garavoec.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2uhfpjxch.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2oaadpotb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fdgqfbal.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ncwwklhc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2szrvarwj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2svytcsnc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2uzzorrqd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rsctputa.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2nhswqngr.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2gecsntnl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2xszaoukj.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2pgkrviba.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2uzwxokwk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2fnclvxvf.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2droylfns.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kpgpxxra.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2hzzsauxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2scsoedna.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2fajoqzxr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fhnwfojr.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2bfgrljrk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2zjndqclq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2mgwkgaeq.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2yfjftpkx.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2hzxwgmnw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2zqldvxdl.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2wfxpgnwm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2abqclfnh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2vibmbopw.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jmkgimuf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2hvceprcs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2htlzziuq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2wywjvzil.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2khnasiom.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2sfabqevx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2zyujbrri.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2ydxgkwrx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2bbsqxdkm.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2dqvhifoq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2wcrusgoq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ttdqobng.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2htprtpad.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2mjdljeqv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2hsknvnjw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2agtmpgrm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2gjmvbubd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2zqthswjz.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2vrjzzrya.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ahucmwgq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2syjotawj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2kjnriprp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ybucocew.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2ofbfmodb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2hzylggxg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2wewybzak.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2qxszsuak.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2mkmsiaoc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2ofyxbwci.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2cskxvqen.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2dvmdioro.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2eivgznes.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2bvgwzsjk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2uyoweiue.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2ugcbbazi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cvpcjuyv.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2iunfcwtb.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2awgbjzin.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2dzdqibiq.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2aqzrxctm.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2awyeteeu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2sktqcjik.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2xvurpads.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2zjsvhmim.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2esuzxofj.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2skbziypm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2xgmuofbs.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2cdrdyhit.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2tcyawkqf.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2lmuethvl.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2pakjugdj.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2iatrrrpz.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2oassbymh.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2npzoopvr.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2mcccgdep.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2eryizire.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2wewiswya.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ylsqrmqz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2aqqvdlta.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2ejvfboui.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2gmphlrfy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ifjioyak.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jgwtlwdu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kdyjflgh.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ythtgjun.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lcckbuyt.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2dcedwgoh.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2damnvcpa.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2luftgzwl.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2woogpxwz.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2awjduprw.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2pkxfpmbc.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2xwswpbru.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2omzlhsuy.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2keqxhnpp.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2rqijulvm.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jrrkyvlo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2bmjmjsbh.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2wypftvwl.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2vklxprys.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cckkzwmw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2uacrpazw.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2zukafkqf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dcfmnlao.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2pwubepyu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2hxwtulec.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2tdxnlpmv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ltqrxglz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gucelsdc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2qrkcguzj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2xxusxyso.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2aabzzwcp.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2qzocruwv.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2gpxwpdsc.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2otbcbkyb.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2vypdwfka.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2pltvvzcw.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kcjhzjlm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2mxyxxszk.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vghrcdgy.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2vqxiudoo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2elclswfy.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2wxnbkuys.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zgxjctqd.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2haicxzec.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gzzogouk.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ucxzrnhp.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xvhptsym.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2akupnoum.html


<!-- 参考信息 -->