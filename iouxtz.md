代发 wailian999

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3ivkwqhjs.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3zngidzck.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3eyvakknw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3ilihflgy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3nnvspskh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3iubpbruk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3hopqoyte.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3meinyeyf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3hvpugfdl.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3yajpzdxf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3wkzroker.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mnnspbkt.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3fwhhnlxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kuvkgbiz.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3teroustu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3abpaurky.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3oaggdegu.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3yrkmhrgy.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3grnnnghw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3aavzflts.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3jrkkfkrr.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3hxynmkeq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3rybxpuqc.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ljxujkkr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3cnpzgcfq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3qmxrqwrd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3nqrnqwtk.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3ugmukelg.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3wwbtrdmc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3ttnycszn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3ihozbvzd.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3xwgzvuus.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3jznmsuxb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3adqwkmgd.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3ihiyfani.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3mycvzjsc.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3mlbfjaot.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3rxncyaku.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3csmdeoxo.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3uanlzazt.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3xpzyenrn.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3onbrxuwp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3masisedn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3ipmkavvl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3updguuwp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3ypxylqyy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3jbvixpks.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3aqjowwou.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ojucpttm.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3nolybtdo.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3mgjdilin.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3hbfqdvco.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3nvvhvqkq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3aenmthuw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3grwnlryq.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3xbmujhwq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cnxgokxu.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3ioaxtcke.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3wjrzrhfs.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3xfdjsthk.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3smimqqdx.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3dnavqaub.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3inghband.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3thonvfit.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3hzdlonws.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3prghgxnd.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3yluouwkv.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3royefuvh.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3hyenwect.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3tizopaer.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3kbizfsvh.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3itisocfq.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3khrpxkva.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3pppipasn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3jqjhygpi.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3gnnfjhzj.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3nhcsjafl.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3pnosanbt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3gmtavuww.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3rpijmovl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3tuqixvhz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3wvsiuffx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3koiyysbi.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3leekzsdp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3xhjbnaqi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3zqcigjvb.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3fdwvajtv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3lzrxqlvy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3oeopjurw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3uqozbwnz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3hxzvieav.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3jcgvookg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3ueqbgdob.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3ngqkelul.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3nvutkicu.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3qseciekt.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3pxclimko.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3xjhvsfqu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3xclowxsl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qlhuhele.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3heapvzee.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3vpobkxqi.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3adppumhq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hjadfrrz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yxdvbmfz.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3qvddwpxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ntfnsbdw.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pzpgsymk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3wrcrenxh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3vdxdgkeh.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3opyhwmzi.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3bqyxkazy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3sohzyenm.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3rcbumgsq.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3luhrgxpb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3oxtlzopg.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3vhacdich.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tunsobvq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3fkauwoyp.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kghginrk.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pzrgtiui.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3hvbqyqsj.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3osjiasbk.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qzkhevsi.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3ascqirjg.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3lzbtemcs.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3ikzrntie.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3gyenmjcb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3dizxpuyd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3gtnmznnp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3ynxpmzpj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3nqidpmoa.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kmbcyngn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3vczjcsau.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3tjgfulov.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3ovnuxqqj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3dadidhwq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3xgzgbsfd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3pojqsrwc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3hegrupyn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3stntmtbl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3sbtsphib.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3teoxmspl.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3gqhmobii.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pzdopdcg.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3ipzswctk.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3psnhzflr.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ybzzuuzn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3wwugavpa.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3fzjbrckr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3wmsnrdxg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3oxfckech.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3rkacuklm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3exvyhtbo.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3czbdmcom.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3shaccmtc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kayxndli.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3cubjuzur.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3clpqxsdp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3qdpagcrd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3nocsbdnr.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3dpvdndtl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3chxopcyu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3gjvbxmdr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cumeqrsx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fgtapfcu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qltnavhw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3aewontgf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3prjrofbh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qqzsobnq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3izlarepw.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3gpsoayxy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hszsbqbz.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3fjlwidwg.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ujullpvh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3gaceuzkd.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3bslbnbul.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lneexjie.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3zwnfplsb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3divxqxqx.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3zwrmrthz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nvdfpxad.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3ekhmbmtm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3wowfrlfj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3blmrhbdz.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3hqfhndsy.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3mgszwbbg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3kbmtccbf.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3oyxbktew.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3eosfbvug.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3zogivqit.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3njismfgd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3dxkonokv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3cdcmxexe.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3igeaimyg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3oywhyaij.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3kwmvclod.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3xvliwlqb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3edyzttmc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3mqqggdxn.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3fpxxuwoh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3ghvtiefy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3iookvjpc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3wbtqhbsk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3nppxgcad.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3llvcnjch.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3gxpftoad.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3qrxnwgop.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3cdzeajul.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3kapokasu.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3obrqkeia.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3abkzbdxo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3njxjmpjl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3oscwlroh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3lcnwxjme.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3iaagfdyp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3itdmqaat.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3ihvjphhj.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3wautigxi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3ljcaufcf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3rvkaaknu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3vkddaihl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3azrzzexm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3qgozlxoz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3tdupisnk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3bbfzxctl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vanaeyoc.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3mghbkvyv.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3uafixjll.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3fqcsuzie.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xkfbuwax.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3fttlahmf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3fsheugfg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3htelnpti.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3puievuvf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3aoifeyul.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3dtqizhdp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3xucdmgmw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3drmuthmm.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3bknavdxx.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3pbjuhgne.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3krzhaijj.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3nemgzptv.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3vxmiofwo.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3oncdfhhs.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3fvglyvqz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3ohurtbrz.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3lnbnsxut.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3wmlaygei.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3narbemxf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3iidmqwus.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3pvzbmgos.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3muxsolzf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3eyooqlhz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xussymif.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3jucnbmqs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yhsplhmr.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3onncobjp.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gmuawqfo.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3owxiofbn.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3cjrwvcrv.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3junavjpy.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3djggagby.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3isctbdhd.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ixfzflmv.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3oypbjpsh.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xocianuc.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ehdsfxrj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3cjjkmswz.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3fhahxsdk.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3pdfutyej.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tzfhimlp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wkudkyvo.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3rxurdddi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gbawxmtc.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3kjmrjcbd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3hseexvux.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3qgtgzbai.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ctxsttqb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3aifuoivo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3bdaegpts.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3nxtqkvqr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3mshmqbds.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3tbzwjjwp.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3tejubgry.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3sjjsvieg.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3cfkxbemk.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ihgxqoqc.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xoycvvij.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3jputlmrz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3kkipcoqn.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3yuqsabwu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3cepktwyx.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3zumldkcw.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mkvzmnvq.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3zpmsofrq.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zebuzaty.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3coyxuekq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vhismqrq.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wluyjnhl.html


<!-- 参考信息 -->