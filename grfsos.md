代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3niwzllrm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3irugqmbz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3ugxhhovg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3vizfgdpm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3bxwznryb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3bxlotybt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3umtogsuf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oppunmod.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3ogimhnuq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qnqxfvyu.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3tosjwykv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3lvugbryi.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3fuackaby.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3wdmzlkwa.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3lrziypjt.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3xvuvixgm.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3okdhksdd.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3tbnnlgul.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3txvhjscb.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3smiagvbw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3fgnztpvc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3snwdrnmx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3bjotdclh.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3cdhhodem.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3udyspdnr.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3ebyuulta.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3dsjzpfle.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3tzmvvbme.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3ugilbyfg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3ywdazupn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3quhuuklr.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3wtbuwvyu.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3itebvlhw.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3bchmtskz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vvccxoow.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3tbmfxxba.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3egiexyye.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3dbkrqaak.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3hyzgodib.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3axsizelg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3jneztphd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3chswpfop.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3vsoyvtzb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3avpjbjcl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3asnyazok.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3wkylodcq.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3yebsgsgx.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3ywgghjvz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3alxovdlv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3afchvgak.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3wiuubnlq.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3bhdnakzd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3fyfqxqrp.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3zvsnudod.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3jcpkaszn.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3cafnwlhu.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3qvblfsfe.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3plwsewta.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3zrhgcdcz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3ixosmawr.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3iajrbrza.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3skpwhavc.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3ubapbfum.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3xmdkifoz.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3nigtnbzp.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3wfwpskng.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3dbkvmxrb.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3lfdeukwx.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3wihimyzt.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3sxhxurmo.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3tbreicrv.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3iusxxwnu.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3licyqckw.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3bzebzilb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3slatraue.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3eqyncvun.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3nwccngmm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3whxzqhff.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3uxvbfits.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3bzuqqahi.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3xmddyasz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3zyfteczl.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3mstgtsqv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3uvkyqsgl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3uldqtmbw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3dihzzvxz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3hnrbwqyr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3tnecpfxc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3aniohgow.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3lfseaucg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3hlobmfnl.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3heqybslq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3dxhrbttj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3ggmbikcs.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3otqhvqkq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ihcdiqzc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sgjsdwmf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3vejpnzds.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3pktujcoj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3atcmrvgv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3alpfglry.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3fcvbbugw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3irjgffsd.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3rfepkgyn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3llwpqsui.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3uflbgdrx.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fviemksx.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ohnkqjxv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3gamcqlmo.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lydbkqgw.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3rncfnppy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3glpjfapu.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3rjqcvcqm.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vxoiacsb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3futlnmav.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3osvvhlyd.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vifeheyb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3euzrljdb.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3zgsofodi.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tityvjhk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3uubaylnj.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3vetrsavx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3bhbcqmji.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3mjokbrvn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jivzfxin.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3igbwmqgs.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3eqffzguo.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3ncikxium.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3qmmpdvcu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3mobnjkig.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3mgixhvlq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3ivymyvoq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3kofdrnev.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3wrfhdjga.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3qxffgygs.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ezsglivf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3dxwlvtox.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3srozvoav.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3wnkjzjmw.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3xsqlcxky.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lmwzlnzq.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3fjjehhfx.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ynpkikxw.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ieunaqny.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ngxhjzfs.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3phpljods.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3cpfiykrz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3cnfpddbm.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3ywzmofsb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3foxswkmd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3xfvwwcgf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3xzfkycch.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ycnzccnu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3uxvysjyf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3zncnbbbq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3gpiwfmcj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3qtuyhleb.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3zxpnlayf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ymcmnlda.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3qlhkqxml.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3hnsensmf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lnrkzwsq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gwxbyyas.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ghspqmzj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3efgajuhp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3sfzgjpgs.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3yeqmfiks.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3olpbkzub.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tbzxfgdk.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3zrcmxvps.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ultgptaq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3ehcgltmn.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3qaklnbqu.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3mlapbxzy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3usfhiihv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qclrgeot.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3mgirlodt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3muypfffu.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3llfskgkx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3nkrdqqqb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3mwpyfwpz.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3efferver.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3pczzqlnm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3hadpqbkm.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3ewzzfwxg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3uokaiehe.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3mrglpuei.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rhohgsil.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3nzqbtcny.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3dynavqmz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3onpitlvk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3zdqgpfsd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3lhstffly.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3gkzdxclq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3qczhwcfr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3kpkhrgvm.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3lmqqlmpz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3zmqqmccd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kamsiiuq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3sbhicfku.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3raarzugx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3kbbtlaht.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ojbhrqqy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3ptkvpklu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3lmanfrng.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3wcdoneae.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3cgguopjt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3yfyggqrn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3aktkhodu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3szrsyhzv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ycowpnsw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3gonlgrwn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3qndpikcu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3tfhcfsnj.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3wecmscrc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3kzpgkjmj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3hmouxjjg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3swngdbhu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3yteuhrmi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3pcptzihe.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3kqkcyqpw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3lfadyqes.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3evewptgm.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fmkvvanz.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3epzvubkb.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ddjcjvwo.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3fxcutowr.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3urjckqpl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3crnidveg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3mqutznnt.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3devwsuab.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3wxefpkaj.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3dvldyczh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3rmnhlctn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3gyhfndcn.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3cluespmz.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3fzzosver.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ntvfmamm.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3prpjoloz.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3snqpknrv.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3psfdnawx.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3ytxuirhp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3fnexydai.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3ljcyccij.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3napnbajs.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3trrbutvr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3qxebwvie.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3wubtduol.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3royfgbwa.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3kcigorwz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cmjvpffv.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3abhbvvps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zeznolkz.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3rrlslfgh.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3wlbzmesz.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3cbtnozia.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ltycpmjf.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3suuucyil.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3behpmakh.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3vcvlsont.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3opylceks.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3gtrqpwvd.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3uikpxmzw.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3akuhvlwu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3opdyowce.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3aihifhcs.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ryqqvsgs.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3uavimqse.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cjgtqlmm.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3keihkbes.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dcjonkwe.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3mcklltou.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3asvpecip.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3waafcior.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bhmbgqaa.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zadoxxeh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3fxolfppe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3zchthzzq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3cuniigde.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3manuajbq.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3ioeduecs.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3yimhsvjs.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3uscmbtoo.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3sxxvchms.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ycffdjhp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3tiparcbx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3buishwaq.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3vjyazech.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3gklljevz.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3cywgjnoc.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qcnjmpzl.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3vozwaqeg.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ddlzybzn.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3artikqov.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gypnnhkw.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3oqsablyl.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ylyqhixn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3kliladib.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3rtdwonfp.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3sdzlqwja.html


<!-- 参考信息 -->