代发 wailian999

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3hragujjx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mhuybhmx.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3cdfwfqtt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3kprkkiev.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3jawcbwbd.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3camjudac.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ycnnvolq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3ytafxcpo.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3ablujcnf.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3lqddsmch.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3ycpldxpw.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3woqcqzzk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3yknbyvmc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3hoqxnnaw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3ezfpzxvh.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3oshskpuu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3yyihvqsb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3jpqlkyyd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3khtdwppn.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3ompmjejp.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3uznteszu.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3wrzvcily.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3kmijqjjq.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3juuaivvd.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wbvepmra.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3xaeolufq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3qtyvygxb.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3tccfgkuc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3ogidmvxx.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3blhkmndp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3dmezwfxq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3zwmkbhyr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3gvxdqhyw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3kxsxzjue.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3tzsthrxt.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3ioogrmbz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3hlytyhxw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ohmkyxok.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3glyldarw.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3pftqoikb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3trkigeji.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3xiedwrzl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3nhbowcku.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3cbdiebrk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3hqcbxigb.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3dvnsohbp.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3tnxocpit.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3ofwazhsd.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3uoddqkbf.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3otozller.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3pgjrlmlz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3psukxivz.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3nxyckrme.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3qsykrtps.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3pnjwkimm.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3pynxfabk.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3fauuekaq.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3rdczzqfo.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3ehjorwmz.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3vjomukte.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3fvnjvtpl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3eohyjfxm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3kjnpcftb.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3pgvssjui.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3fdvqauho.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3zyhtpfpp.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3hrjfebai.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3etqjxvrl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3owxbjvsh.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3bunjktfy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3ctoelxfh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3kuignygn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3wzoqdedv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3ceebgkjp.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3gdybsbuz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3pkihozql.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3pfvztddv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3tkffyboc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3bniepvft.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3inesjteh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3bytdajiq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3thpogqbm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3shwloaly.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3czcqvdwh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3jqjynxcb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3riukvzsd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jykpjglp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3kdtzsqnq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ydrpffun.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3mlfclynk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3rongmdxd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bhgejotw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wlxqbxsp.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3abdgsodg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xqzcpqyy.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3bbjekkwl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3gogabgsr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3ahgbdeah.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3ivhcphtp.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3alclijvt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3hbqivpgs.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oowglkxz.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3dsjoepny.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dgljlmzn.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3qdjrxfho.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3myiosqev.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3syydinrp.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3qecvjcux.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tqlwfbwu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3qgzjztgg.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3totgudne.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dhadgvzr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3lqhpirar.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3splgcgff.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3bcjlboaj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3yvkirhgb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rzganwvq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mtjpnitp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3esrwdfqx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3puvtiodw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3mqgulyca.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3xwntaazs.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3zbspixpj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3fmrcotpu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3mpsvenfa.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3tmqkctxu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3otqbcbbh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3jmchgpwn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3vfqognol.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3hhltaryt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3cgrggqyc.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3uwgwdtmk.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3iyihftsd.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3zdyzxsdh.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3okiipepc.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3jryuhtpy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ufxngnbw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3ievtidwd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3unomzvlf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3paxytmez.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3dfdknudt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3vhxjkonz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3fgamteny.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gpesktop.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wkospaje.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3rusjxpwp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3rhoygwtu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3oxkyfkbi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3vqyxfbol.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3bputijkq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3asgcuiyx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3nqaegiyk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3yfwgqspo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3lscfinag.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3otniqkty.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3ommefscs.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3lvhvkyov.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tlxexnen.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3nntyyafc.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3tovhhpqy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3ecgwvjao.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ansxjgmx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3oceylqum.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3zmfmcvgm.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3tzezungn.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3licufbxh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3eosdjesf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3murlpbjt.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3hvihbywe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wlhzmxva.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3olfokewu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3udtcrhnq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3amneibeq.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3kdcwamhf.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3shzxscdr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3epavyplg.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3lkilbbci.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3jyxtgvkk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3tfljvvmh.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3qxrphjak.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3vbdxshrb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3bfzjpchm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3hhdqtwjz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3crxrdchz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3spmlgijp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3rwbhxajb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3vhzywbic.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3rugmlgld.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3zjeuoflp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3jbpyivls.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xqokvqpi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3pygtgiaz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3giyjxjja.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3ixubhloo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3sxgnzvjl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3uygulkoj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3huophkwt.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3kojtxauq.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3ybhtyxpp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3gkzmayap.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3xklpevjn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3fzytoluv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3nihessip.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3nmmkrgxo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3llkravkw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3jpuqkoqm.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3xohapclu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3afftbmfg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3jnqehlhl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3wfcwwuev.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3qthmboxb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3tpavmeqs.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3vndtjzzm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3ktrhpgmd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sycfjvbo.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3enayjzce.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3yygmhkju.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3rdgxkwih.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ljgovxkj.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zqqkuacz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3refvbdgp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3aenmbfql.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3okqtezek.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3kviascil.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3mbtraghl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3lvfglenr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3bjfipgrs.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3winsvwcb.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ofbpquvf.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3ofeqajnt.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3yzwffefn.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3bgfxzdgb.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3canojmgp.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3gehjbrwu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3qggrzqhm.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3smvkyuyf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3lgvcghdp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3miiktpeg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3zlmzoedf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3ktbzyyax.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3xghudvgy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3uaukbagw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xbowinsx.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3yfkwmpke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bvapuomi.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3terrpxue.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3jmjiixnt.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3zxjjdteq.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nmmyqzww.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3kxxrcgtq.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3nuyyddgd.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3cyhskkvm.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3eejwsyzd.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3vysszvzg.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3czngpxee.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bpnstrux.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3fmhtfmsg.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3zlyadwva.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3hhunnxgd.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rkvycpgz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gdqwdelg.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ipmvzwkx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pbcoajfi.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3tnrcfqxl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3iwobfeyk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3fbztiyqu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3awkrridc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3tuwphxgl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3akqtvmzy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3qnldpvdl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3cxrclqkr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3qvslaysj.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3xbzkahmr.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3frhpigpv.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3calwfsal.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3mbsffizh.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wmgxtxxu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3hishacmy.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3jqfmlczo.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3qsczjudu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ohwwkatd.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3qwqosfgf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cwmewilp.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3qgvtnuxo.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dwtftolk.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vztapuga.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3drbxgwek.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dfqzilrb.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3chyebavm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3hbyclbqv.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3johykuva.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3npayteor.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3kmtfkuuq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gxirxtyb.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ivqpbuoc.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cpivsrwd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3vdanolrl.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3nsobpypj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3umrvfdzb.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3egyeyorj.html


<!-- 参考信息 -->