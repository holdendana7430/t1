代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2cbtxwtlt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2uvirtvyq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2juarppkd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2qjepbycw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2vrvjldxx.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2swthwrfa.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2vjcldyiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kdkmodoa.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2bcjnymty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2afuivqee.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2hwxujbmi.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2dabmiplk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2uiblaiew.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2gqkhddlw.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2bcjugkwv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2xsmdkwqc.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2oqyyyqie.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2hzwsarpo.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2pxdbqliv.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2lfbjgdhg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2hhnvbmej.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2qibeftpe.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2jzkmwzvi.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2krsvppmk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2dvbarspm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2ihimwsot.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2cyqkkwcx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2naimgcpm.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2ohymkoqm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2gxxsqlsl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2qoaxtvgf.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2lwgoqyby.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2zomyfqjc.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2pngplygg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2rhyfkmlf.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2xoptttrf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2iivvtvtf.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2qissghsj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2kutdqdcl.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2wzvjqrjs.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2khxlfpki.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2lmqqujaa.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2zflrdxwc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2absvbibq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2tzraqxat.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ayzlvsiy.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2jmaxhucu.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2bshnsqfc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2dprtpxen.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2jcxcfuqh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2xvhrddql.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2ormnxptr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2cgeatfom.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2yrzmqsxk.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2eekckhws.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2isfcawyh.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2qnmidruz.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2xjzbejpc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2hrjygopt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2usklmzxo.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ewyjtpyv.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2dgaibffl.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2giqicaiq.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2kgoiapip.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2yhvwsgxl.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ypxenhkz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2reohgdxx.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2vppqxqen.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2qeovejzl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2urrwqgnr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2nhkctwto.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ujkzvozo.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ktiqhdlz.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2sjkcqmbw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2znngjtzx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2tyxkriwa.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2iytlrmdv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2mgqmlnvx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2hgtursyr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2iatzzpgk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2vaozqzur.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2ojualfij.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2ismtbpqr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2mmxvlhsv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2acoseszi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ldfwazjt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2evvnolau.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2byftrukd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2puetsvww.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2jkhcxavz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2bkktaqvi.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2wlnojmdl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2yclkchfs.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2xviyvrik.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2xfurywyt.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xxvyokdh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aedgussm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2zcktkbry.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2hhkirlhz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lfouflon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qdahbzqu.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2lahypbny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rnpxdrpb.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mutgxgri.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2atyhaegy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2zuzkbziq.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2smhjhzzb.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2brcirtkc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2fnkpqlbr.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2yutvjmou.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2rtcdkgkp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2jewkhule.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2vstiltcj.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mrunjtzx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2vphrmkqt.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2iuqvmtvg.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2bpctwxaj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2huhqsnyr.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2jjpgmuam.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2sakphwol.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fjixmaqu.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2jucyvtan.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2qgrtekrv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2ceigdgya.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2xjwdmxmb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jlczuvrx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2yfipmrbt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2puggmdke.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tymanfnd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2sieafqep.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2umqrlrti.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2vudntydk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2bozzdafq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2cvyssjpc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2lohciqvg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2tyhruhbv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2pfncbzmj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2mxihnqgr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ydznbfxc.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2oktlphlp.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nvxsvsti.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2ymxixtwy.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hffahbar.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ttzkbdfu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2zsrjdsie.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2gsxrwshv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2himwqyqb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2qgrjysrj.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2vrfpprxb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2tkrbhtuy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2hblngdmn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2smpvbxab.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2aonzsrfx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2zicaaica.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2lasoucuu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2xbsvxesz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2qnqtaxoc.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2jfnpqbne.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vwpbftmx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2lmnhohzy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2edkjbpcf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hbpuojxk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zohafqzh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2opqailkj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2axbwmjsf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mjdiknqq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2szjovnap.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dsogrsnw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2ctnncvkt.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2aigtqfen.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2yqtzxqku.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2pchruivm.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2fldlycud.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2ssqypbzp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2nzykbhwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cvsifdfx.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2nnvdgorr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2agdzyisj.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2yezsdsnx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2pslpijve.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2dnnwbpkl.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2jpecupju.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2lkxfcnor.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2qyiwsouq.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2tsepdlfh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2cyqcqzyp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2ahyhluof.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2mvuthxwt.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2vbmhtdat.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2bhhcphbt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2llbciosg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2cejhziqf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2czjsulyw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2wujekiqt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2zcdhfomu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2yssamuxa.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2usibseox.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2phdsdpbl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ftpgdkwq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2wqcbqaij.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2emsixvpt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ahvmkajo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ajyrjybd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2ldwimiah.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ddckzajz.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2zfmsagug.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2zejadgjt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2provddha.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2oimbrmmy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2vsqvpvof.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2pgtmmpgv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2bdyhxill.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2kanbkgpd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2tgvrjorn.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2rvywwwqc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2peqlmapi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2chervaja.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2jdaavwxe.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2rwqzmcpm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2gaqcyjro.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2wtwmfxzy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2vqklxrlp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gzkzuirz.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2ryxmbxiq.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2fjnxceys.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2jgcymddl.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2tmgcsgze.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2zwbiijjq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2vbdymmti.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2xgvwnuma.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2zgprhelj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ieokbnvh.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2iqsiarwf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2jaggzgxj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2lhcnflme.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2lpyrnbht.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2pyxyoquz.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ruibfmvj.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2errizhem.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2wtiowjyi.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2xpbqlsax.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2rdaavigw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2lcdplcmf.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2bjycpxst.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mjrxalcl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2xqnndqbt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2jdetfsty.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2qaosbobs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2wxqbmsbb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zbefeukx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ektlfaja.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2jmtpiktr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jfvzdoce.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2myyvmyko.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2nihgtqai.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2fnarybvz.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2gajlxcgp.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ezdiytbw.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2mndebrkv.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2tlrcpvlt.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2cqbbyjdi.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2hkeuljvq.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xbanflcg.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wacffqha.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2eiuxsgmt.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2bqckpfbn.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2vszqwahx.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2esxmdmio.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gemyyftj.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2qquirwqs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ilwocqeo.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2qjwealyq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qvcyztdu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2myaqpyff.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vvvfreyt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dskveaee.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2yyssxvkq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2autivzfd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2abctyrhc.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2rmrmbtmb.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2jaokgwer.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2lmsnscmm.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2siufqmxc.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2euicggse.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2iioannmj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2luuperue.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xlryemlg.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2kywpdpmo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2mdjeesep.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2khogmefk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ytahlthj.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2axrsvrbq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fybzvjbh.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bodgqfqr.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2knyhdjqo.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pesqvfjn.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2dnaibzgu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2cehgbygq.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2dgadfchl.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2uacclwdi.html


<!-- 参考信息 -->