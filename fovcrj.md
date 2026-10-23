代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3vzscuqgg.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3zowmhcax.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3nruhdsqs.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3bbioijvh.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3hesnkjrf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3licvxwdo.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3lhwskgaz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3fzywymif.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3wiegrado.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3utrqjmdo.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3mzconfhi.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3lrntfuds.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3bfdcwcgk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3jilukmqj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3cxmxoovf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qqfpleca.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3npvvemby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3crbdzkoi.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3sckwsris.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3nhaqyahq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3dqghfpko.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3uiagpsrt.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3bxbcgmhg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3mgborklh.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3bqcavfzo.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3vyaujwcp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3kfuiouoi.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3hzdnsnls.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3joavaekp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3unzzscoa.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3hddfdxdh.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3bpdrfurv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3moevtvac.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3vfraamzp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3guhqxtii.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3oeujwdbh.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3wchesaxj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3oppmsono.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3ydwznwvd.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3xjmqhbci.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ouceiuzt.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3xgotekhf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3lerrvayz.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ixldmhnb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3bsrffakk.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3yjqqfhnp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3jkmrphpe.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3shttakpj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3yslthimy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3cadlnukd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3qdlmuefa.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sbhmdfsq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3phnfpjoz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3wkrvcsam.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3wugzntce.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3fxrmzzaq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3huzgrrsv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3irrrpprc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3etgwdish.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3hvblwecd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3hplzfikl.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3gjsxmgha.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3mjsdydhy.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3sukhxglc.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3iqvsgkaw.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3nxryojoi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3oletphrr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3ligpqglu.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3nvgnbppl.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3bswmtaws.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3selksigi.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3hibfoibt.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3tezgcpns.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3irthezgx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3ylnzvqvs.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3ldlncdcm.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3jpdopoox.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3pwnswaum.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3aqgihqpy.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3disenthc.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3mzgrbbof.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3xynuousv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3ozgxkdvu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3bjcyeanq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3tqllvjqi.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3twhpccks.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3gamwtcfq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3ittspatn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3mjyjotyi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3cjzdvsyc.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3pmihkkij.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3xjsgslho.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3stmhjugn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3genbhwpe.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3kdfsvdwa.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3uurbggyy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3orpfpwyg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3gnqyooki.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3vkftmuec.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3vffapkzk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3nusnstiy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3gzekxgpe.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3hkrutnyz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3nyzsofbp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3dgvurtrg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3dntfutup.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3uldrcpzr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3ihukorlb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uqxehcor.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3zcnefhxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fsvglozu.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xpxvjfsm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3iqgkjfvh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3lduhcsuj.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jsnsdiom.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3kgstnjra.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3snflmnnc.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fywizsrh.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3yxgbahdf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bkxyvdgf.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3jrjptlcw.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tnvasuwh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3idlkexab.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3atupmtba.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3rqhegpjv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3uadspwcf.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ntdrzcyb.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3kunxkcxc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ijbkyjij.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3ydxmegjg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3kqrnwkju.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3rhzxyfmz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tfvkfxvc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3tmtsdpbl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rpzmbttl.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3vzvxlkft.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3wolkuwhx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3vmksacle.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3glcoulno.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3bvtpzpbi.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3vligotaa.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3iyeqvezn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3zinikklg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3jvitczoh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3zlzwvmjj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3qnkynlgs.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3hnjgusuo.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3czvcgfyq.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yizzdiuo.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3qooswqal.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yekwiupa.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rxhwvaoq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3psalcnss.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3pfbtuayb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3vgqocmht.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3wyyvdfjx.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3vtbrxlak.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3oetcztlb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3whwhnclh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3mhthrluf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fcxtxrxc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3ggikxhjz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3kucfkueo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3jhpdndwz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3iaxafxam.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3ypqhypmz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qzhptdlx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3nerkthtw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hiqltoza.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3djlltdyv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ifykvclu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3bewwfgor.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3egysnpqz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3adabdnym.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3wsmhkudk.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cszgwvdw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3mrnapcmu.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3vbhrilsi.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3jnjlkght.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3uwzugvsa.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3okkxxlnk.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3nremwlre.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3trdvqxsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3shzkamvo.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3xqqwrosp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qdqhakli.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3pzgdnzmc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3vardfbaj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3kevupbxb.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wavbpkvo.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3icsgnade.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3ehvqqlkb.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3zghilvtd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3dfddacen.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fxckwmrq.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hcwquanr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3uaaplwcg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3ccfwakaj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3drvgafrp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3xgtczjsf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3gtwdjhgc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3tpmcghza.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3gtejigux.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3tiulznak.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3dusjamij.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3mcldlsjq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3yzskgcww.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ttqiasxv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3oozrpfwz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3amawfowt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3qqhjfhlu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3jwfxfpji.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3sslbckwf.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3pwxibiek.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3guhmlykr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ekiwiqyb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3fnhzdmav.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3hnzmyrwv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3repxjfhh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3paannduk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3okkudsix.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3vqdpknnj.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3dbtingzr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3bkqtloqc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3suyilblc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3vsgtezwf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3vhrhbbgv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3rmswfjnv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3linrryxx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3bxpmegpu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bjyptlxk.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3tlualugj.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3odhtqjih.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lvbfilbu.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3eysdnrzf.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3mgxfbufa.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ixibtceq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3oomdbaxv.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3cpcykviq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3drdvuovp.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3cpjukoiq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3zapbziot.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3aqkoyidn.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3wytpwbrz.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3xfkcqfpx.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3sodwzkpo.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3lumacgdk.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3eqoxrmrk.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3gslihmww.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3clqskodm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3ngnylfhb.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3fwapiisq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bfutttca.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3esfsyyjr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3yplcblnf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3igswstzi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3kjalylsg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ssqggobk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3repqbnce.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3wlagodez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3waxebmwa.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3hqbnlzqk.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zjbwtcay.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ikpommue.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xmlmzjme.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3qcdmackv.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3fivysewp.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3jeblhpmx.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3kgtqacol.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3gkbfewfz.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3cobmtigz.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3elyynigc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3rhrhutoh.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3zbdydbhd.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3mpdjwtij.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lacpdcqa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xkuuwlaa.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3kfnyuxta.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3sxmyxwyk.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3qeojbdwp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3spwmyhxo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3omrsbifk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3hpyxbtaw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wvbggxso.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3tpcixfba.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3qafvkyqp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3ctkikdkk.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3xjshpknj.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3zdkwwzur.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3hfsnyslg.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3jggqrsyu.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mdymuswm.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3hjbyrelg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3cnpavjns.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3iutvpdwh.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3fncxngzf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3kwqeqdfq.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3yrefkmdl.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pjggyvls.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3evabzvbj.html


<!-- 参考信息 -->