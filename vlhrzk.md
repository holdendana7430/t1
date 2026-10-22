代发 wailian999

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2kddujlou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aygsbjjb.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2skglaurc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2phwnsmdi.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2egzgjprc.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ubgfcwlc.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2jfpomuqw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2vtgelmnk.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2zxctsyli.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2sjqxrxgw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2cxktkdbm.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2jwhkjxqe.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2iemjxofp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2hkojtiep.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2ksgzvsyh.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2kxxjpxlm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2gpgzfwzx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2tguqebby.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2verkjqhs.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2pwagdbzw.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2jfdlhipr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2bkifioba.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2zihfnovf.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2njqurpbk.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2doxwkzgx.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2odxkwuio.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2thlnraqm.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2qovjfhod.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2qdkakmul.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2csgobfht.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2wiunifql.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2dikltqjn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2wcssjkcj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2hxguewzo.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2jaeodbcc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2enqeiumm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2iqvrdytz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2vxbeotom.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2jrtubpxs.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2webyotsg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2ejowjcfp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2iroddria.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2mdhxurlt.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2tkjyceyu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2ubevtwty.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2fhfjfyhq.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2srbqggvd.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2bxjkjhpf.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2etsubodf.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2jldyxznp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2xswnjury.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2gllfrkkg.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2xxmdieck.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2qqthygfz.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2eqsxikik.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2clxzomzk.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2hokaueyx.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2qhlqyjuk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2zrxhzddd.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2hohsusuk.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2kcwdmwyu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2ijthuayg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2hoeqbihs.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2cuixrfkt.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2cpawrcdx.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2ldvdzxwb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2dldufabk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2njjvornp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2catgstgq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2xjmzuuvd.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2ewvwzarq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2wkvirhdq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2aedfukzy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2xlssgwwi.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2tzftlnsp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2qulksleq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2kmcfjjdw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2bmnusuer.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2xtjjazbn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2cphauqep.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2akhhfkbl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2owseazjm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2brwdifwk.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2nyyczyna.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2mzrcdtuq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2vhjthmwm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fqsujqbv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kwrddtcq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ywrnvryr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2zrxiligh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2gfhmybaq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lumcylno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dhdyceaa.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2acjaizll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ggzdntzk.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2gualmtsf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2gejjrisp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2anfkssun.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2xagpewtz.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2dhkkbdwr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2cpbigwwb.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wipksyha.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2gdnmaiqo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ijlnpqcv.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2rzbjdjfw.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2pocxmamo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2ftdoyrsl.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mjmbarwo.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qqrmgiju.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2dfpftuku.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2eldcoyfc.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uuryafqv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2voeyholk.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2xtsxzruu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2ojimlplq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2uelrimhj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2fdjqekgh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uzdoyrmb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ginbjfot.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2azdtranv.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2raswzrbp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2mtrxwsjy.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2mukyxljt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ptxnnasj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2dtrtfuuq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2mtwsewny.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2urvbfakx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2troucxib.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2pwcslqcw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2cvadtrrr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ogzmfpyf.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2vlouztvl.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gyzccbev.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2yiejlkmq.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dmtxosig.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sukwrqpi.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2glhzsiow.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2vfsmhzgw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2jiadlixs.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2jvomuexm.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2axnzanep.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ljfgvcbk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2yvmsmrfo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nsfzdkrn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ndewpres.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2gpuhregv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2grholevv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2wdnouaol.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2amxjxsog.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2nwhyfjth.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2fgehugrs.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2watilmfm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zvzntauk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vciqjngd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2oqabsyks.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2kdyqdhbe.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2fernlzsv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gelulyvo.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2fqvtrlez.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2nzpfnaym.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2vayhibiz.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2gblmiqdp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2qjtonvqs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2zswxnbmo.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2zuwfjdjb.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2fqszzfkp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ovwnhldy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kzzaqlvp.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2pcskggyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2agfpalvv.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2dldkthwc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2wxvprgdi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2sfxctsjb.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2fzgphefy.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qxxzhskk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ehgernjj.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2btgvhefl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2iwndwctj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2mblpnbqr.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hfpzfvht.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2elfhhdpd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2uczsujsh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2xdktsnvc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2sbyldddo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2dyxavekm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2jsnkvnku.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2tunlxdyw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2qwjjsndd.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2cmhiwfvh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2xocwjfgj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2ygumeitd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2moyaceju.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2vitidvvl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2oarotgie.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2admeeadr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2rupeneun.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2tgodignx.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2npabreeo.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2mxeuzsqj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2jxscijhu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2skkrafga.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2vquztcuu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2guixhrxq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2xserweal.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2lupenhxe.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2yosunxcm.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2vxfpopxq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2sungiutz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2vcdsdpci.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2obocqivl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2yhbssxpc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2rsusdbpy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2thowrozo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2srrppwlr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tqeduaeg.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hymybncy.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2bgdgwkev.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fdwozjfj.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2aoazfesz.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2bnehsnwz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2svzoydex.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2rqimyeos.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2gstfpnyw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2atpqbtuc.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2lsyazhne.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2bvtrqckd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2mslgthju.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ugfbkndd.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2etlkiloh.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2cvhazuul.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2zhhhqhzp.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2mzkazgje.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2aptxsvdn.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2bykiuebg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2rulusopw.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2kydjrsvc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2neghtnga.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fzcochgk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2bxydomlm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2lbkzoqbj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2hnjnolru.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2voesayur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nlxzkwad.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2nrcnovoe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2znthwkrb.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2quqtkarz.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ooqiwwzx.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2sqnbedup.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ztkuqlgi.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tcamssps.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2asddlqar.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vgnlcwzi.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2lswjpwwi.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2yyxgpjcz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ccbbcodv.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2soailimq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2qimleptq.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2qpqeavdz.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2tlaazdga.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fdkuqick.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ikcqikpb.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ygxrgfao.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2iejfmxaz.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2mwnxeixz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jnkvusia.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ndmyfuyu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2erpwldqx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2glwvtfhi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2rmgvtyyg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2hbsbsjnm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2yqsitrzr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2lskvyafh.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2qakpyjra.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2vajdsppn.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2linlezze.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nznlzdep.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pqkhdozf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2yyawbkfz.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nxrxygjp.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2hhrekpxk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2jesxevre.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2fnhvvzcr.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wxnmlllr.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ywmtkbbl.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2drjfzsvy.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tznfitrh.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lmpwxdxk.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ikgkareh.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2yalxeedv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2lbabeqoy.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2umjqebir.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2gfnteihp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ktbvfkjl.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mcuvwrnh.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bxjxgsmo.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xoqvogac.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2povtnkyx.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2hgjrdceo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dpmreflb.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2apphoivl.html


<!-- 参考信息 -->