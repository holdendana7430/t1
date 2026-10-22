代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2evwdsoio.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2ncqeduur.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2iqoodbuj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2bzcynncw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2zlsxivcs.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2gcnykfxv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2ezujsnkf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2gdfupzhp.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2tvkotqct.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2chixwpir.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pkgnxnxt.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2fdgrrhur.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2sobqziys.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2gqujhafe.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2ripkeede.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2rxbmeqcj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2yusoscyd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2ggnsepbc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2qhirrlli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uilqdpzl.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2elxtagxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jtxztjss.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2dqkznjza.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2qhtkhgra.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2cjtedakx.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2gedydzwy.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ifwyuyae.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2pvetejpi.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2embtgvlm.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2rlxatnrb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2gjrsuiwn.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2qzwujjft.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2jylusjdw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2nmoyogps.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2qlfcodkl.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2hqjmapok.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2uigwxkrn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2etkettji.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2sogfiaxm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2vviheash.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2khqeaqvg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2wbxaxwsh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2eposzdwl.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2yhhwnytg.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ruylbioz.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2grtuglgc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2kmpoawrt.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hnhmvzjc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2iubggzue.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2oapcvfxr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2gntqpkmq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2mqroyxnp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2oqetlfyl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2qfpoizib.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2hshomfha.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2twaxpeik.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2miwhedaw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2cplosvxn.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2fluizqre.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2yjdnmxhy.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2usvojbul.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2kztzbrny.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2eavazoev.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2wllrtfba.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2ktidrahw.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2jswkdjco.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2aqiwskdt.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2xhmkxkvl.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2jirnnuvu.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2itcgnsiu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2mrsmmmbm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2soergejn.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2pynroyuo.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2hfcemese.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2luiybmmf.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2gekptxnh.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2jdcpvtmo.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2wepcubxs.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2oumjuiki.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2ysxflcvx.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2vlpetlln.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2kmiigexf.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2oojbwbfj.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2gtsvrkzs.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2cnyveedt.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2anaoprvm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2htxmykvm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2gxeqmilg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2knhvxmkt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2huwgizpo.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2fsweuwqe.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2yacjzypg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2wykbfcts.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2yunsxuwq.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2ubsyqwoq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2wrkkemok.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2qlcotema.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2mkylssmr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2xypqilao.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2frfotaya.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2cphuvebt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2gidnhajm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2zmqvazla.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2paxqdhny.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2ijazgfgm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2mwlplxqc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2tbrbxohn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kmykqxgr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bmigjtjx.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2ktidlihj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2minmggav.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tjsmslht.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sqptzpie.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2dljfyzrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pvmxgqkp.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2etrxwvdl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ameltcvf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2xohvbtcc.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zeuyxmhm.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xwycucfj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2hmfnhvrb.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2vslflhuz.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2xltqwrpz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2boeuzexn.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2zoqndcui.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2slnfclxa.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2vfkhugmc.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2cihowmbw.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2rxeyogqi.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2rznumqfz.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2rsyhkegp.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bzrdehuv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2yicgivyf.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2ijakdrdl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2lilddotm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2orlcutnx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mqghmlpd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2zpcbfjkg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cynoudby.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2sogpsvyz.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vsgrkiok.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2tabsmsmv.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2iapyeqkm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2edcfyuio.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2mmsojzvp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2vylpsxvw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2qtvhilky.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2vjeyfbld.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2nmujhwsd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2viuxtvey.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2oxtjgmlm.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2rsvpazwk.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2utzpcwih.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2uhnynrtx.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wltmqkcc.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2xftiycfi.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2loslxoyx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2mihsjjbb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ibooladh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2bkrvkenv.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2blpqucqj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2kcqcrfba.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2euctdbay.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ubheouuz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ajmzlgfr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2prrzlvno.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2twppxobf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2rliuewlo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2shzitrjv.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2obdplzuy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ilygdrgn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2tyycpkgr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ozgbeefe.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gnwtxpss.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2extdcxth.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2zcbrwowo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2xwtxxsqa.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ueqvwfsw.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2rwaaxywg.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2kdrmdgib.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2qfjdvqrq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2wyhklbhz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2yfwpykmc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2vpvdvxvz.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2nraofiwe.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bjrqlziz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2jlpghabw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2owcaogrx.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2dkvkowim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vllvixin.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2hxrruafd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2ducfhzuv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2npnnubwe.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tpeibrrc.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2dvjvdwtm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2ixgtqrct.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2nudrcnnx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2ngdseacl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2rhmmbihc.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fzlzvfzk.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2dgrekoaw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2vlmnxrxc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2zlzisuaw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2nxiawsgf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ziwlhams.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2wltxriis.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2nbymojak.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ujoxoqhb.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2exnmmbba.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2ckmbfyay.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gfrwpyos.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ufxfcfwv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2enomvmfv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ywzxlnqo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2rzwvcnwi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2dsrbwlbk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2abmlyfby.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2tngjncrl.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2xypuwwrl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2mczoopws.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2wyblntcp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2xlykwfmj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2hnlkhmpn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2phgogjci.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2vvqfwreu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2fopjhnao.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2yuevbayv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2mvpagehy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2wcaledaw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ltzewogd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2zoysdlkt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2qngfvihp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2trqgpmob.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2lazjjgvd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wjnzefbz.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2dfegccet.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2unmmfagf.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2yhuzdusw.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2xzskapat.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2wethkcus.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2dpclecfu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2kbvuczox.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2yuclrvlh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2xwidoiuw.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2eskvviiu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2kebtaphm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2uogzepsm.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2xkyehcmu.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ccunxjhi.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2hnrbmmwg.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2hgehqllj.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2zzwqarad.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2dtzmqgjg.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2mzlzzwmx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2exculhrk.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2izimvidt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2pnioycnj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2poaofcuv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2wmryulrr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2gmwufjjm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2lwgdqgln.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2kkrqqrcz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2inovlpch.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2xsnhhdbb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2prditufs.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2hleqnsza.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vjvzrney.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2qqiuctzc.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2xvtnblzk.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ggkmvozr.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2yhzgpkmy.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2oxieotlj.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2ojmliwvv.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ddaksggt.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2vowyszjh.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2sigfrbqh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2bkejsayq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2uflkmgsg.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2xufkpivr.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lkyzbtur.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yylptvyo.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2hlcixijz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2uhnahtwc.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2tlnyygxg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lsxhvfap.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2dwyygjmb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pbecakcq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qjvgyavx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2sgjskzui.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2tlwgthfp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2xtwhicma.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2ugajznro.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2mdohqvox.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2wisejpcf.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2yyspyfzj.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vsenfvqg.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fawmadde.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2chfeavlf.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2qdlwhmjq.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2eqpnxitb.html


<!-- 参考信息 -->