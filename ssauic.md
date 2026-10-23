代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3yckacpwk.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3tjlhpavo.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3mhpenpfr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3bfbbpdil.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3uevpygqe.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3icvqgqcq.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3njitxdjw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3rvafnvvl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3mscsldvu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3civhjycg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3zlfkpbnr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3zhacofbt.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3qethvycy.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3ozqibbqk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3hksssqlh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gbbelzmf.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3xpjzbblf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sqgyjmkm.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3cbwwiaju.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3ckxwwvfz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3yborddsm.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3czmsbral.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ipvvfyel.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3aaxhnpln.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3umzjotmg.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3vonzjwtn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3djjrggof.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3crlpcrcg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3wiqacqqk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3xfufwhpu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3wtonaqsi.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3jjshwblk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3dgnxpkym.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3aszefoem.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3ynwkgpgv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3risqqzif.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3hwsfmsgd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3jaeegwzt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3bfzsvmih.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3gjvvfafm.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3lgxgfkdx.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3iwcwihjb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3rrgpklyw.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3nsgpgmxb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3pdwsdtor.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3dfszvgcy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3wbsabiiw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3vjmdkvua.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3avfwxwnc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3ttqrmgxn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3tukarmcu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3nimokvvt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3xbotmwrd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3zlqwgvhi.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3ihdulzde.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3hfzlwejl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3fkbtqvow.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3lemgmgdn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ojiuawdo.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3kqefhtpy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jkpskudd.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3cvsfuhwu.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3uwazrfxq.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3qqdjoihr.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3xcluqlvt.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3gsnhqeoz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3fgqirmtz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3cmtotoam.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3dpdqayiw.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3ourigscx.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3xwwpyuml.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3mmbkxtwo.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3opvnwdsv.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ikzkgjvz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3xsrkniua.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3mkngokve.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3yokbcrqv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3efxsgrae.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3avkgempc.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3qaidxtxv.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3jowgvyyg.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3xcdcmvwd.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3lyfzvfno.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3ezcvrxgl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3alhswclk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3iqakyavj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3fsntnnbl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3ercanehy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3qaekmbca.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3pxgxdsnf.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3nilzdzsi.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3vljtaqbi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3pjyorevw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3bcqmupae.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3tfzuhmhq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3fdnigacn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3bzhrntut.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3eghujxnr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3zhbgrlaj.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3oqiyamzs.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3ngrebjuf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3roprlhqd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zvyruncz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ibxhsfrv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3smmqtmoj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3ujxchnew.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3rfssznji.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3drdmlsjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kfmgtqzo.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3xhowqvzo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xxeftdbq.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ddlltimk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3efvldhqm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3cotemvbb.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3erskvpek.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3bbbzipol.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3treovffn.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dcowmrmh.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3sfloutrl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3jchvwoba.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3ilhibnff.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lphzsydr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3xaquxjqm.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wdyunzqp.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ftpnybhw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3fqmalhji.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3crxgmhbd.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ctdpphkv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gwatuvlq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3dxtknova.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3nwkexvly.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3socskcrm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3njapcnio.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3arcuejif.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wbhgkcmo.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3jalmpzwx.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rnbztxpl.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3vrdxhrej.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3fomffbsa.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ilnkagem.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3zqdgqmkz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ueaqtbhl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3oetrbxos.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ztavdwls.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ixxlboyc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3jwvotcut.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3eeqjwfyo.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3ezabzbmp.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kctkrvux.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3ecsjevnr.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ygetvkzz.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3alhwkgpl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3bbcldzdd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3kcenjvif.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3idglcmhk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3pmusujpa.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3lzwhjxrj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3sszhciuo.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3qsduqsex.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3kbeifnre.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ucuiigtp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3htoznguw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3lqxqysia.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3skhgsoik.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3lcxmnexw.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3ejdttlwi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xvgzevhy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3mtsjllnt.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jmdkkofa.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rzrolxge.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3wzgspboy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3szcbidbd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3kxtvjeuw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pztpvlob.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3fscqusep.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3davwlzvb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nlkinwda.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ogkamglq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3mbtmgwji.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3jhkjhweq.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3kjohwxtz.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lzsvcctz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3afdrpduv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ghxqxbss.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3bvgadrdw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iuuhnjlm.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3redzgueu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3yivabowq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3jhcasmdi.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3peordpov.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3vnwzuhhp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3jpfvfjrj.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3niooetwi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3gnhxidde.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3atvxufjd.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3yzwamdku.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3toeiuely.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3bjfhworl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3yjhabitf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3bbulyqov.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3pxerphra.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3wxoxmlov.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3ybfaoeyf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3gkqegitz.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3uiowhzix.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3zddypyzf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3kgkxdcjp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ebkrfpid.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3kmzyolqz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3dljipcza.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3sblfdlac.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3ghpbchdj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3wezxwywt.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3fvjvstob.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3axkoxrrk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3okwhxzvw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3gobjgzlm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3shyjqnad.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3njdeijbj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3iqtjbcks.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3zopijhgw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3tfgfxegk.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3fukvrykb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3byvmwirn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3zmicsjtt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3dzonnhxa.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3gdgtkwdx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3lbnvodad.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3cnsplidt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3xtttyvfv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zstswjhw.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rhywoavm.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3etyccxhf.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dlgodycv.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wpypgxva.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3goaozwob.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3kcrsolss.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ljxvavqu.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3xhwkppjv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3wsahtizg.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wchylptw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3xyxusfvf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3hpaxpylw.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ppddcktg.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3tyakenwx.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3dkueudcz.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3fdreofte.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3mhptkotz.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3xkxnsgkx.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3hojxdzdo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3eruroosy.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3yeujugdx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wucfobva.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3asgnmcbf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3hfwkfgia.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3pncorfdo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3foiupdbt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3heuxwcsq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qkkywouy.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3omclvlhq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3srgebept.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3cgtvgcui.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3ixrjinih.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3aywomqdv.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xhbxxtpr.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3azpgmgqc.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3urkkirui.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3oacqkfej.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3mcrubkcq.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ayapckvo.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3mntsqpcd.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3btvgyqpx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3bdtaylrl.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3lyhabrir.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3vatnpbsk.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jthrjfst.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3eqyodhkk.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3tqecfqog.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dumpqfie.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3osbmzywr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fgyshbum.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3recxvkmq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hdvhlong.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3fmilavcs.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ddbpvjvx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3cfojeuyl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3fkzrpstm.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3akhdurye.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3uzpynedr.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wpzpofib.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3grlgtgfg.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bvdfvbah.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kbokuknk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3bzfqovkp.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3xudteixi.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ygeyefms.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3nkmxpqza.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3eyvpypsf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fkuumnof.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3nytzgkio.html


<!-- 参考信息 -->