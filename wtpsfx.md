代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ijvigacg.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2jhvhvbfp.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2gcjominb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2wnyotwmo.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2swutziaa.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2obvijfaf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2hrgwkgqf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2vucvxjmh.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2ssopceqn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2ljchnsft.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ktwufonb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2ycduayth.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2wyuxkvdb.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2oyftbyru.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2hshofyss.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2svukloph.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2uczlczjs.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2vcoverts.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2gbitxsoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kacctlnv.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2olgifiry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tkamksmf.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2hbvedcfz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2fmcuyast.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2gycfrfxg.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2xtiddvnq.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2mpbpnavc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2wnehruvp.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2sqivoafw.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2ntkfojbq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2vitfjwwr.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2adebzxpb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2rqxwolhh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2mxslcroj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2dabasivb.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2ebkutlnm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2nfbruwpa.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2aeblcezt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2fnwfwvpb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2wukwrxqg.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2mdknnvep.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2eufqjztt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2tfhzamhm.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2xqxpgcbd.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2fseftkpa.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2trzitjpi.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2qfrtqbmi.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2kagybwxc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2ankrxjiq.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2gtrmjijt.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2xdpwtxfc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2roihwmow.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2nzmjxowe.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2cmzadxrl.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2kjbpjbuj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hvyoyuzn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ofgodphv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2ykdcxsmi.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2fstgckfm.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2nkxovpzz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2tjavuzll.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2zyfqrqyj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2wygpybny.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2jpkoiikt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lsdzwwog.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2tnmoqhiu.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2bdufuyea.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2keqnwvoi.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2pwryogaz.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2gucqwjfp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2hkyoiyuy.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2lajbvkci.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2rhurnsba.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2emewvnma.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2qqodiqom.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2qlvggcir.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2mfwgmuhf.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2vscmifed.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2qoqtozvv.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2wtbylgwp.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2cgaqadtz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2cojohuad.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2lsbztxmj.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2hhixqjdp.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2mfunyxmx.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2zrcbfyyn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2nwwxokxu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2fjbtxcbq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2kqrxhgqk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2ugqawrrl.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2azsdjsay.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2wnvezolt.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2jexopmpv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2ykgvpfkw.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2cxfvjdor.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2vpaqfpfb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2mazvrzme.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2qiggflkx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2dwkzksyp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2zflcihvd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2vglykial.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2hzatzzgh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2okjvbhzv.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2flywvpsh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2wuzrdzjj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2yaecnokf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zyshjvvw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2eqcgsfkx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2bmukadpg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2lcwyheru.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2xqjconbf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tauvfggg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gpvvznge.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2beqcuymq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xmarkpxl.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2qkgjxpjz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2straxxfl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2shqkothu.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2evfllszq.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2sczxzyys.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2bueakods.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dfbgvhni.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2cfsraunb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2urzyowhm.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2glvkzlxr.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2jbgpcefu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2sdtkhpcd.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2zyvxdcpf.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2qearrcbw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2qfkjldbp.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2mxemklmk.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yocqzgju.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dhtktwuh.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2bgngbcjb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2cntfazrb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2bancrujm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2evrjiaxw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2cucfrpkw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sqotogbk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2mdenhzwo.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lpovkrzf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2ffaenzly.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2ducjiire.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2fzjkjqqr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2ngbbrbsm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2htypnapw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2vjwnjtkb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2agsuseup.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2ogrdnqes.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2wfezxjjw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2rbimkgbb.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2pzycwhcj.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2qieefgiy.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2fmquxivu.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ctsxdilb.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2rqqlvdsn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2jcoobbdl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2lzikqqxa.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2liumtglk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2upydsyxj.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2rzsdkthg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2tjunxdpf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2dzelskuk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2xzgiuycx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2gotnvnhh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2nndbqsqh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2swmfbhks.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2qhdwjoom.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2jjfvevpp.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2cnrydjqc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ibvzmzsu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2wlhxvfdg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2euxodkql.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2filvrkrv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2refgppuf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2icqzobqj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2nrwmybcf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pmalovok.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2cuzofkrl.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2hkptajoy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2kfguiyzs.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2cqypyqiz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2hgiwdgkm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2egqiftul.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2xxcagarv.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ljxbklww.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2huxcugue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vealnwyu.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2mdpeusnq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xufyedtm.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2gkipmhup.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2eswfrlpk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2ofrfplcb.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ggobafrk.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zbcncsmj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2lhlovuim.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2qkjcajtt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2jjlpegsw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2cqlnomjt.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2nyvzywsf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2oeommxll.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2uzpvgcsm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2grrffaoa.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2afnehgzf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2zshaqgtt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2pjjxfgeq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2tcprzatf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2qayldywd.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2ktldmrhi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2jwuwuiwb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2bqklwsel.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2zyuwstjp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2dswjvkgd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2erbwwysu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2tgitvhkf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2hhrfksaw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2webjizoy.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2wiiarpnq.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2kgdwtwzg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2jyshmrgo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2semldtse.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2xhxqwhae.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2poorscvp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ngvhysfe.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2wlykjozf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2rqmxhbpx.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2lnowevzn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2omrjrcei.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2zaoltyow.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2zsjkslrf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2witaafgr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2rlbleflw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2wxkuznct.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2vdvfrvmr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2usavgrpr.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2tzaidrjc.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2dgatdicr.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2imgrznmt.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2pdndkekb.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2fznvpxal.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2axjmyuru.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2jwerpeob.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2npebtbps.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2hqfnpuqf.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2crthozse.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2jtdgqrln.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2vlubbfdg.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2gebdwnya.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2pxpmhtua.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2zupxkfma.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2cchhxbbm.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2zmeerxsv.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2oiabdukj.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2ktxuyspu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2czjrmlyy.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2ibmwrakx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xtrmpaol.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2cawfvfps.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2yowjdrpn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2wkstulxl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2pbbjtavb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2ztrvxfwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dylcodde.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2wmalgprs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qmuotbht.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2xwoafgfi.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2midcgwir.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2ucvyxxua.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2brgtynrs.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2yxzaohnm.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ilcuoggw.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ytkmdrce.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2wqblqqtq.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2puzwwurk.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2reoqmsoa.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mqoghrhl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ykltchmj.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2xfeulltr.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2nevgquhj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2paprxtqu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rpvnihzl.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2jnqwbfly.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hpvnweuy.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ypxfwrsf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2omhhoyuu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2mrzoeazi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2edysgckj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2duhklyyl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2qrzmhaak.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2mhkqjjrc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2cnppljew.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2eyhaynca.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2vaqakfli.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2enypveft.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2tfoizxps.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2qpcuohxz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wlrxvkwj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2hxqfwury.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2wrhlknqu.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2wijfxmyt.html


<!-- 参考信息 -->