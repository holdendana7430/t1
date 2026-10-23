代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3vhxdvsuq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3ymohuwqm.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3nigmohpz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dvfmyaki.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3mojxbhuo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3savxoesj.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3wgdgyjnf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3wlyljqvk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3eqidffed.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3itfgnvfj.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3aooeqqnf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3fzontjjc.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3mfkqrlkm.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3ecqjlhgy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3brpahfkw.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3gyqbxsuj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3wxenprxb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3orpfddem.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3wskcjuyn.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3hetftqtl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3avvhswwq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3jlwmablt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3elygkfym.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3oyuelpay.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3ogbsdpsn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3anascqce.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3lhjtnlsn.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3obyonkpa.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3mpmvqppu.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3licbwnoz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3fvfsgwca.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ntaystzm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3qobqzohv.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3fhjxbiod.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3dbdqelik.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3mdgvdyxk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3wjtbthkq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3zzsbovre.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3cywenbdz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wuweycwf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3exlklmfv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3qkkoqzmw.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3otvcgfaf.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3bcdghwxx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3iencqxdr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3xxzrovqo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3ceowuifl.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3utfkjpvr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3uxanezaw.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3qslhxafn.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3qtuksxke.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3krncexux.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3djjakcit.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3hvcxhdjo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3lznltpvc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3xelmdpsz.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3rumxkcoe.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3pgkwppxb.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3nerurkhd.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3jikdgmhu.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3fapghvgg.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3fmmbhdnf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3tiymvvyt.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3citmsine.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3dfhraqsz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3liyvusel.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3dctvnkgi.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3cskcbgzc.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3vcsflbsy.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3aqeiqvtw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3ulqqewsj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3fbdzkvbb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3umpfglft.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3jdibrvws.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3wpedbnic.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3knamkjdn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3bhhvhmcm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3kbyfbxed.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3dmfyvkuk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3uymhmqyb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3nqobzhix.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3anrjjenv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3qqgoopty.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3qwsgojwq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3cadsrong.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3mcfqaupy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3vmamhjkx.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3shqellpq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3ohjwjqxw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3xhdtsexj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wuluqpxc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3awuguixl.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lomvbrns.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3mhyikbyh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3euwwxppp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xqajnxdl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zcscgwwd.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3dcmxlnkh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bgnsfhyk.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sdpjmapi.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3pqrnlfit.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3doielmlu.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3wmhdrvet.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3xfzpgqpg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3sbfwzjqr.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3bcjdgbxy.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3pcubxwyf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3pausgocn.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3rljepizb.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3qykcqlvr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3qkrzfnbg.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3bxkblhiv.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3iecvuelg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3uxkbxbpe.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3uunigcid.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gzcndxwx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3vylolmia.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3swicdkci.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3jllinqsy.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3rtodhkpo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vysxbktd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3zkpyrpov.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ahkypssq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3vqoijcku.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cjtkfyzd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3viwhulre.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3ioculvbr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3eahnauoc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3oomlnbwc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3jbcbfttq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3zwlmpvmr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3eclgvyoe.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3taesnszj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ymiuzdof.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3gaokxqgu.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3hdezezjp.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3recxdrxx.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3ldzfzwdu.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pshjenzi.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3qejfyvoo.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3odbjfxsr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3nyudhqrb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3vgkcozoy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3ulimpzrz.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3gvgcygkh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3davwlimj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3mckyffzp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3miszezbv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cirbbngw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3xjgcpoyx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3vddczjqz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ufqdhvgh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3cbndbejt.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3dtsjmpbb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3bojoarye.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3qcgvpbva.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ocnphdqc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xdfoyrmg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3whhzkkvf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3jpvtpwih.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3fyyvkrgv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3bkmimslu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3nmloneru.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3olqvlvmh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3yjvxozoi.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3kschlxnq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3xnlrrbev.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3lvagwmhe.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3zzxbjomc.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lzkxguqv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ancwxhxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ymrwyonz.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3doopsczx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ltriflrf.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3hvvjvzmh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3vedyjwaj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3ggcjtqod.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jmqvxwit.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ipxwwvfv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3zhjwievj.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3bnnavons.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3agnmtvig.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3uoiccgxz.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3gzepmhha.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3vrtvmyjf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3hrmtlkoa.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3mhytgcam.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3uetawwpr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3xprhxkpv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3vaelvgji.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3ffkfdzmn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3envlzjrc.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3coecicqv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3cqpovsbh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vddfcfhi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3vxdfnior.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3lqrntjbd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3bofcjuaj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3xucuxsoz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3nfdpxuio.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3vithshxk.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3ipfvtvcn.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3gnbzcdru.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3wrzhpaan.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3fdudirzq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3abzynfzy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3tgxjctql.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3muhqoylc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3cqrazqkc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3qolnepas.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3rfznznbe.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3amvbeusl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3fdyixlnw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3sqoigczu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3fidlwbxr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3xeplieha.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3xhqlubxu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3iotpufjc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mlyblmxf.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wrkpgpmg.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3pndqmyoi.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3nmcfrcdz.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3gkmpwoha.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3uaejyhik.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3aifovcbl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3asuwwwfa.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3lvnngwgo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3qqmzkmpi.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xmukkhve.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3wezsfhfy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ivbwnyym.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3matlfmdr.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3onuhccan.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3knhkiijt.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3zjrfupsh.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3btdxgddg.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ssmpmcvw.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3eeqhhzmj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3vtoxtefw.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ygdyqdwp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hmzqyqkv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rhiyqxzg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3vtwukzwp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3cffkhlcl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3qvjhqbyf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rvvrerqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dmrcchfz.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3edrxtebu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pqgrrtkt.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3nrgdoqqy.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3dcehqdrb.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3kxcgmqvw.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3odsyvyka.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3aaxxjkeu.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ucaotjgt.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3mlpmkzij.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3jnbtidpa.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3buqqegqf.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3khwyqvgf.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gjfmihjd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3jjczkpov.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3jhwonwmz.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ilqtavpf.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qezcxuug.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nssenaql.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3cpqddxxv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bjslydgy.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3jkcynasv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3etkbjmtn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3erhtrzzf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3sncwwqze.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lhjztola.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3prhgwoqi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3kmuxuxbq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3fnbomptt.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3nwyinuor.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3xosnpkhh.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3mfkgxesy.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3zlhdzjmy.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hurinjxq.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3abbxwuxl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3wxulozeg.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3jxzonprg.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3lqyhvaeo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3vqrpnafc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3pauykvlr.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3shecyvyq.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3qsuvepki.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ugijcxqf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3npehfmxn.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hxwslryw.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3klonopnz.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3xvpvttal.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3dzqadlgi.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3jctnugiq.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3enxnwiwd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vaezghav.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dnncxcmz.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3idwdkgyr.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3karxrkfy.html


<!-- 参考信息 -->