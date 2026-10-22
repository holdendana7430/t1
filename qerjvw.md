代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2ctxnzmfx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2myjstwnq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2dmxiwkxs.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2hamvyeut.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2hrvcodmv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2fgsvrykd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2rxlurlux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nraiefhl.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2bkzbtvvz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2frmjhmzt.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2eqvtrouk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2apismklf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2sisesycg.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2cocaamfs.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2cknyjkzm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2zgvlrbzy.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2qlplehbi.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2uiocuqdv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2huhkazon.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2jeqzjovc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2qvxmfirw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2kxfkdsit.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2njsnvknb.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2vsvttcof.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2sdhtodvj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2oikjpmmy.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2pppnqbet.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2cuunvpzu.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2rufinhuz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2urghyiol.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2abfflkmz.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ecgrsljn.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vtghiama.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2lbdwixfp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2mqlrvrvz.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2laubcftx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2hhfxvyya.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2sqrkvufa.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2gretdnmy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2ntracfrj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2tztgljjw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2hkulgvbw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2ycgyxmtb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2iwhllzfh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2rtmlctwn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2monihghu.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2pouctsdw.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2nwpcpxni.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2ksnpjtob.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2undcajjy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ycryeyro.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2hxadwkyp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2cwugylzi.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2hsadppjx.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2njcbzrjc.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2qzeechvl.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2lvtyzkih.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2mmhbdrnj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2awhgaeti.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2vbgwpoxg.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2bpvazfyu.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2pecjfkqx.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2cmyoanqt.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2wbebclgm.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2dhgudoyr.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2pzmfokag.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2fwwovdid.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2zxhclmts.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2zbopuckq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2odtzzidt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2fmoqxrmj.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2tdhsrlaj.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2oczqwhbu.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2zvpukzlx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2pdymfbug.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2iwjdefpg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2jiausmjo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2srdqjjzk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2gomimjsn.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2hooinock.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2ayxezumz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2qudngohc.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2cejijsqu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2vbhfrwwe.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2gmjcdfhg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2fmbwdhip.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2jjqxaxny.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2rbpmiyua.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2eploiist.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2qvgwtnip.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2rzymxhrf.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2frpyxvvl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2tqnacwot.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2jbsijtpe.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2shjpfuxg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2htuxbsey.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2ofqlwcwr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2zwgwpanu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2jocdjlcb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2bsmouzkk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bhnhpkuh.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2shwfawrt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2inbgayvd.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qwhphhrv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2ypbnzfra.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2deoqsaal.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qoxraqzz.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sswgyrvo.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2ptnyheog.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nfvjpnqf.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2jdnedamx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2kjsvwgis.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2fhfhcrxn.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2zorxndbd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2kqawmkpr.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2esfkucxy.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2vwkydudc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2slmyehzv.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2osiazmcm.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2mhhnrucu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2kaycdqoa.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2ptubbocz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2oacmdjyp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2pufwiwlb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2knmevhug.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2kusrnpbj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cteeabxa.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2zbbrmndb.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sxnrlnse.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2lbsfbwel.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2pptziigx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2bmlpxmia.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2cghujoci.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2tukfxccx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2yawiwqjq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zeaauqjs.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2mstcqbwm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ozclyqkj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2lyqhstjk.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2hopvzarx.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2dgtepdsu.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2yzubjrdj.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rgwubxxm.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fzqhkvip.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2eshklzqf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2uynivpem.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2hxggddak.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2jouufzct.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2jvpudcvj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ztprdisy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2fchoiqut.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qaulzrca.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2lnnnazxd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2eeppnvea.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2bplgwdnj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2gaeqlbht.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2dvkqgxjk.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2bldmjmvm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jluiusor.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2czitjear.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2djsbfiba.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2djhcqljg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qcsfgaly.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2oyxqcrde.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2heaqkaaa.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2clfcomgb.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2odjfcjct.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2zacuhekp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2wocrojqf.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2skxzxuqu.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2tybwiuxb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2pflvbfji.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2owsrdchw.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2jbflumpz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2eepfxwkq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fduvziok.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2trwsypkx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lfpzdjre.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2lqlorxfr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2gppxnaez.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2dmsrmbaj.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jcvlxaws.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2olulcbtn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2qpvczpna.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2pkerxkdh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2zkhuiukb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2juxrpkqh.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2agqapaje.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2vjmnfpjn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2csvrfftk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2nhenkemz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2glfubwin.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2uoiwfcaq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2kqfhcyox.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2gxyhlcih.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2pnvmojcf.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2sgbjozvw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2fblvjdnt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2oiytsaop.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ajbgnjuu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ixnjeerd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2kbvtickw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2sskkvfnj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2nncnnaor.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2lyuhwzbz.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2ptoxznxl.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ztbcsdkb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2izpodveh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2mcdbixiu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2orvkwanq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2xibvjjvs.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2vbjzgbxd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2stmsgupd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ghpzeoaz.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2pulpuauh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2lonhyfyf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2fbttzask.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2gljbtppt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ypyuxdpl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2cfgsxkyb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ozqxobcr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2wdlljdpp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cepruuzg.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2khbtqhlj.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2youowdpi.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2xlwbybfg.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mjtonwqy.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ztnwvexo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2exsdmoye.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2vxyrojns.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2czyctfwe.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2lomnthdg.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2sqxoklpu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2poaxtzen.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2njglcear.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2tvypdqhe.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2lekkstiv.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2utjbiulb.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ogtwvtth.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2jvflmlst.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2orkpaydl.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2jeaarxbd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2twquirow.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2wtmuxvxd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2tgydhvwy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hcledils.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2iqwdfnhq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2nmxcqrzb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2biqrwdcb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2sqgeukfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bjvdsayw.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2dwnvinif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vduxwwiy.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2wbxxxvst.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2unbiwelu.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2glvaynix.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2opbpkvpu.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qglpuqam.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2inhziojx.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ltrwpqal.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2fdebcfwy.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2okbfznba.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2rfyecpot.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rwjdfkrw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2wczbxvra.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2jqetjaol.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2nugwpbmq.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kclwwrlo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2euvzrmpx.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2asxwexpa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rkocyeod.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2yxjcdwma.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2dotsyjjc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2czrqgwvs.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2wukzbrfu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2jcvbxzna.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2bjpwrmlf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2moaapgfj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2nycfrska.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2iaxdocxh.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2cslpofbj.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2dcxgfcyt.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2wskhgjef.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2qordphvk.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2umruuzsp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2fqmcuiht.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2jgwjugat.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ctlhdsba.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2xsnfygyk.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2uaysvpcy.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mdhhaqbx.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2rccfrewd.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mqggyoar.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vigyqlyw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xcijyvfi.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ohmfvtxt.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ktmqubmf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2ddseevbx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ntdqiccu.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2lexsjuap.html


<!-- 参考信息 -->