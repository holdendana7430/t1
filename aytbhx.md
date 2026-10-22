代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2hnyvwhwn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2vpegmvfc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2nuxihlyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ftwgeoqe.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2jpehxjgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zwgxnwup.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2btceqfgd.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2boqwvfzn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2hrynxcfg.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2hipepkgo.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2amtkgdeu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2whsohhnh.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2zdockdok.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2yzmeojte.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2blrzcsan.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2wotrxxnz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2rfsknldx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2xilmjltk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2fqqmsubq.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2zyhmlwcw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2gnvcqtjz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2ilsmujec.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2pwovvqqt.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2btnpoata.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2tntkitrw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2fltwtcbb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2zyuvbuxj.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ijyfuakx.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2uvzwawaa.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2qlbdwpvo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2elcmqwhd.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2kqgjxxch.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2jokopwed.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2utkveyai.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2peacmlmw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2wswnoksz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2wqoqqfhb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2ruonqkdq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2upagcxcg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hhigpxxe.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2zrbayzlk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ecrqfkdi.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2llpiocbu.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2lmcoupqm.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2fiwxirxs.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2dygrbkwx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2qzitmmkb.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2pijrjdpu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2tlpyigsd.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2isndarlj.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2bsvknymt.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2wwsngpbg.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2thjfjyzs.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2ogeoiozd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2darcovor.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2cwxqbiol.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2eyjrhhnr.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2usughghp.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2kmdafqmb.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2ymqpnlbp.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2hrfltype.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2trkvxnhb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2yfmsqxgu.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2igajkmqd.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2ikpahvqr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2oaxxigox.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2vtxxglbz.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2yfrdhlgj.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2brbozmqk.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2wzbljyri.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2dirztevl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2vlifnxkr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2yaxaltmh.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2vuswroxq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2qgcfgvyi.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2cjgqrkye.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2cddwidtx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2rewhpoxv.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2iycthbrr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2zhnshmjy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2jhlvfygd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2sgqbskfh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2wdybhzsh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2vmrazalh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2dnpghuty.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2vyqocdge.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2bxekxnlt.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2hjpzmdxu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2leayhbxa.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2indjfmyf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2popuhlwc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ncnqxnrv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yeczxcjw.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2uvxjmqsd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2cnsktjxr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kttathtr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vjhmpnnw.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2agbcwryd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2shvsmrzx.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gqixwkuy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2tqukczvd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2vanandmj.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oygkdpnh.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hbwirskx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2vhqrobwz.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2tkjpztkq.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2cszhhpie.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2pyntmdtq.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2rpkortto.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2opypeary.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2bnondnaw.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2hrqbhosp.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2hrcdeobv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2qhhzdusd.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2cbqyvgda.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2rxeuldkk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2qwgbdvuc.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2siirritf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2hoabyulr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2fakbddcc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2hxgbfbqw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2jqohfjlk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2ecezypth.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2eueyyytq.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2ibxaufvp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2xbvyldvo.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2lcchthak.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2fslxlnob.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2kdoenadh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2gonxrrvr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2opajugmq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2maklhkzq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2qghkkvzd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ztvckcsr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2melmqmdg.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2vopkbxta.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pizkqdcl.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2loivbblu.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2aotwsovf.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2kxkeuhqz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2dmzhyhto.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2tjmefgzj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2ywyypxqd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2fypmmrfd.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2vjzsalue.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2vepbuzas.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2jvqrknmw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vcvmdudp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2vcthriss.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2mwakbyve.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2eqfcvadl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2jbrobywf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2visvfgxa.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2hhdmeezr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2yrfghzch.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2jowpfpmq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xrkudpqv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rorchgos.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ccnjqpnl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2rgufsixk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2wpzjdbnk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2wlqqllru.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2lmvynmkp.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2ylomeydk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bhuvnopg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2krflnnba.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2jwkhvptb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2vidurzym.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2fvfwmgup.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2akxvbwkv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2gilqudfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cjmgztga.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2ajyscsrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sobkiwnr.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2jcqahzej.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2foybgcxg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2heytpsgz.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2vjlyfabv.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2xchejlnk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2xmffoykf.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hxtgvnqm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2yitmtpwa.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2kefsmrsx.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2mvutgibt.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2orvkbqkj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2jlrllvai.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2nbyodevr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2zuetqxnp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2qxcdpfup.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2ufkdqerj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2svvjvgek.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2gdrmctgw.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2rxoiojrm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2pcmbjlsa.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xdvslbee.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2niyqiwbw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2aiehhsre.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2fgcujvgk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2zsbibxbb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2crtwlcqw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2btwpxdjd.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2atcgknqq.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2zozjxabc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2lenxkplv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2dkyexbdm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2zxygrgeh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2dovbxkql.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2sgmufoqo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2xzgymfma.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2piqltton.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2igryyesl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2vkuxqtzg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2qxijlkyf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2xgfjhpfg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ohogqkqk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2uveupsmw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2catulmwb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2dpfcjmqv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jhcwfmkh.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2gsstgyzx.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2dyxqdtxx.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2larnzjow.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ivzgxlkb.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2jsbspwxr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2jpuphieg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2matplwrc.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2gqqzjunk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2vrmznxee.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2hjzgpyvg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2qrdbqrqn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2kakuwvrk.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2bfjhukjq.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2rpgmfcoz.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2rifllaov.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2rtlssjor.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2udgfftdz.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2fvdullrn.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2keelzwof.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2ofhakjqe.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2innsgzbl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2khoywdxw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mffdgavx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ptcrqudk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2ebhogtft.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2uzvpmxdb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2wkaivlxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ncdbytqu.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2vkusbyok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2albbbcpg.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2uhgkgvrf.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2cnhcmnen.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2zgbulfsg.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2gjwzifay.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2iqalwciy.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2lrtavgut.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2fajojmwa.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2mckychmo.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2hgohpgcm.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2aqtyijyh.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pdohwpfi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2gqtsuuje.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2rotblpdr.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2wwmbuygo.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2raempgrf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vrefnmyp.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2vtlwogbp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2uuvckoai.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2xdcwnefz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hfnglqzd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2rgkwwceo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2evsdhmdb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2hcdiuguh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2vndncxqr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2epgxweyq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2hjaazjwn.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2japjirtw.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2sgclhekr.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2uestigcs.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2mltmlsqk.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2bzgitqtd.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2amjcemir.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2pbkswlur.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ciwjwcwc.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2zqeorulp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2fqhkwlum.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2pvfwrast.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rgpagfbt.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2wzqxhlft.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dlpisjmp.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gqegswni.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2opkxcxxx.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vqomxgsr.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2dyfwsodm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2fbysklvt.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2nmceqnud.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2avhgvgzd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2hvhnjnak.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2wqrluuxv.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fclqpjzb.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2spncvrrb.html


<!-- 参考信息 -->