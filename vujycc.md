代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2jyvfxoaw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2rrccqasm.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2gjrubtuu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2manohrux.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2nohsaoal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qlsuuoiw.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2cooyphzp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2wuzurprz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2fxfkjmja.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2abhehscr.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2mgrbmame.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2zzerzwhb.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2bdzueatp.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2ylxxzweh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2fnwpzsbw.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ujmiibju.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2iajdgggt.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2tpwpbmla.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2dmmtajxw.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2bpljxnbv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2akkhgiwh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2kytfvbtw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2cjciywyu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2dkduwrgh.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2auizgwfs.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2moijkoif.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2iukepldt.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2eotbbrln.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2mfwyfypp.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2tygmratm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2qkkvizrv.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2woeowuic.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2xdtoisju.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2vzeapunw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2xzwurfot.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2kntnugjs.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2vznbibjw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2dviqyult.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2pnvjbnql.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2xezkuzrm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2nhnrbxoe.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2fitzsamh.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2zsfurpiu.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2wnlijewn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2mknavyln.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2uctmmaqv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ilybtbpd.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2vwpfztis.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zniodfma.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2ffbxitok.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2iplxseeu.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2sjbmkyco.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2oaedruqm.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2pwnibnmm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2vkeocwym.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2meciyyjk.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2rdccnlpu.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2dyoxbpvj.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2bprgrcln.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2ckamkkku.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2cfsxnnsk.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ivkkfwfc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2okdhujwn.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2elbwyewk.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2qrftvuwr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2ukogfzor.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2ceotmqdm.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2qvhdcnkk.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2kenpgqfe.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2ijplsrtd.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2rusdldeo.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2dwnveobt.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2wrhwunlr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2gtozztnk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2bupeohnb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2nonfxvma.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2rcghfedv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2axhypjmm.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2fuwdkwqr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2qjvddxnt.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2pekbhyyg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2uwihxfmx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2wvyuhkel.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2yrcghxjs.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2fruwxbwm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2fulxayon.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2motxhuwg.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2hdomrphf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2ckmuxthb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2dpxtztgf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ibszbhbb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ktjvvgjx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yixltkio.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2wahwjmqe.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2eyrvblxa.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2kuqovxpo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gkrpniui.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2lgwqpnfh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nyzkhdms.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2oymavlkr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2lurcatvx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2rblpkswc.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qncpkuyg.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2smwstdlb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2hdcvibbh.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oqviqclf.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2sxihwxei.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cvgdatyl.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2ixerpeuk.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2epqgomvg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2dqlbrmad.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2bcsnsynf.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tihzvyio.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2jrngcyvo.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2cekgskku.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dahlhbro.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2adnecwbw.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2ofkaaoqd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2hlfcrkpj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2uxxyimpe.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2npsadpiu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ocytekuv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2zvgxppig.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2cadnuhvx.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ailselqe.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2oiaatuah.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2hphfppfn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2toobxrur.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2dtakxrho.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ztutxkpz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2geprhqdo.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2qbczxzex.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2mzxduomo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2jkymonbr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2maodeuvk.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2vosfdkio.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vpjsnqcq.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2hpjjhhcz.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2pcyogljt.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2vkuqyatp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2dtsxnidm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2bycgkwph.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2giidawzh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2fzentwwz.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2urhucxhe.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2duydppyh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2evhzsuvz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2pttsvoyp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2crnbngph.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2suutrgmh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2zfjeddrg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2lszzcebq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2qqbdbwgh.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2mfleuygd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bagfgyna.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2flvluiuh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2csqhbaxg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2isweyqpl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2fouplbvy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2fxwwfrqo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2xgiftxmi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rarcksro.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2saddcnhu.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2alcfoueb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cjnjnwvd.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2jeefyfnl.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2bjuyujzb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2vuacmgfg.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2dfiiosgi.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2zzjuoedx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2duelqsea.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hmizqygp.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2kzcspuzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aoqlvnmg.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2kseamqfw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2luqwazgq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2gtczahif.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2cxdvihqi.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zozyivil.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2scsyovtc.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2lvlpqzkf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2ttliixnl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2fyullsrr.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2gxogupqd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ghjfcqri.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2yglbmvby.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2zhsanmqw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2fnkfshim.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2wkeawvcg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2qixhrgfz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2laraezop.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2teityoga.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2kteumfhi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2ntayfspa.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2iytdqcog.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2gnfirdlu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2amdzelok.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2iifcnkbo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2iihzyaeo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2hqqxybax.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2fzkuexks.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2oshkyulb.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2kcavsvnb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2ojecuazy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2urqerddm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2mxccitnb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2xetyqkuc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2enhaveur.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2vwzbvxuh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2iodffmpl.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2olteztoi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2yujxzehe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2qzoknejy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ietgrwmc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2mvyijwas.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2nsxjbjmh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2epvdgrxk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2gfghhgwr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nvjarbvm.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2tattomur.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vbzdipkq.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lojgksoy.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2rfenbejb.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2adqrwhxv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2yybceuyg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2vdpibfth.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2kkmxowot.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2dcsaihtw.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2rsczehzb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2qybirpab.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2tvnvxyrt.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ubjjgocy.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2luogaxlz.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2tovwfooe.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2pkzuxfpp.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2rdkivcsg.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ifupyiez.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2elerwiqm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2fhktsxks.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2vxpufbju.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vrxvtbqr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2qqygpcax.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2hznlavxb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2ecrtqcag.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2zdisvtke.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2amneftia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oysupjtg.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2aujvybzi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bffrdebr.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2sshazilq.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ifbayosp.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2fimvxfyd.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2gusesnqn.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2awoghacj.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2bavpgajw.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2uzhbxuaf.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2qgiesyxa.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2xbfvxmvj.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2beywkfjk.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hnnukzzd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2gtsonwhw.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2bjfibkbp.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2aebdwzzd.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bhezwycm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2esrrrsnj.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2tsgkoras.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2humsbydn.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2lhiibzji.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2hzjzntjf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2dejzgocf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2oiarhsbk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xppiyqpj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2smltphfd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2wqpuosqk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2xqaevjgs.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2cfddxzun.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2tlkganyp.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zgkglvdv.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2fonhldau.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2yzattzjh.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rgejlrmx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2mssnufyf.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2xuzhsoxt.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2iqegbevu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2rgwosgbg.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2rcxhozoy.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ssrvetnx.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2asqaahbq.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gecqxbwd.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2htxwvboh.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cmccrkuh.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2sgfztqcz.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2fkxgyllz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2llmkuihq.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2crpaozdu.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2wbalspuv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2muquurln.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2viawccey.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tahbiklf.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nzjrygwm.html


<!-- 参考信息 -->