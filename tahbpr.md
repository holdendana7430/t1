代发 wailian999

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3xanxwvnj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3abboptdn.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3yfnpgost.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3ysjxkudh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3zbizupgt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3nbjxwmcl.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3bolcsyuz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3bnvxodnb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3hhfwdtbm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3adgemqzu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3yvrrgrac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tamvyimf.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3jpemmtqa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nmvyjvth.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3wdfqtzox.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3xdclvwqr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3rekeaukn.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3pdjgxhmk.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3bjvfanrz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3qhgkrikh.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3wzskgbaa.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3aogvvbjn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3gczebcnu.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3qgwrqkum.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3rrnymlhv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3zrcjhvtn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3zfegmcxa.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3lonzdqtp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3czinqlla.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3pndmzlbm.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3steshcam.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3qaoshjze.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3mlpicxhf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3nelzuevn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3drivqsnm.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3vkiwgynf.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3vwzeyqoi.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ffaktrxw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3vxecxlji.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3yhcnrqrx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3oklbtaiz.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3scxixckc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3ullbqfwq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3pahfbvpj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3lpcdikns.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3qkzibhaf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3iuofbesn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rtodorxy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3hddmqqsv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3npzlktks.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3jfzmksty.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3pbryouov.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3azeuoxgd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3ghadgtbc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ojxyixis.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3dslvwjbm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3owmvhzqa.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3qxslyxfb.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3nbhifimr.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3xbvhjjlo.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3svawehzf.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3pzwjrcpd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3igcmmeuv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3rstqlftl.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3kvxtjliv.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3qesdevpz.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3echglbqk.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3xyuyuzug.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3ryrlhxga.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ujokelry.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3lmzfwmoo.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3znoomjfa.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3ezglqfyx.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3mzwbubdr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3fczaaoky.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3vpkppnfq.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3yarnkmep.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3ymrtwlyg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3ccyukcpb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3mncnfjxu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3xfffjlrb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3ckrfyghj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3mwarfiqu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3yuacrvqj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3vdncmtri.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3vesrzive.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3ipvavcms.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3akcbiras.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3tnwlrjjs.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ngzhilzt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ffelikyq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3zaoxqbyk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3mgdqttqm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3lysfkhsg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3adazoxgp.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3lkdmktoy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3illifcin.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3najzfhsv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3gquozqut.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dfpjlwpq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3consnpff.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3vxvggtbm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3ebcgfaoe.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rovcsoli.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3infqsixx.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3jbwbvdvh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bphrlzpw.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lyopyavq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3lgqsefkw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3khfvzrof.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hswnlclx.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3vynijdhr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3twqrclpu.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pvyfrwpe.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3qzdmabvj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mywjpdty.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3atazlpji.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3wutmaoiq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3vkqoofyf.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dbwstofr.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ojbczqnh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3oadaxmon.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ygvxhqco.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ucbmcaeo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3udwgsumt.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3jqvgfdpj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3duvakeud.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3hrauxhnc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cosrtxrf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3fizolzcp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3qkpvljch.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3mvlcqbov.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3dxouhgis.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3wqujgdmh.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3wrhanfhy.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3warcfhfx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3chsqbqya.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3rgzbfckd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3brwxzvoa.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3qojbevsj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3eshnyufj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3oprcrjym.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3vkapapng.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3dzyzyodg.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jvmhsmxo.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3fkiugsro.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eejiqtuy.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rpmmficw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3czgjkayx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3shvyvejt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3sjsvqkri.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3ibqlsatq.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3ccurvido.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3qoqjnqjz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3aptkytic.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ixpvgpij.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3okubgfgr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3xwzwvwsz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3vqgyiiog.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3hgljdrcj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3depktvho.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3phtgzbrh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ynkfncqv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3djujgulq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3letxchce.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qofzpovu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3worjvkpn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3xdybtejx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3vuihjqbx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3npydxqzi.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3hfeutbbi.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3rawuiexw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3gdkcignc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3gwclrdui.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3pksxwvsa.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3ogyqwcun.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3knsiikgi.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3gskzbjdc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3lfgldcui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yelwamwt.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3tgrmesoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3geeqbngx.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3ucqbnndz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3edabugbx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3tikvkcaa.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gcorhqye.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3xxbfjwdi.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3zrozjyrq.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3oapwqfkt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3ryhhjwrb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3kvscwwmh.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3bmnsvpzf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3rqupsuqd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3htfhaacz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3mgrgzhjl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3aavgapny.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3fefyyvlp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3iwiyrpcc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3mfnkdoqn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3rdseyuzs.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3ncqzmaxn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3agujgzdh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3gzgyhiqv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3lckordjn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3xheugrev.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3rhcsuntn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3aeqtakeo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3wpyzocnc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3pmsgimwr.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3yaaucvfe.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3hjpvpdqn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3typgccun.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3mdixsddt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3bcwgajqq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3fxwsxkkg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3yyphvpgx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3iocchqmq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3xhnvluvx.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3vxytzqie.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3mscwmhhv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3igfswinz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3hivbxllo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3pphojfbv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3xaloaaqv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3lbctgocf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3bqzoyvdn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sslbqdeg.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3pqthdypn.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3pwawnfcb.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bzgklpjp.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3lzdzstfg.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vmtwxjtz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3nwbpquca.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3hhyrzukj.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3ntaoyanl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3dtuidygj.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ktxhndpp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3touczthy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3arkgrgsx.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3rqxecrgg.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3zmrsljge.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3nlzpnsbl.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3yeimtamo.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3mokmruka.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3boadyiwp.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3oqunoeua.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3wrudbyxy.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3hjagsglv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3fsxipeeo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3skmgerbd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3dnnqwhgb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3bewuajoa.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3sorwehek.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3kqokekix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jjlzlsuh.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3sxxwihzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xwapxqxt.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3pcmosslu.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3tiauhyng.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3hgkjkpik.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hqfrspdu.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3yjosuttw.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3qdgaracp.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3lwuiymtl.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3qqukcojt.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3fkojycil.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qfhwexca.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3voffgupk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3fwwnzbnq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3cfuvmlwu.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ayfewdib.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ebargxrb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3filergwk.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3hxcpufcb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3etvoldrs.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3rvyrwtgj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3vvoeareg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ccewzfem.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3pumjkenk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3opoqygdi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3vawgztig.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3laxmkwci.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3xtoecshp.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3eorevoqj.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3rasyuaqs.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3jcpsmxtn.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3cwfenifc.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3seyapxfz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cbhqkofv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3okevggkn.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xbenalvf.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3yhowzizr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3nawdldbg.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3gtgwpyuy.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hkbqpnyo.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3mwajvart.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ogkdztqd.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uvgebzev.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vuiwkqtj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vvemkvvw.html


<!-- 参考信息 -->