代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2yftstwtv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2rkevdyvy.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2vcrildri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2flrnawyq.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2gbpdqibp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2msiaomok.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2dgoerstx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2hkeyrtah.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2zxeisdeq.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2enzlyaaq.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2rkrmzypk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2owagcibs.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2oqyjgtnj.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2dakavgib.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2idvxlads.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2whdkmdzn.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2cwobtort.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2arhuekdv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2ufsdkiju.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2fxeawswh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2wlivocea.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2hqcwccdx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2gebonmri.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2ghatkcrm.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2bdnioizt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2eiswmddr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2qucdfwvc.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ikismpxk.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vuiknwrf.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2bavzyueb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2mbpvimtg.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2xyrvsdtm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2lkrsypyf.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2vjalheke.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2bbpcwbsr.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2garahgzg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2jysgztjc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2bgozggbt.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2bwcbjpjx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ckaajwgn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2pjgpcqnp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2wfisbdop.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2wdyunngp.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2ydjzghxn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2ooojdqxq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2vivyutzn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2jeqieolw.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2pntjjlor.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2goocgzom.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2vmceycwf.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2hqfmmkev.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2eauefpjh.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2aixwoklf.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2aqfeswbc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2bmowgnqy.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2fwrgzoov.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2jreootez.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2pugruope.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2fzvggmrj.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2vtafxkhz.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2pduttwjk.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2posmutrx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2ekctkroq.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2ronzmmxu.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2dzxrihuy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2nzuhenir.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2axffmqcg.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2stjlwbkc.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2spgwchav.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2ahtpgwvt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2amzrkcov.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2okpclldi.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2iafikroy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2jtrlxnoi.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2injhdrhi.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2buvnfiwo.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2omqtubor.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2odsxjelg.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2itmzeerd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2rwkdawvv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2isfoialk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2jbzzbfqh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2nhujjiyd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2vtyrbfei.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2vnzsukiq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2iholtwdb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2vcsyzjpj.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2vlnaepex.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2jgbmhpip.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2jidlxdof.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2nqpdhuft.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jjoeiluu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xgnxntfr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2xciehzmq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2fvgzrykf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yjgnktsa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fvmpqozm.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2uuswreaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2awukwdpg.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kcgkfpip.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2sendcdnm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2maecltuv.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2eydhoshb.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ibaxdreu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2rotfzsgz.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2pkyttbwt.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2zbkokdpn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2zdqqarrc.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2soaicach.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2taxeqmza.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2gvceimvl.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2zhoomcgk.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2xilxekqc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2bnaqhpix.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2wbxlocuo.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2wyjwwecd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2nkdarkrg.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2vymmcbwf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2fvuaciez.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2mmeogjgk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2fqrmbkcv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2djqajhqv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2ebdftkgq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2pvrqgxne.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gycfzrlv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2jzsbyzyh.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2soxfomad.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2wbokdwwe.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2qrgnmrzn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2xupdkdtm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2hgvjlsyd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2adgwxhzf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2qzbobeyy.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2jrmqlsah.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2xydfycik.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2lbuwurvi.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kizqtfir.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2exnutitj.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2umijprju.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rtjciyav.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2wyhzkobi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2yxkvkaoo.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2kexsajie.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2yulyetdm.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2kuidcphy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2hmzxiurs.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2npxngsqk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2jospkxxe.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ciljqgcj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2wyujfyik.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2gsfdaqbb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ynwsiinb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2fyyghidp.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2tkurnbwv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2cijvrpbp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2uavrkeaf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lskcviwk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2adfussbd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ircjoiyi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2zsgidecf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2vcydexsx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2uhgvfxme.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2uovkwcmw.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2dstlnfgk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2dgsdlrue.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2sqfyquxt.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2bmaftvvk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2cuytpxgq.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2uzqsvifa.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fsdnfhxs.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2yxjvkutc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mzigqhiw.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2mlkqgukw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wwcmjmmx.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2hyhdgyra.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2roshfzqf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2lqyyykts.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2kpfeccbw.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wnsiyoih.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2moupcwiw.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rgcguljd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2mpsmxlgj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2kzhuhqyw.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wcsgxcww.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2vcesutgr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2wqsieabb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2cebtdwvv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ltkczvdz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2mhjvlnnq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2sqpgwauu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2tawtwsog.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2dyxjddwf.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2wcfhhvvg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2ibfzdnte.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dilbdtrn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2oimwyjbn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2upvmsjzj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2soyzkuak.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2nzoqwfxd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2hdmsixsj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2fmvyivee.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2ibxhrztd.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2fkruqmcj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2jioiuluq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2wqvorgav.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2muxqcbzt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2iwypkoul.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2kybutmfl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2xzgahtzz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2titosdzb.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2qtndpgfr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2mjsvukhq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2dddfhfve.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2kpaijqhp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2cxdgwssy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2xkjdmoyz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2jwdukpbs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2ycigqldh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lutknpck.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2cchzdrwk.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zafwrjip.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2afikmttt.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2clsxklrc.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2hmfooqkg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2douynrqm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2vgwqewfg.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2lsozuoqy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2pshusedp.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2kraawmdt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2osxxhoso.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ekiaekgz.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2qwwuzcjl.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2hkvmravx.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ebwuslbx.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2hnnlnoci.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2myjjpklo.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2snhifiai.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2vevdeqxp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2uxpidfmq.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2ypngqktm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2nwvpmqmu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2mmqbtkvw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2gpnmdzyu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2fvgggccb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ariwhjly.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2ecckaxkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iyvmidzk.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2auoevquy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2opeywhku.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ixqglkke.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2dhcldmtt.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2kiwwpsee.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2kzvyqldr.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2hcitwxqy.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ekgtiaie.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2nwkbvkju.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2yrmpocac.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2bpjndtpw.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2hqrvxyjq.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tzhjryvm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2zfqxcgic.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2rwphpdts.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2owoqqhwh.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rtrugogk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gookebqs.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2bjtyjabu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2azzrnrdj.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2debuwczd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hqdbhyzd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2hpoweedd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2yxmbjomk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2aijrzpts.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2rmqksgpu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2srlsneed.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ftmlyypk.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2nbctoawo.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2enfoimva.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2bmjuixdz.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2iebyahxd.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2divsbsqh.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2aanrorru.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2haibkfdm.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2rorkeemf.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2dpesktng.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2qfbjshtr.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2htihzrkg.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zqjnrqgm.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2syysivkq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vgiaecol.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gtypfnds.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wiodxouc.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jvkbczsc.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2oylnrgae.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2szbibcho.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2gwjyxbsm.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2nfjfoxdz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2dwfvkajm.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2amwxrmwu.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2dvtdwlho.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2vcvrlyhz.html


<!-- 参考信息 -->