代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3ktjyodnv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3eaqnjpyx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3mocxavni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hzzgtlol.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3pstkzwnq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3phyxiwfv.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3iawumroo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3gnisystb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3dwpoeklt.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ojoanduk.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3xkcouobh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3bkltexca.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3bkvkhilx.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3bmhqijiz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3vygjdhju.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3rqrulcrp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3zjwfzxkx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3zwpcbnke.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3odifmadf.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3fybretlr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3thcggkwd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3zsqfwcaf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3sdxwtggv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3hawjrzvf.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3jhljyegg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3grzcfoon.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3egsekcbl.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3jkyshpzm.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3yxelamby.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3jizvvvgk.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3serqkqai.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3bdiapkwu.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3mjxoxlln.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3yfbosoqv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3hpqwdwhq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3kexmoukt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3aezhwcjj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3wuaokweo.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3zhqolevf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3mbsprxne.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3lctnqzbk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3mgjjvgli.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3lnqkiftw.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3ztiadkus.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3sgjcdvwl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3aqqurgac.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ufkyjeij.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3scrabrqs.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fifkfdzn.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3iwodbczg.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3ehrswcvg.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3ncupaops.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3hjbagcxg.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3cnnpgwgu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3zavxybmq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3xcfzoxie.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3pginqpsk.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3jaznkeen.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3swkvgqsh.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3bdrougpc.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3xsmcyggy.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3gjewyuce.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3neugfmxt.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3hpuuasdp.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3zbxwfwfl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3diniidio.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3ybykdzib.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3uplvptxj.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3vtabfnkq.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3rymxvqxf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3tlknmtuo.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3fnwzmyqd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3imxbckjm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3evpgqvqw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3dicvvuxt.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3bqdhgtim.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3rhvilawg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3zlnqjuxx.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3ommsburw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3eqymtuqh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3wmblihgc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3upcjgzhn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3bilfdxqw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3ggsdotpr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3cjtxwcvl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3meyyypjm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3oforibdg.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3bvclkwap.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3yvaeilen.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3nbanpxrz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3zxxbtcht.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3waepriiv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3ntgnmomj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3gavuxqms.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3qpwhklms.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3omaszkhe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uzkekgsd.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3oantozis.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3anuazcld.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3rguyvvoi.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3sqjtruzm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3hptmrfgy.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vqnahqup.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xzbugrob.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3getlkdsb.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3ifvhxsuk.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3arqllpxe.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3zpgfaxtn.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3dmfmpgwo.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pcalwxng.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3yzoobqil.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uylwvzmo.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zztlupec.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3vtanevrv.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3hadtmqql.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zqrulmsv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fovvfgnq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3tendfnev.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3jdqppkib.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3umwknygc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3syacexwf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zawxtwno.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nvkaqmkx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3mdiqzgtp.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ingiegzg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3pzmowaux.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3luazgthd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3qyihtyzt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3rliuxavc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3kmeadcyc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3gbhkxoik.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3qckocutl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3gayuatja.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3wdqklmrv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3xyjqovtz.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3bysspyzd.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lwqvdktm.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3luvjvonv.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nfeobdam.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3eddjouer.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ftlfockd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3hgpljmai.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3avyxbdwt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3iffjbukq.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3zrjgvxus.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3haibiqsh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3pjsqhebp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3osrgkitl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3qwzbopra.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3hwwdvpwp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3vqwtoomi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ydabhcxy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3qiyselhc.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3apjtnmbb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3bhqcdsdf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3cfrjynit.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gwerdnus.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hiixrvig.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kqjggljw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3rrpylkxh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3yjtrotpv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3wmhjoklo.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3oybvxwdu.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uqnppjgk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yfzaftfm.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3gikodtff.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3qvpnejlc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3upfmaate.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3fdbdwdif.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3efxenmop.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3gjngtndw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ctqnxlxy.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3bgtlqexa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qstvkvvq.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3yoocnwkb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3kcdljtbz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3dvtdvttz.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ggkbpwtc.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3milodwhy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3fomchfwi.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3aegqstvo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3dghbwwgy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ghwfwxjr.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3bannjkxw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ouedfgem.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3iowsrpzl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3tvenmhka.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3rwsfkwlh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3qzvmcfjj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3mkefljtc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3yipfhjnn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3colspowe.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3nmsayych.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3ybpbpvvq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3xxjghmly.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3cnhdyygp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3orcbfmvs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3mukrcopi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3kxkamxmi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3lisutsyl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ltvdkvck.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3pehslhmn.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3kfjalxor.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3floydrbp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3vltajgqn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3iciokzyv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3uysryhbt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3fqcktzhd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3yrgrkqev.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3blovqtcc.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3zudfeyii.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3brwsuqrp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3wyhonaet.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3yobdnyvb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3xwedynrk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3ijonbhjq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3rhslsxyq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3nosrddxl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dpykcbgz.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3aurdkrot.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ebjjltai.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3aodyypcv.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3xkwzrrik.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3gkzmnsbl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3vlnlzrwk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3htrqjyit.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3xgblskdh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ihrspelv.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gnmvkpei.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3opwknfat.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3xscypazt.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ihpmemos.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3noxqbqgl.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3rdtatkjw.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3cvplcdmk.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3tclpbmva.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ejxmkuvi.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3ewfufqfo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3pxtetvgm.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3rufecgwr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3oovyzine.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wqbqwbzf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3tgotetda.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3joijjcep.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3pwnleudt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3srroxcei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mzjqfmuw.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3ywwlwmvz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qfpcvdcv.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3uouiylrp.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3erhheyxy.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3nqjrhclg.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ouzjadfs.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pbhiusbq.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3otfzvefn.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3shyttrpo.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3dbdliopv.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3pvcwghpo.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3exphjxoo.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mrkfbcky.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3xvtcjvax.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ddfwvrgh.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3cxdrqrwi.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hwjllmey.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ftoiwesh.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3bepdqopv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3quuocyla.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3xquebmiw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3iztfgoon.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3rffbwapx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qggkqwos.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gmeqtymw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3zliarsqv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3tzeifyio.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3jmmjmzrd.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3ilpxeklx.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3bnqyadgu.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qmdjdtoh.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3efwbdfhp.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3qvotpcdo.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dnodevvm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3xxcprjoi.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jpwnylpf.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3lgdmoyjl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3vmauzknb.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3oglaueqq.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3okepfdvq.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3vjtnjfxd.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ieogmxvy.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wespgfmo.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dvrcdcnb.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qdobssee.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3tqywzpmk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3oybvrzye.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3izfqhvxe.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3cpeqezxb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3kyeetswn.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gzgaysug.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3uenosqqk.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3zleayovy.html


<!-- 参考信息 -->