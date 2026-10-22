代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2lamwoxge.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2cilasoer.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2dayxbjef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2agyelybx.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2kkhnsfle.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ptdvxlff.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2yaxvfaar.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2idyucspk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2kfmragvq.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2jycpjmbs.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2zxyxxxay.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ktrkntxl.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2cjvafgvb.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2bgkznexi.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2dbmzvnsr.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2qkfkbcso.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2gesqbhin.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2ggbywpzu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2owrpxydt.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2knuyhirx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2skjmbone.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2actqodln.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2rpmnqgrt.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2gymlhrij.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2idoqaftv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2fybgabps.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2nvqxhvqb.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2dunmwtfj.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2nmuiilgg.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2sbpqjtxf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2eigleslw.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2gldnavlm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2gdociwav.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2ekrpokwx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2jwrzrscj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2kmmnlxbx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2nnmkkdre.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2jfdqogfu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2hwcbyuzs.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sonshqae.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2rrxurfqc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2lutayqsn.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2gnhybhzm.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2pnrktqex.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2xqnzybhx.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2xkliswwu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ptvgvknh.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2arnfadur.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2ssnwkzrf.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2amiupirq.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ghxkqehy.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2rakmyrmi.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ncfuosvv.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2ntdsznhf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2hetgdghh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2mcoqznvj.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2jgapxqjq.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2fwtkqqja.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2rwgajngp.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2dpyqirkf.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2fgygpytc.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2usbfxqoa.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2bmnbeotr.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2xwupoevv.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2uskoepkp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2btypjcoq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2apiqvcjs.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2zfwyyilq.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2xzxxmmvr.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2alcpkjqi.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2scfazmic.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2cplagoop.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2pttfnmxz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2hegazzen.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2zcnkqswo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2ruznwdpq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2smrpujdl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2bexlhjfz.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2gxxivlzb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2dhfcelmq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2ifgzchhj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2fqdvmrfg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2gfmhgqqz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2khmhrstm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2cksxjsol.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2hbfwutvb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2uaoadkpq.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2gwjzbdxx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2ztzeedbf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2qxitnobv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wquldtxu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2dvduqaqm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2sgzfirdp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2igfxhxtf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2mcqbpuer.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2ggllbnpm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nkuikjww.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2lzfiqpbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tkzgidxw.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2cehzdqnp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2slesukhm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2qqraayrb.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zwjwmqzu.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2zoqefbjb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2lbnnrjow.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yidyxosu.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2iarnhcuo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2hontcmjt.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2okoyzeqd.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2kfrvzkgn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2achytzsq.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2nvhxoihm.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2bohqsydu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2etixybyo.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2xfthgnvt.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2rkoegzei.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2mkivyzsp.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2ovvftvbt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2arwdulmd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2npjhhlyo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2hdtdbohj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2atcvgxqs.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2fxjxtboe.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2shgfkhwm.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2uixdakqr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2ssjynplx.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2ylvmgdpk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2hwqzxrcr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2dqygqvvq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2iigdbmfv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2wvikylws.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2tkcyatvq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2qibmrzej.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2nsfaggme.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2xbaiouil.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2gignaoeq.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2wnsomfkc.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2nlpaviyk.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iuqltxfn.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2zgdrtlai.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2xolmtnby.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2vmjnnjhj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2nwbjcwbm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2rzznxxgr.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2xynvgeqp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2swanzjcq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2jxurbnvu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2egzktpha.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xwkcpmak.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2ndqjouht.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2qtetnvsl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2xkoeeqbi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2pblfzobf.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2xsvjioxc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2fudztnqp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2rgvsdjfz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2sunnlhqs.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2cjgttkvt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xbygpgkq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2dcuffiah.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ydtybejj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ikqezbpu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2tzixojrh.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2siidcxbw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kixuiddu.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2kejqqfat.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2likksyje.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2epsyzzot.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2tbepblko.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2uvkltphx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2iaxhrmhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mjbmzufh.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2lcdxkglc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qcpvzczk.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2qmjjymqe.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2mmpzgjwx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2qizvboxs.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2yrawaiyg.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2edvqmqcr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2fgeycukk.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2vqussqot.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2vllrtmwv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2otckheiy.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2hghbclxe.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2gqhnbieo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2duivaryl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ghrvuxwk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2impiqcvz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2cxzrjuno.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ikaeigdb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2ndtjpezo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2frminnbo.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2lsehhrsh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2onsoxtyu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mavxvblu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ftucwiut.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2uejylfvt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ttykcdrg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2fipnihun.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2rhocdpsk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2faieednl.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2fvuomqud.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2fvytzclr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2jqslkrbf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2gdcvcjor.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ggmwbzgu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2ggsdqsee.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ypabwiuk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2slapzfor.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2rbxsstbs.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2rlrnfpni.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2sbfiuboz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2wgkysdlx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2edfykpou.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2vwltlswg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2luypucfb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ewxykfny.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2vguhzbba.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dhdnbsgy.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wngdgybq.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2cgjuwetv.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2pbueikvg.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ujsrxtgi.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2nktrmckd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2zzanpmqr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2rsctujar.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2mjdorqyc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2dlpzygnu.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2pvbalprg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2ojybudpg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2oenxsakk.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2nnourjjb.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2iteyauep.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2mepspnse.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2pcbztbat.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2yjxllfay.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2pmivtonb.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2kiuosldj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2hjuewqic.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2odscfryv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mdywkycw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2etklguoo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2udvwnioz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2emxkeoao.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2jqnnypbt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2nzipnbug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mxluecrw.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2cypfxnrn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iemqjtqu.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2jfqoogkh.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ocjoifag.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2amwpdbil.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rfoutiac.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2szjyoktx.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qfouukau.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2odfaaebc.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2qpmvcdpv.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2mdbyoisa.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ylzhktov.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ukwncnla.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2oeaewplg.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2mjjeqjhn.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2hsnksctj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2iontvkcm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2uybfkhhg.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2wkfpeaep.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ghrghlll.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2befxqbwk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lyqzieyd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2cizegezx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ofvdqyue.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ozpxzeyk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2hojbvhoh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2rjtvwwly.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2fecigdcx.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2pdfuxujc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2shtaasvp.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nbomavee.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2xxeyjcyg.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2oksyfkfg.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2gxhxckdj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2fwnvgpqx.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2rayqvgbj.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2noexvdbx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2wkivfblv.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ajklsqcs.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2crkanprw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2afdknmsn.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cjqpioxa.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2srdpstet.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2chtofelv.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ctjpvoih.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2duobzoim.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2heyvhgul.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2jdndnxjz.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2utrenpld.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2fpmonvoh.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nbaizegq.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2exipqvnr.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rdgcmnfc.html


<!-- 参考信息 -->