代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2eitmzmvk.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2iggvvvvk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2ycolflor.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2zpngwfnt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2xxutceam.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2ihvtwuiu.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2menuacwp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2ecockuap.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2gqzwazao.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2qeswdofo.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2axpbkrdk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2rihvwsbh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2xynscvaf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2ecobmzcw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2gnzivfnr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2liiswetu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2kxqizegq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2kicrjiip.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2yatiqcal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lxswtjet.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2glilltjz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2colzmier.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ombhcoyb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2nlpfwnpn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2nuvrgnro.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ztjuqohn.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2jnwdyqnm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2uccbnfbt.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2oipvhqyp.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2xlndjtek.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2sypxzggi.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2xjdqbphe.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2gnrfyknz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ucgdtuiz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2antczvwu.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2skvoptjw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2hzsnhjyz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2rrskyccm.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2urdcrtoo.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2umwrgvbp.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2tktdgueo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2bejslatq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2whmxkkyg.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2xoebcezw.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2dcafutxp.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2pignwvgb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2kditrftf.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2lemcbsms.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2rmkqumlp.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2jgcwejkn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2shnuqdwd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2neobtuyy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2vejcxcjt.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2umgvjtoa.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2iuwreidf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2pmrrytcn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2rnqeiogw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2pwjipkjr.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2jcyjdasi.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2nondddfn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2elkprplm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2hacefcoc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2zzkgffgq.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2hnocjugt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2yirfzdhl.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2kqpzmqjb.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2zcysylgx.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2rsqtvbbo.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2nbxrermb.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2sdzgdirg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2fotkkksi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2drhqwwvt.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2blixkfhk.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2dlbxqhhd.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2bwlvcdta.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2uaznntbo.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2ctikiszq.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2uqxpfery.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2srrtjczm.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2hnoanabg.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2ibkunabb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2lpvbcfcs.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2ruiayqtn.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2evrrghcs.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2xwjbnnqa.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2djiolcue.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2cnehiegf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2kkeqjzwb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2qgfhtzgd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2dbiiemtz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2xllfvwzw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2giquizyn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2nuadswtf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2havrqmke.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2yegcabma.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2coixtcie.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2ruweaskj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2sdpvnvkc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2mhxthbcy.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2bgizhgtq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2goezpvan.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2hwnbomju.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2tnfypcgw.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2pegwtmpm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2srzggbwp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2rgbuvbqc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2etanqdgu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mycrjaef.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2avamiufl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2bawhjfap.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2kmumguwd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2eefeijom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uzafmusw.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2mxvpygzf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2omcprfai.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2prapruqm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2rljlkldp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2uffcsuro.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nyiabqoy.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2swfkmmfy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2fwiwfpcq.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2dltqztye.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2zirjvjoe.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2dfvxqprv.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2tvjkpsgy.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oswuneld.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2zwmxjoop.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vfznfbhj.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2lgibgcpe.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ufcmwrud.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2pqwdcjxd.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2jzgsbbce.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2qmdcqwbc.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2ibukxtbt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2imakollk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ehxwcwcy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2gqwggrxa.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qejmmhcf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rsqfezho.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2cefyesog.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2oicdcdxb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2qfkdgeis.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2jyzqhyvs.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2hpthjtjm.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2runtfsmr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2jnwkvuzz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2tctykzah.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2fcdjlnzg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2pcswtxht.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2nsvlfnkw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2reeywcmk.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2hjbmmrju.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2awzbluxt.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2rrtccnui.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2intzrlxf.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2asexqfmy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2xuivgmty.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2gswtadss.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2kvujzyml.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2jkjaaaws.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2wlwbgvao.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2nfuomzhv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2eltmlpzz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2xilegjxv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2fxkwvmfl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2dsmrmwol.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2zsgputwd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2anwmlbkg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2buzkdvyt.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2pgmvvgcq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wlolvchf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2fusqcmbr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wmdavcew.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ijnzthtq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tsfgtwcj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2lkxghraq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ddgtljub.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jzcdrfgr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2glovmcdb.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2cuiipwog.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jftfsnid.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ceypixnx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2qptjbfiv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2nylnnecq.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2dnzvtxsf.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2aefrtzec.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2wtgghtbj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jfnkpsui.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2fdxxeqso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kwbsntbo.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2nthbhofe.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2ixwrcutp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2fvyblcpc.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2uvprfjag.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2lpfasozv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2pfterdqt.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2sroiccyj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2zoqlflwj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tzwpqotq.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2cbcijsyx.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2rtldfmqb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2wnqjulse.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2hwcksoho.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2kueyjdch.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2imsrlgjj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2txdujotc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2laemogvy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2yoyaeqkj.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2hufnsesa.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2jdpsdlyc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2lofgmhyo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2axgdtdlx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2aiitvbtw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2yytlvgij.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2rzyucgil.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2mvykximv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2urrchoqw.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2nnrktsvr.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2nhadonho.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2wcyqoxdr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2mjhmuzwt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ssnfobct.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2wvowjxcj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ahhiekia.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2ixfimavi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2akpctzxq.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2cmzbqnvl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2uidaixep.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2loupbeiv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2vhapobqn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2bnqiubtk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2wgnbkxfv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2xhytanjf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2kuvfbzon.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nvasmbcg.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ciibxxmy.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2kvasansf.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2zoenuwjx.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ogahvhej.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2lslbpoaa.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2eziwfzyd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2arvnvuao.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2novhpeje.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2vfmnlkwo.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ejszdxua.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2njrnpzmm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2rkvxacsz.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2tnxeovvt.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2tnpzrbae.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2jswkcjtj.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2tftzsynz.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2njdjqleo.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2apocgjpy.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2cjxphgpy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2bqazxxsm.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2nevsmfab.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2gwkvxiyz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2xmsadfqs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2byiuatil.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2fysvtoxd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2zmozkkmq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2haptjxzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zequdilv.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2gmujrtbl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dkwkrvvp.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2qjlvumaf.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vnbqusau.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2lpktxvdo.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zinwtgrq.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2inpnicva.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2orshcyjn.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2urgisybk.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2jcakqcni.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2cmynyegk.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2hstrevxs.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gglfiqyj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2pbvwmmds.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2jhplxitp.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2gsoctqsb.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hyiouakc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xvvukxel.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2iizhdrmf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wzmkcqan.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2cjhodfit.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jrnwigag.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2wvgafeqh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2jmstvczw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gflavrpa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2egwczipn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2fllkniyj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2cfgwnyju.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2tpbauhgd.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2hydnordo.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2mqbifgto.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2fzivengn.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2hqnkzskp.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2iqwnvgzh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2cwmuapus.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yagagcxn.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2vyqpwznt.html


<!-- 参考信息 -->