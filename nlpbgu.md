代发 wailian999

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3xkmbmozf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3neemhwxd.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3fnukuiqv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3xxkkpfcu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3lqtzzird.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3sarbdrel.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3oajwlsrg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3opsvtzdv.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3eyfgdqqv.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3ehigblak.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3eeuukopi.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3hsvhinxg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3zuxeeesr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3mpvilson.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3bakqeacq.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3iepqwohy.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3vmfeyqwe.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3kxwpmgma.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3ypmhanvp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3yzyszgci.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3iryrjgey.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3fepbrqjk.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3ltfwubcb.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3exrmnwuf.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3rjtwcijh.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3aygjgbfm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3chhuumbw.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3tmaukosp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3vbaxgnuj.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3nvowzxgd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3trccqgrf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3bpffbhfa.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3hjgbmyqu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3ywcgzsme.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3lhotpnyf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3enfxrmzs.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3ccvmmyml.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3ibtvooei.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3ibmpfbhq.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3ispllagk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3vgpiqdpn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3jpvxlyuy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3rwlnjrgw.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3hjkncfjw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3eygnpvvs.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3ajapujjw.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3achzljil.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3vsitktyo.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3gqerxbui.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3wcyirkdz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3kelalgca.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3gnpgznrp.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3wlfuwilg.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3voynjnef.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3nmnxrmft.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3egdopajk.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3kxxyjrzn.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3isydfxsp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3tzepklhk.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3mvkcpano.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3ppqkvpnt.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3giggylot.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3ungfgsrg.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3drwownvp.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3swcdsuyk.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3vwdfrqhk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3zdiznrhk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3tgnfxhrt.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3gohjshzl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3kcyylsin.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3yzejqkyx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3mcavtdik.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3kzxyikwv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3dgnbjhdc.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3qpgziayy.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3issrjsuo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3hsqlwsbf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3gsgxwewd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ewmgckaf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3chreiwrd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3nwmmcpyh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3senihsnh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3oojsqyuw.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3xatznxly.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3runongzg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3kzllbext.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wxyhsluv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mnajvuvh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3litlrvhp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3yxvohlrl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3fxuiqdqw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3qilimdbz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jwytdfgc.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3jqcnlriv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xlrhgnvr.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ifpukmpx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3mkeyctgd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3zdbdlrdo.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3zhjsnxtt.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sfwaoeqt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3dkhxufeq.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3ebmwirce.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3cowkxvws.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3tjzlamjx.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3yyyllmrv.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3lmdvvpmx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3onnxsdma.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3cmnmralu.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tnhuotrz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3vsqlmkma.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3nkdjqpoe.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3mfaofpdf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3mzqlaggd.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3mpsteqrw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3easaipgm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3jyxrzjsc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3qplwzyur.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3rvuuhomw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3esofajgw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3aogrvnny.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3anixkpju.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3olavzaxc.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3spymtgbd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3dzjkaawh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3xslcdjom.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3nlzxmozu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3zfxzuxrz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ppiulavn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ttkjvxej.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3gppjsyzr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3whnvpwvs.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3wrduzqco.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3wsppcprl.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3lkmehvhs.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sobksnyi.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3xjvarjva.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3cavdulgu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3fkthvued.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3yuvxkypk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3hvrmnmsh.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3cjjmzkih.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ccngknqj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3pvumkwdl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3baijlpif.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3dwkhccsr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3skhuzjor.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3abqcrkrd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3uebmxzuf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3yaejmvaw.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3dnoieqhx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3essdfuoo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3hamwlttp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3tcroeexf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3afrmjyvm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bdbaoqdi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3qgrdzswy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ufikbagm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dgjxogqk.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3rfxfrveq.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3neygjxtx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3tfieqcoc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3dvurwjap.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ehfogrbr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3luwoohgo.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3nuufbyxf.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3emfeyxrb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3nuhbypxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jnwjamew.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3clxokwzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qhcslshm.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3mrghzazj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3dxobdgnf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3bzltastp.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3wezgofda.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ymvvhunw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3lrtjgamh.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3aasatiso.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3rzvbsdbf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3vppqunmx.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3rdibrsmm.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3fhpbowbx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3frxytxka.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3xblnkmuo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3lirmidwi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3fzdthyug.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3hdbrsicy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3zlgwacou.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3dsamoczk.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3ytrcxqit.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3odfndcbk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3etdbvguu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3lwxxzhpi.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3sqxuzmbi.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3tsieeanb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3wsfvglga.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3hdfjkfws.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3fiwedwsb.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3udxucake.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3ywihralc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3dtvhsvpn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3dshjxjtl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3igxsopaz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3nmonxwxk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3oeemftct.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3rlgkmkfm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3zrianxmd.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3xrkfyrcc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ivsbqbvu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3wikrfmuw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3kqdkextq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3bbgqvkzi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3vvwmmsfs.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3ynynefwp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3aeeharro.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fzrgrcil.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3omqvnvct.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3pzjkbyuh.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3juystxaj.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3bsrxrazj.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3gjqiymte.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3twvoxlcm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3nubicqbo.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3flwqtjce.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3dkvkzqmy.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3cefhtacc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3azfqvkmt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3varkzzon.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3adasblxm.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3tkgwfeoj.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3zjhcwknz.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ykczbucx.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3eurlcdcr.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3hzsklsab.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3uzjwwgzh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3mabgwlir.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3aopvgifv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hxraovui.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3eeppshns.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3sxwkwddy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3jmjgdkxl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3lbjjgytn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3tiesnjfs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pwjmunlv.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3kgskvyuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lazcixfv.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3huuscqii.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3tvlyqtef.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3amcclksx.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3slcawidt.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lnaaerwk.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ccheoomn.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3crtfiblb.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3acdgsxxj.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3woqoctfp.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3owzhuire.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mhzkpinw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3knptxtxq.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3rocauxhi.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3gnspwaca.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3inorerov.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bpmgokuc.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3jgzjkelv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xqbhhbfb.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3yrltglyh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pxkuzbcu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3mfrklbmc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3cjnotslt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hmsutqcl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3knkjiovr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3gstubaet.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3ckrvsess.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3hbondjgs.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3twnngcia.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3lrwvjxvi.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3jwvecelt.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ommpnuet.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3txbjirtx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3glwmjhyj.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3oqzdrtuv.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3rptitadl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3mhrpkaob.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3nfxadfix.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qrvkrwon.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3uzwtmfwz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3etaujnft.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dkmosdxp.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jytibhpn.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bhmvmkvc.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3eugvhovz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3htlcenre.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3coxgwdsa.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3uvvgfevl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3azjnmahm.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zluebhjs.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nfretxgp.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hfdueies.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3vcaycwci.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3pikezuvc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nctkknod.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ksktdqvi.html


<!-- 参考信息 -->