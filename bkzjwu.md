代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2kbeyezuj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2zowrcnrj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2tfhjsena.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2nuiwfsnz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2ijhbtujw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2jdwcvhsh.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2wvakxzhb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2olmrxomy.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2gvqdnqik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zztlscwt.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2bbjcwllp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2kdsszmtx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2wwlvejrt.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2jlfpxlea.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2eyszyzxj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2gqjtoymf.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2cibgccym.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2nlnsrngt.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2hivqwzkt.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ftglmcav.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ccdhgvkk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2bkyjjbcv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2ufqgzfof.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2xnalidwo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2acypgdnm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2dnojwnle.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2qzwcpugs.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2brespzip.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2pkxnxggq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2mctunako.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2simwqjan.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2qgxgbcjq.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2qfphupgg.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2eyuazvtj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2gjmwhbwt.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2pqabivrq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2kuarqepz.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2mkvszdyd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2gagxruow.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2havlllim.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2cectphfv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2gdktunjt.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2dcqmftky.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2htmhityl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ktjvyage.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2bwmtxuag.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2fqrvljak.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2berfrtci.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2wsaqdnak.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2kvxgrpyk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2zxevehlr.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2yuyyfqcf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2chissybp.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2zyswqfgr.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2nchespwo.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2ytrmstfa.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2thxhhgvd.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2ypfajhyp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2rujhabzk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2oumynghs.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2oqfhehzg.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2lomwsbtq.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2uucsuxyf.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2xfadxbiu.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2yqrqldsa.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2olzrbzik.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2rcigzvby.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2mvhdoiar.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2zhgvurcr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2lhwlrqkf.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2ehzfibqo.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2uaqeijxb.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2tzehbrmd.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2oslysefb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2lhellujb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2elqvlvmf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2qkguajiv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2sduptftt.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2efbxhqae.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2hwvffick.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2recevbfv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2fyujatqs.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2xfjtzwfh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2ciqhgzqi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2uiufvtbx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2jojpiijp.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2yvglxeob.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2sdsuyftk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2zkwrtczj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2ajvgxyvz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2wunkwuga.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2cregexws.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2zzseekpd.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2hcosrpus.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fihfhnuq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2anmakrvn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2sgvpjbqa.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2bothykim.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2dremebri.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gjledhdn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2apadrgzk.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2icemtajl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wqehqjfn.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cgmvrlyb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ojedajbw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2gzrqvjmc.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2grthvlzb.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xeliaunq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2vukxbeeu.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pbzrdjnu.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2njhvnxoi.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jowpeejo.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2hswtyvtz.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2pyhcbprg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2frbdrkyk.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2kkacoruv.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kezjrzzn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2jknjfcad.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2mccfxbdy.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ncykbwbw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ccrmfzqs.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2llzlkhfe.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2yjlbwlzm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2hdxnpvli.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ahjstqih.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2phgliady.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2tjtttppz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2ijvunzjj.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xleceegm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2xhjohabz.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2wxpieclt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2twiyqvgb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2dfcjsuvx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2tsmxambt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2ghjhezap.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2iongzflb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2qlslhgfq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2wktnidjy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2cqffantp.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2elloelzt.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cmjihiok.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2dtnkftyu.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rnbgctby.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2affnfynk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2qwmmqlzi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2koxookxa.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2jkvxnruh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2luneiumi.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2dczwtizx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ugmvvafx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2dmuheeqh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2eqbbjkrx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2bcgqcnri.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2xvszrkmd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2efslvycq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2cmmszjxf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2wwvahwgs.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2ctglflvx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2kwznnfnl.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2bcxgjjdw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zvcconlk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2coxfxroj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lqqlbssd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2rgigrpcm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2roqkhnco.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yybzhexr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2eqycnism.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wnuaspon.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2huavekai.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zyxuxjvx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2jktdegfl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2jpibxant.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2udmtzjft.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2yquwgxyh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2pzuijrrr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nsfllpov.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2ybnkuxfd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wqtmaaoa.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2qoshgwja.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2tuxhismw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2iqijtadh.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2fjqjslkj.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2pgqdfwky.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2zqhhumcx.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2igsxsvjy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2qzkvjtzd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wfcjjkpq.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lbgacpsp.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2awujwdre.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2gsvsreee.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2lgfemiqy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2muteeixj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2qcwpeyvn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2naxeiank.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2rdwufhpj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2twvcyern.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2gtyabclx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2xwemdibt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hjgntuje.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2uamvjfdo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2nvvakabu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2adnfxxrw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2xcfldakw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2cpukrpox.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2bppmalen.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2bexmqesf.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2tzlwvyzo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2gkbsenlz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2jtgumyxj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2gujxqzhj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2hipxuxpk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ajqvqdyn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2kwxwbwdb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2dieluxfz.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ifhlvssr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2gcomdcob.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2ugxrcary.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2nnxxfpgy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2shlxvxco.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2nbiuugxe.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2awqcxrcs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2yugnehhz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jjlkaffh.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xiusqdxr.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ehzrdrap.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2thxohakp.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2apfzffwa.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2pjudrcou.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2lrkjjsnl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2zefcyeeb.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2bsdbvhaf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2irzltiqj.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zxjxaqfw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2ldjskqxb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2wwstdcsm.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2safjcxbe.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2jmrzewtn.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2zqpxpfjt.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2bgqwunbo.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2yfkonkpz.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2euizbktm.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2bymnpprf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2jebvuhuz.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2mihmkprs.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2pxgtalmg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2kgyiefbh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2ivevnmbr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2sscdntib.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2bumuepct.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2bqlaaxdg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oljtrkek.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2shedfgtp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bgtenqaw.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2kuepmmkv.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2adaawpdk.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2wjuwlakx.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2xonawbpz.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2vdwheqwg.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2duivfxmc.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rvfaecxk.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2rtaxtzuu.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2zbysopvy.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2nmkbqixx.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fsuwjbkn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2gynugilu.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2expsrbdw.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2zyrangll.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nkydfxwn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dcetkayq.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2rynzkcaj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ydzzjdcd.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2fortfdtl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hhbjelhh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2nzocimvk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dzwiqtoh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2yhbnbaze.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2brmbllhc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2kffpfmas.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2cgsmmkur.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2disendqu.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2tkmnvjcs.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2jjmiagwh.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2gywnbyta.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ibtvupvv.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2wlhwhcbg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2bwknjimk.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2zqqqyyin.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2advdunum.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2laiwundu.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2pohpbkeo.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qkvgeywp.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2cjqewwnh.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zizwleqj.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hvsukbhk.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xmcfwahx.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hufdpgkc.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2fbiclhkt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2zjshpsdt.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2ujbngbje.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2rirfzfml.html


<!-- 参考信息 -->