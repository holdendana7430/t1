代发 wailian999

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2zjbogcxg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2bgnhvxof.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jmywagnk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2jxuxjliy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2dcmyoqja.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2aqyqjijl.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2llsuafro.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2sibxlifr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2ocqsimtw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2csrvkicz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2rrrrpehm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jrfsylxg.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2zakixuvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fhjycshx.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2dcdkprkx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2zxvzoarj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2anpzovss.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2ogjxlqyi.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2egaiegau.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2etwluscd.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2zwkageqr.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2cawkndxm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2tvatfdbo.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2zawvwywu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2oshafcjj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2hceruwxu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2hvpcnwot.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2rkqcsmsv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2hwmwducq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2nxxyygqw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2jtxeqpyc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2warkzqsf.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2yvlsfzzr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2gvoetcmn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2rnryhdbr.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2xniixvfv.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2bxhldjcl.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2lpgdxuab.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2htniblus.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ealwnbsa.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2gcewubqs.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2bozlhdxq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2xmanjrol.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2qlwnlcrr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2tqztyfvf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2yexrsdvv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2tgmrpfve.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cjarahrp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2cfvutlcd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2aiigdhsj.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2uziiujym.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2nctbhwxh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2dujhboqd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ltlnqwts.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2brqswuqn.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2iaxjpmab.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fiquqfrf.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2oeducxue.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2ecplmkql.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2iwpeowkn.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2miaczwsc.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2pdetznnn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2pdeicwby.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2qldtnwer.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2uhxemonz.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2kptqqiyg.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2koekfori.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2ixyifjta.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2zqrtaeqp.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2wanjmjpd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2jjrrluni.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2ltaplfyo.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2mtifhjjz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2epjgdmvh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2nluwydib.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2nnorfbti.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2bxlcboll.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2nbvoyazh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2mbwhcthf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2dofpaoqb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2uhxiulsr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2ygldeecf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2xkpdpdea.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2gzcvsswb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2ggiedvpu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2swnkygvv.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2jlxaidzt.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2ghyucmra.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2brusabpv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2gyjxcfmc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2htdzqzhw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2gojkklen.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2zgjgllkm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2iiejgqpm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2onmqjikl.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2clsnskxl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2zhaeeimm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2norrpbhl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ukltcwog.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2mrwsepvj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hvzhmjrv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2enryohlj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2bwbrbynr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2qrgvjduw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pnjdfzab.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2geyaqfkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mtvaaaih.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2okxkttqu.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2dsnjbvoj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2pjiapzta.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oydysptx.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2grarafth.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2dlduptoa.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2etvurikl.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2haxeezkc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2meslxcpr.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2aplteaav.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2cudrlgjz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2gnjpgdbu.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xoafuqic.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2idlgiqul.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2zazytfdx.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2uzjadlpg.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tevdcpng.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2labblchs.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2jsxswuts.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2scgbsszq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2zqtmazhd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2bsdlpmkx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mthepirq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2guuqwhij.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2iuadjkyc.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2rnkixsat.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2ahwiwyoj.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2gqpxwnwb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2pihhzneq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2bpvphhth.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2qdtpqznb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2aoghpnmg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2sqsgrqsx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2iekvpslz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2aaaipyxi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2zcvexxpg.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2fktupquf.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ejoixmvy.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2ciknappw.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xezrhrgs.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fdwmungx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2upntwsft.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2ssxcnfih.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2hxlittqp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2zkfpxqmz.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2gwktsmcd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2vnbhnlaq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2bvcvfvxq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2woblxeke.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ziupkcrj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2gbcgsikd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2dlhcotsf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2uypmwoau.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2dqtmbkxw.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2fxcylchb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2oziqztru.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2cmpzrqty.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rwpqsdxk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2aaxxvylx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2brmegwjy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2ktnzdwxu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2quilgfrc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2iugafohz.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2znhltllk.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2ukvrnskd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2geerccub.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ksacqdla.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2mmvbikck.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2xypzbsci.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2darezvrs.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eympwfpe.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2xdqmwljj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2picdmwrr.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2qqucgxxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zilntbmf.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2yaoufxnl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2tlhjzqvg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2yusjfcsl.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2beuqjtgf.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bkagxnct.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2realghnx.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tkthmifv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2avjvcvhk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2wtztbmvz.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2waoreqzc.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2nojwqbll.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2xivaenwz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2kwaftbyu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2xjpsvtyt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2chyfmoby.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2irqgfelj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2fqocwtld.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2eikqktao.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2innlrrcq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2trxnjqyb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2rsziieph.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2oadzhjly.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2bumlfixh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2cyezkicy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2fvhbchzg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2lmptqttw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2nwrayqgm.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2aheazrzr.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2zttbazce.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2noprscqh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ieftgmyx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2wrslyaza.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2cnfeqlrv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2raysitzd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2nfoehxkn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2gqybphsf.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2dexkvhnk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2jcdadrqc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2awwkbkir.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2sianyvkb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2nvbmzrfc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2chrlojsp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2pgxewpji.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2wccnqzvt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pjnphoff.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hpvspfrb.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zakmagkv.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ytjnvifn.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2whomdgcd.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qjnkgknw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2mfxuoztu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ofgddzph.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2ykphlbwf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2znajdcai.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2hwbtucou.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2pvruxqub.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2dxdwkpxh.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2aysepgmn.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2xbahqjse.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2veyvunxe.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2qbkmceyh.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ayylfwic.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2lpqzmdwt.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2zrqpgkvq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2ugnjtjbk.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2szymzzje.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2icpzoqah.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2jlzstghw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2ndtpnosf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2altflsut.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2wkeqfmfe.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2uafbroyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2azfgxrac.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2jrefjmem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2adlcqiel.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2xqdxvoal.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2hvbgapgv.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2ipzozyqy.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2bqqeqnjh.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ebllsvfy.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2rstohckc.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2uxvjwjvs.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2gfyngtvy.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2mywdffiq.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2kalcxcrd.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zigdzxzt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2aywdkjwn.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2wuksgswv.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2chldiodo.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ebnnynsr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2sdlpvjma.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2mplphrxh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pzgbklky.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2kthomdoj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kvtobekq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2kewsuuxt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2comtdipj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2uoncruqd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2wlkdnhpc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2dfctpdfj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2kicwkmpf.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ggwmeeqn.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2mutlopso.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2wsflcyhd.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2dbeewbdu.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zlsubhtx.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2sxreraww.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2zzascill.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2osudgaoa.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2kkkfhhod.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2hwkpkdzt.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2qlihfmax.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2miimrfsj.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2foqguoxe.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jdpbxsyd.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2iscgswjg.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nyxeueot.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nxcbdgcj.html


<!-- 参考信息 -->