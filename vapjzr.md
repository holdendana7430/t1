代发 wailian999

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2bunsrwec.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2epnyccwr.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2nrosptxu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2xidcwcap.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2unweprzl.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2fotmgpts.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2sfjyllus.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2grqqpzof.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2woovywzk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2hobjlqsq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2hawgmwrg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bpyegrgu.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2bqgwafmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ookkodyb.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2mdzycyqe.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2lofxrskf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2niksjzad.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2pwygsfzu.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ftjzhgcz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2pgmimhqc.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2arovkobo.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2veluunws.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2saplgrfy.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2nabekehp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2xrfjehrb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2rkcphwrh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2extvxzdb.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2mguojoxg.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2ckccbapb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2lsgwodny.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2racayqth.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2acowifur.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2saufxkup.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2stjjucyk.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2kjksnpuz.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2oufiohui.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2waxveaai.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2oulmymgd.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2lqupbgus.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2tbnxpqqu.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2uxnfmzlq.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2mmifciem.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2xvnzmyyd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2umkwbhtt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2rtlkxziy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2tacfbpas.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2qfbwwcsv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2rusuucme.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2wymodsft.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2xianawdr.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2spmjmqjq.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2uhqylonj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2nmbmqnei.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2snmjeubd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2dluqbdqj.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2vhjkwjry.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2modzpjco.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2wfemyhox.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2izhispno.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2tocsrakx.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2qbuflmcg.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2gbkmfpua.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2hxjkvbfu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2egtaxzfm.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2ykmcysmh.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2mshscacp.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2ticuqssi.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2kjvwxoaa.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2jptybalz.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2wycszubw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2gmlktpur.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2fubvrecq.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2pqodtlgb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2snfwylyw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2ggghwyxb.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2uzywaibi.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2fcannpvl.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2jjvrmqbh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2euxkpjnf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2sclejwtp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2baaabrwx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2jwbhvtvq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2ndtrxkma.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2fwskacya.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2cmsybrdr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2gjzcvpuq.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2mixlrayn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2mfcsyjxi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2sjnhcpvv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2hhgtuafh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2knttuffm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2zfdjjpps.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2hmjjghsq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2cmjqzhey.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2sxzfjuoe.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2zyivdgwc.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2xxfaikxv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2mbvxrqfa.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2jsqdcrzn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2mkknklrb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2omfrbgnp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2zbqepqam.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2sfllwjpp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gibtmrwo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cjncwgog.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2rudlujjy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yrltjfbn.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hecxspsx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2dffhcgjo.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2lkyyuxxd.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pstofhdh.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kecibwjm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2gnkbtwrz.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2fdycwmtt.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2wkpkjzfn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ioylrrzl.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2hkrbzahq.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2hcuavmgc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2zrmvxynm.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2orsoayxr.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2sraucwqr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ifjcmmqs.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2bysqqacc.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2nyrlffra.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2smdccvxk.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2phlzblzv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2rxxvboik.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2zdqnddst.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2dbqinntb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hqaurjzz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2rwfpyvbt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2rjzfklrs.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2qqaqzjlg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2fvojokrm.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2hzybvqus.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2eqbyjpay.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2tgpamkqy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2lbmkiozc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2zvbxckzy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2rawazvpw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2jgkclqrq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2nejgarmh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ncmkmrnd.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2ipnbjpim.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nztguygu.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2vvyzpquy.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sliwtxzt.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xwfqpmxz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2bwafands.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2dffuqbho.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2ullixujy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2zusbsvns.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2qjzrqipf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2edkctosi.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2wkklvopr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ypmknggy.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2oijrzvie.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2ezvyegud.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2rqqpvpzg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2uvnopbis.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2olxwffku.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2tfekdowi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zynhfhot.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2jzqawgjs.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2tlxdkzyf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kxkuhpcs.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2uifueofy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2wmxrlcar.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2kokqarvo.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ppyqxndr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2ghfgflhu.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2pfbrtnnq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2kwiuefgz.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xfwcrzxb.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ijknyipd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2ewfdgmhs.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2brkaeock.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wjleyrmu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2hjzoccsc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uhcvvora.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2bjvsbiij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aedwqbql.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2sjuwsoeu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2lmguwskg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2ysxttvjw.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2oaaowowi.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2iadmyfhg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2zginowxk.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2npuiytig.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2pzvvnzxo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2byrsnnak.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2wduiphxd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2domftnek.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2yyooirtq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ugdmzouz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2oxhbuyvj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2unosgsky.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2kedenrlb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2mkconcbk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2zxxcuvoz.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2uadcjwop.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2bzjgafhg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2aolbupbe.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2lobyfsfn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2hvbadram.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2hnnxwjlg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2qneupoka.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2zvurbexm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2gizmgepn.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2qmsxkhcw.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2wsqxryrj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ikxmcyrp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2bszaaacr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2zxkknesp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2xuegfuuh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2modjckes.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2slpforgw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ectxebia.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2miglotze.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2evenutyd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2rhpamuyk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2aiqidned.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2klznozdk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2hggyacrs.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2pvaiinsf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2gmirejmq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qltcrgkz.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2zguwzmfm.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2yelukshk.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2dfxzpleo.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qavfqczi.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zotisjjs.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2lmgaqngy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2mfsqczdm.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2jlbdunyt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2vbyhhxlq.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2puuletpj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2xlbpjqtb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ivoxxueo.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2bflnvato.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2sewdvpmz.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ybtrjinh.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2eiolleyq.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2ehswgsym.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2tjprohmd.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2ptkfjoyg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2mcqlauxi.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2dsjwfiii.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2imcnzixo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rvvgbfik.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2llbdkfmt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2qnbogpmx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2tnbahnqp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2pscydsep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zfrqbbbr.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2oojanhzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qxvikngi.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2oreevpga.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ucvjmzdc.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2tdbgqmst.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2uiusahdn.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cwccuctt.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2mxrupdue.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2fhkqkzfk.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2wzaetakl.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2pjqdaecm.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jzuqkpsz.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lorvenwd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2aamqgist.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2uxixljsr.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2nahiaddi.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2cajijmgt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vyfiqett.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2affdfckf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ntjfhyds.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2frnifolq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2hghoksoo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2jgwvagvy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2dcadlanh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2gfvapepz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2vcikaofc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ywtsbepb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2sumlodpp.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2kqajnpry.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2mqdsjsxl.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ivvslqzc.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2mfirnixg.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nnlmqbil.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2tvljlpyt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2tsfhpusi.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2pydrpuiz.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2fqxubqsi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2bwzkfvjs.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ldibivxt.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lqwzqhzh.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ympzkbdm.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2txrtpbhh.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iemegahz.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zlerfhmn.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wijrtqkx.html


<!-- 参考信息 -->