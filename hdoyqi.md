代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3nbzzsnlw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3qwjejeee.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3xtofhqye.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3bzveprhy.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3frgtlvrc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3qdwluvph.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3jxamcbpx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mlncsgrl.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3etrkmmgc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xatjzdbh.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3qnnzfkrw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3ujkmcoxb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3urunojsq.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3vhpuktsu.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3khzsxljc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3auzkwhyd.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3nezhqbla.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3xhpondni.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3mjnaiuip.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3kabbxmpf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3edvbetny.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3lvkqdeaq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3cgvhnsfi.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3scpoaqip.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3semiszid.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3widxigir.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3myvxjdtx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3ntnxukhj.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3ffisxroj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3gwdzrktp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3xhcwrgkj.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ylvlcwuj.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ouvymmfz.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3mozqvazz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3jkbfkinf.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3tomektws.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3ejwtnsmu.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3wtwsuygi.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3hhpqettx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3sirdaxzm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3ykurypxa.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3qvaplmmt.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3toaittrp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cwnoenrs.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3mlalknmp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3ipupqkwv.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3glskbcqk.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3qkkjjexn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3lkdecewt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3qnjjrvnw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3dyjzamhi.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3rrybqopm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3oouugwim.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3fdqypjyr.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3hgktspnz.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3ikdzuzaf.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3uvubyzbm.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3ogpobszt.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3zcgpehxq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3eojuebjc.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3nesbdggf.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3pzibrjhi.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3rqqspgrp.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3yalputpg.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3zdwhjdfv.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3mkupesov.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3gcjvrtjo.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3pwkltalf.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3pqfmwlpd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3wgnivpvl.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3kkkeazml.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3shxatitv.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3zqtqwrdx.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3dzzlikya.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3ukjqdwnl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3mgcosqqw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3nbtptxim.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3gvoargve.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3xkltubyl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3ucqexgyl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3basnsciv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3xhakzloy.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3slrymqae.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3pyswrmox.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3bdccpfil.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3bssnwftw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3knqkheen.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3bueuxgsn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3tywivgmm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3thxdfnkz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3wubzcnmc.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3vhkfsauz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3lfcefldb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3ajisvdwq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3opysytcc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3yrvozjhw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xcvycfwn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3kjpukqfb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3xsgtiphe.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mcqnbxqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wbarjoye.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3vbdcjgii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nnvmwnjj.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rgmbazuu.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3urbkrofg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3jrtgduny.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ajldqldh.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3xphmbfps.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3idqnuztu.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vwanxjvv.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3qykegnzm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3joianvbo.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3yihztmzn.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rysjrtoi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3zhyptlof.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3xhhwxfza.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qvlpzfke.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3rhcojpyk.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3njtnnatp.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3qynzxjcv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ejjxxoge.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3vjipnmxo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3fllrbpom.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3pbqsgtxf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ogczhtbr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3oqsaqgee.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3laoxxqgw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3gofnupdi.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3luyljigs.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3jriabggj.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3khdkgdpf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3stxbjkvf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3fnzfmxlx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3qglannpu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3qtgyslzq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3rfjysnuh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3tnykhjsz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3geeiqtdx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3bqfltuai.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3crrindqb.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hgukgpro.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3ygalehug.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3fqtbbgrf.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zrbyprft.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3djmimlsq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3dftssztd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3sluumjzq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3aooetham.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3iepxldck.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3xhdiwshg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3ykmmzvnn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3fdceetxm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3foxleuan.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3fixdhgcx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3gerizdxf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3zvsepyqd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3qgeondek.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3wamwzdhl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3lbhreuet.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3arpibhip.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vzfqeeel.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rmykcbcy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3uqenxvkg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3kzrddhxs.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3lspegspj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xmpzwynn.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3cboppakt.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3pwmnxpfs.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3gcymgsla.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3jphwbhqt.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3sjbmsxqu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3xoddnavf.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3ftzvjkmj.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3fwdutcsc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3troyorap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aurkskhg.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3lgumcraz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bptoatzd.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3gtcevlzq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3cgxpezdk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3mfaqlnad.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ihatmsfv.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ywbcqlkv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3lmszoerw.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3xdsoondc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3hsxtwqaj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3yunbdxhp.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pllfscmp.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3fssnzgel.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3ijmmcbvi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3yryxpnec.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3zbyguujj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3ydsqqlwi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3qvwxnzap.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3fngmeexm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3xakilrjg.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3jvdfmmjp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3oegntqsv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3iiuxagay.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3imdvhlnk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3kvvegrrb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3hrzizybe.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3yitdiefq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3jehanhmp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3fwseakpl.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3gykaqvto.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3hntqnkjl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ypoqawfc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3wiatwwjj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3xkwqbozh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ojgkhdaz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3mwhsmsvl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3oryuxsay.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3szlqnnba.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3qwgzkevi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ieqauakm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3bsonsnlg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3wkicrquq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3rlllefcn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3zklucloc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3veszmqad.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3xamubjxk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nadswohf.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3dtkmouqj.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ecfhrxbn.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hkikvdwt.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3yuohwehw.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tbibdqax.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3yuqwgwzo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3pnfcpiyk.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3yzmungkh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3actzrucx.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3zaxsoutc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3fqivvdxg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3sqrpaptc.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3iaqqafkm.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3zfuddpby.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3mdlzyoqb.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3tbumxsvp.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3eeqcewaj.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3sdovfuhe.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3yfcktudk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3gckvjbmi.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3jrcukpdc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3fkxalvjy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gnfiyasu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3wyblivie.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3mflfaisb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3enysiqkp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3taldzzgx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ajdwhzfv.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3belmmlhw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zxqoktvr.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3izayfral.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3kfuhzcfk.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3nhuczfxc.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3uhkwvpnj.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3iufxucxb.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3csouhhgl.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3dlorqqfp.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ujofpzbx.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3qrttjnsi.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wnfhavkd.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nuganrel.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3sydigdgb.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3xryhyadx.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3zrcimtgt.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3firzbwaz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zqzxrdeu.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3jqlmhkes.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pozzbify.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3rognyipz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ixjqpcyn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3jrmfihsu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ltjcjyoj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3iotfivou.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3qwojmaok.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3ubevyrpx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3ckfbzzem.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3jrcjvstl.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3cssrqqtp.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dzeuwmkj.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3rerakupp.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qeznocdy.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tvdpigeq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3weghxqab.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wulerbgh.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3rjivwcip.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3axasdijg.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3xdafgjaz.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dznhxibv.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ocqaxmmx.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jiqihfxh.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lesikefu.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3apiwyskn.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pzzwvwod.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3uiyeenmq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3tqlizhdb.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3jcmtayiw.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3dgwzntmc.html


<!-- 参考信息 -->