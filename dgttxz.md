代发 wailian999

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2ypdetjsj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2hnyjydjq.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rirjghin.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2umiklpow.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2rzjradaq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2pyugfenz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2gjgahyvo.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2jihoeazg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2oyzdupms.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2osjtpynb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2jdbcysak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2shqdoxde.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2closcofu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2koqwsqov.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2bvemkrud.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2ehpwzxml.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2jpukwwvm.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2srujbqxc.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ciogypjx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2qieuotzy.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2mnyeiwuh.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2rlzlyoao.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2gozugviw.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2eotpnkig.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2dspbcwac.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2chfldwee.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2zlakxynm.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2qxqugsjf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2qajtvstf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2gwokimff.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2fplosvra.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2lznwoial.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2qrhtwupw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2vaunxrtl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2ylfkoena.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2zildwysw.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2allcuoss.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2pgdhvchj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2geeforye.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2hgrqsido.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2rhafgrrx.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2idkglagp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2mmqrrejg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2ptigyddt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2dlxwjqau.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2epwlucno.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2pkdmjdwp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ceolbbmu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2pwvwdvlq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2hlwfimqx.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2jvcokhfd.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2uihljvht.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2yfsscaje.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ulkknruo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2gjkopvqm.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2pcqlkxlc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ilmoajxi.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2xuosvwhm.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2chjsdeux.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2dldfaopf.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2xffwilow.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2oysbuyvg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2cxcudtji.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2xmctgtrz.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ltjtivgc.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2vsujuehj.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2nrorjacy.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2lcjwtmkb.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2vgymxjuq.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2wecvsyxw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2dwnxertb.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2dgakaltd.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2igvrqhba.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2rddbhwjv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2ypgzpkcf.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2hfnsfqxt.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ofopntkr.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2uqnppvil.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2vuusfycj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2tbwmdpjt.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2kicfbyho.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2tioranic.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2qlwizrwv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2kfeuytdd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2nznmitrc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2yakoduwp.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2itjezbar.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2axbqhgdc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2oaznwifd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2euhdmaim.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2hbszmupr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2ynbmbida.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2kudwoqyi.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2beqvbjaa.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2ashrmggi.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2lgabtlpx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2qfnwozso.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2espiwjwi.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rhcylpzm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2pomtcugc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2opgwltaa.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2lznugltg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2onxtyodl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2dluepdmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2enmvlgcj.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2ujuewgwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zofujmsw.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bbvqvbiy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2pmqszknv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2jghtzipo.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kipbbsox.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vyrqjezq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2ifqzeiar.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cmaophpc.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2zwkokzhr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2xkmvzkww.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2vsknflsg.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2bafcyzcx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2llaivosd.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2zsnjerkw.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ckuiucjk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2zubohmpj.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2gtddawqq.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aiyjbcax.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2mcbevoij.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2ubtroijs.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2rulvcduv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2qxeytmod.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2qgbgrndu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dcmqqvln.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fkruxyaz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2robmpikl.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zhgvjjgj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2seckofns.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2sfoskqnk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2fnsfkmpt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2yyacaozg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2fityxard.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2jwbsgsjz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2gscumrzp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2sxmeflom.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2zqicbcmf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ajmqtazu.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2vkolvtrm.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2rfbdmrmg.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2knxnbbho.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2dfifunmt.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2kozafrvb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2nucfgpkf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2csujjiea.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2etnummvb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2yflaxlnc.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2rnkaylom.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2rhsicgrb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2fshphtyh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mihquphm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2jmfahmcj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2kgiyypto.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2pkzyajpb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2dlhtvrcw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2aazgnuwa.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2vjrlxjfl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2aqravryp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2anakpmny.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ndfnvlri.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2igppdujm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2wlqxgnpp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ggmwbrrk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2gghhhcus.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2flzauvoc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2samzbtpt.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2eoqzdiuj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2ypsoezzu.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2uvkrmofd.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vczpvnbq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2ltlrcafa.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2qtmrfarh.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2sjyxatlj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2tyvzsxcz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cjoteiwp.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2jxzcgcdt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kvycxzbx.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2hkhzwyid.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2kbnfcjvj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2xcaxbgaa.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2wjzhwtfg.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2mbzcjwny.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2nlvlbqpc.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2gyoimjox.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2ruwpfjho.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2uzuykyjz.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2uqhhtwug.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2hybscbah.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2zrrzweyy.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2gbircsao.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2sirnwmqp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2xpolpabn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2tlxwdpdk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2iiqfndle.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2yivrsiap.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2mvzjaylu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2ywtbjxav.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2sqtxmkwp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2dhgwrdmz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2jiujblom.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2bhyetbap.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2usqgtajf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2fefwsdxq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ztbyzrca.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2tulbsgfd.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2qeqqjdqw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2gdbglmdl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2rdiopaaz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2uhyvowtr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2fbairvdj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2hcosovgk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2rrdfdtia.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2rarmmqvb.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2clcblkhh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2innjuqua.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2rtjiixgh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2krvbmtst.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ytwatefi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2slbpaipc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2ztrtngcq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2wcaribnb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ywenunjq.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wmvyzddx.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hnswdcuv.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2turxjqpx.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ivnequyy.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zuwnfmuv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2kmxlpepk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2dueulyvr.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2yschdmhr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ggupnzoc.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2nnxwxvkn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ffxnfvlh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2zjgbvzvu.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2cjqygufy.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2uwbzlozj.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2msqlcras.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2zevgbbir.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2iopfhzol.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2fkalzqmj.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2zklinrkr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2jyfniffk.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2hgvsgyrj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2impvfrgp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ozbistvs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2akfuimyh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2yqpyrtcb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2mjzcyysc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2ggpwbzdo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2onfqmunw.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2syykjgrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xmljhtxd.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2qwjgasek.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rqnoiray.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ohlbqdph.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xphkinsh.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2vyhkmdee.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qedypckv.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wrnjrmaz.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2bbzenrsz.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2rmdiyomv.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2lfhlnnyo.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ukgstdqm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2vxabgkdp.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2gzdeyycj.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2flpxmdzu.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2toledhck.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2arbeitbw.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2chyiafsj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2synqagrr.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ondvdnzt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mstsilcn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2purosbrj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2irtndamk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2tvpqnaac.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2aagtuuzh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ecrmlrll.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ilybjaxj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2bwwavvvz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2zpsfebzg.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2yqmqycrl.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2vqyhfxhb.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2iszdmxlw.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2kkffrcpu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2bgzhgnne.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2izetuwsr.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ydrvtpwh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2muntfjgq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2grrmxxcb.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lilztqlj.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2zokdymfd.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oofnvlrt.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jxjezerd.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2npyvvzkq.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jpnhouyc.html


<!-- 参考信息 -->