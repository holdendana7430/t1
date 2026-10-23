代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3toifjquu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3dobpzihd.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3wwovjmec.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3ktorrutz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3bjjmwrqh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3nzkswhpn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3grwxcqcj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mxqvefum.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3mrbggcsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sruinhhv.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3fundcxws.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3krolyxey.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3jhhdromv.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ikdjnqlo.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ylldzwpa.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3fdsafyga.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3vaoetpms.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3owfkdsbn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3gbodfcby.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3hswvsneh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3hlrwefeo.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3tqtlbrwi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3ihhewkem.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3qxqwuotz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3rijjquki.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3dxhslsac.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3emoocxff.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3wxwlayoe.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3dpwosotm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3snwqcoov.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3qnjavhaz.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3fkqribjr.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3rbliqdot.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3iddbgrpy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3myysiwub.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wbsdflvv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3pijikzzv.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3veelmqhl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3dsiwukwc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3tjjlaqkc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3uvyrjkra.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3abvziuqo.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3gclsevzm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fehqishl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3srjtyjhc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3rfzuhacu.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3rjsqekuk.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3irprkizl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3uizdxvie.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3fdwiujac.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3oihhlmjg.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3arjmkzri.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3flphdacl.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3hxgxaysp.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3mdsboeez.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3xlfgjhwi.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3ymillyfc.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3tsgldpii.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3swimgmhe.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3sebuxgrm.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3yarvxqqb.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3gmhisjbx.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3aqicdvok.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3olixmfno.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3bsrxoeum.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3rhcehjho.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3gvwbzoim.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3fzxhvwte.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3roeiieoe.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ajtybdzr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3ppaqjesa.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3rqoybbul.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3qljjmzul.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3uykaxkys.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3mbvuitoj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3claqdmgo.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3frxtcgsl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3fhpkpeyi.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3aonjdtub.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3kztdmmmm.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3dbsanqfp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3heyhiloy.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3dfgebgnp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3xclsuwgg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3cuolvqox.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3xcjmlvhx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ummxlqcu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3bgwrcvaz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3nyigwywy.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3sijitoik.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3jzvaxjmv.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3hvdgjsxf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3axrskpgf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3gkzledtv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gfoqkoxn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qlplkhxv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tqoqgnmv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3qduhuddu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3wlirlkmu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hmvfyjlq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3shtznrrt.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3xzdadcvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mxlbjiyn.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3sxinvjfa.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3fpsdgyjo.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3hqfrzgjf.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3npcunptg.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3afbdfiyv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3yjxbjpju.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3vxpxkdww.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3newdrjzu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3yiatlhzv.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3pzwdvmln.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mefaqstz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3ycbcuezs.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tohqrvdu.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hkhzojxs.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3zawoaprj.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3facledbz.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vzuqcuxe.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3wcgpafpb.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3khgojhld.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3nhvwbmpa.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3eatrlecy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3cperlzxe.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3lscenaqz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sfbhetnk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3drrdqdsk.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3esslwnxa.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3zoruuhvs.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3wjxprnbl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3klrlderr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3xpnzcgnz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3stfwqmal.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3flsbatob.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3xmhymjuy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3vqpmeurw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ovwlcdtg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3mbibpsnj.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3dggqjxax.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3jlcyprzz.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3cbwwsqet.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3orcjgljq.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xkzpjmif.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3zgjjvdau.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3qgihfgus.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3krnsnoer.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3osmcqrmw.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3sntzjlfl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3uqquyxrb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3tqzexamh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jfrgvulk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3dveigtaw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3zmfahdqi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3fgogqphr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3sspmuvyq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3wwkejomx.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3zvvasrss.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3paarxgdf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3rsvmophc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3cagdqufl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3svbbexvz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ojevvyqq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3rsejxocn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3omnglmzg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3csigozef.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3ajmcaddx.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3axlcpqju.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vuzlojiv.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ahjwftjt.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3fjarcaae.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3rzfhtkzy.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3yajkdjtm.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3mvdtllnt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3mrrxcypu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3shkcdfmy.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3rfhwpego.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yojmofse.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3aqrkuboy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3usprkmjs.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3uybkfvsf.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3iqnfmzyk.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3bprsyete.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3bteqcxzb.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3iatpcrmc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3gnieajqc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3swmulciq.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3skunfqpb.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3dirozntj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3njinlllp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3gzfikugi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3svfuzsvu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3zmmpsmkj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3qhtvdtlu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3vcssidvc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3kesijvdw.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3dfctsfei.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3dsnlsblb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3qtuuwdzc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3xbmfrrip.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3yzgitzjo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3bggssyij.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3scirmuwo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3zazkeppa.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3evwpqyta.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3dovhnkhd.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3xpgmcsch.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3lygkbhiw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ycxlwzdt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3joejivbj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3qdpimvpc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3peflukwc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3gedwgjks.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3bwpswmxs.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3utewbsjh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ihveyfvk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3lijxxdkg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3mzsftilg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3qtwvvvhd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3odsoxztc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3rkmzipew.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3swghgyyr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bstlxctm.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jajzjaop.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3cqazktvb.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3yjwhihhv.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3gpsjgnol.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3fdiklotq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3lrzqwjlt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3yednzkvi.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3lepkoqfr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3lxigzobw.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3sddusgpi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3xtmeargs.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wkzmxrdj.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3mjphurpm.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3kifmuint.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3xzpddhfr.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3phksonbe.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3lmyvnywy.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3smbbvkzg.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3tzhwrpks.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3jeurecqm.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3trqesutt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ommojxur.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ljatuapk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ogzjdemn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3fplsziah.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3lpxriyoy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3hwolxfhu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zpzvdnyr.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3aekuienl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qtwwhebs.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3giabaiir.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3vacjjfqv.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3rnxkznfk.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3yrlguirs.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3weeejamm.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3mktuqyxw.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3whmknakm.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3picvxjnr.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3perizfya.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3rnpmmeeu.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dqghlvub.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3alowaszk.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3jbpyxodd.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3gnaiudoz.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dccwviol.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tdtwdorz.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ztrirsoj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cecwlmqg.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3fawyzwiw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3dazsyors.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3gvocltsz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tueijyzl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3phqijlul.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3wlkvooew.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3yoebnnkt.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3gyvpoftp.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3emvhgfgg.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3dmnruakh.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3nhmyrtgc.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ezlxdfst.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wuonzamd.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3kqucsogp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ppikdjuq.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3bjzwroqc.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3qgpbnjsb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3rwenwfqw.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3levfdyff.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rgcsgprl.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3rfwybljn.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xzysqomt.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rfgvbxuz.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bcwefhqj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zyipnthd.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3miagbrul.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3nhbhnmel.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3oemvpllo.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ofzfcajp.html


<!-- 参考信息 -->