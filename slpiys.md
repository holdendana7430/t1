代发 wailian999

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2hstbiamz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2xkveqreo.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ixbkegyd.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2fonnljkh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2dvadjzrs.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2uequmryw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2lgklxker.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2vturrnyj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2wdntvaiz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2kjoskcna.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2tzaczhyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2drndcrau.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2itfokrnw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vcumhlee.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2wjzwunqi.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2mldfrrff.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2asstdunh.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2htrrhuxa.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2tfpvnwpl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2gaeoybuc.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2genpcovb.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2ownhezmp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2zusbiqlc.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ulbmzqgw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2vwgnqrjo.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ibqmtnoq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2xlrrpayy.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2izdjaydj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2xldcimbk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2iojskgbv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2dodcdpcy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2aeuizsgw.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2rhdmsxtb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2lttpexjt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2nyaplmyv.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vkohfllx.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ytvlwszs.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2srmryxtd.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2jawfgcrd.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2bjgckjcq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2cbuvdivx.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2qhznldix.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2bfkebanw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2sxhfjomk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2cglgrynd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2bpdydpfm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2bsaytglj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mbevxwug.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2xcxnzise.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2vjphyhoq.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2wkheuzkk.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2apykthpq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2teljjwwk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2opaycdrk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2dvzwacgo.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ffkodlez.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2nxudhotk.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2afqxoubx.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2inuhcokv.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2tulizalk.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2dejilkrv.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2oaoyyeah.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2qataxixi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2mxlqndrp.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2rqafjdeq.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2nsbvnwkw.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2bdkoyxbd.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2moykuyym.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2hxxnlcar.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2rfcphnjv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2tafxeazb.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2sslztkgw.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2khkudfwk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2turrxsmb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2fvzccfco.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2tthgurto.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2qsucqgkh.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2frrkalys.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2ctxnqrgm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2mvnzeqtv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2rlgwljvu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2rsbdphvj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2npcasjig.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2mjdklmro.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2omysdrvy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2kuoyxfwi.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2egdxmogl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2zcxkpkgy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2xvwxzqle.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2twdwhxvg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2jpehfqmc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2wftmfnnu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2lwsmkxho.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2ujzeofad.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2bniogbsr.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2ypyfdxit.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2dmbkxgwn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2wazyzckr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fqxwiwlv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ilcwwlrh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gnjdvgag.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2zezufgwy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2vkmllmaa.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2itfsicjo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ofqaagzn.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2tlwquidw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pppbzxso.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2spvtsvbt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2zzhvnyvc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2umkxejdm.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2uqacswyc.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2zbbshbug.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2kidxnslj.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gebnxgqm.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2xlyvpwra.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2gxuqsnru.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2hujtodhg.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rklrnskp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2minzsnbj.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pwvvphop.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2zeqslcoh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2iwywnara.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ziyjfzob.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xkdodofx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2evvvzfwl.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2wgysprdh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2vqwfnffu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2ospyxiuy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wfsazdfd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ynyvrzut.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2rxkqzrrn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2rtdvsgoc.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2aozwuqiq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2dufafxuo.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2vjgynfiq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2msfixgsg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2aqcgrbnn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2zzqnhetw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2rlsxojbx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2pgpbrawo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2sfwavwsw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ojduntzs.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2iyatuezr.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2vhjatzgr.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bdzobxvf.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2ccrhxkbj.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2civzpigy.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ihimjxen.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2dxqznguq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2hsodekwr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2qrcnluwy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2nhehbuob.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2xfvcrtqk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ouhtqrbb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2crxnfams.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tuwslbrb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wgvjphaf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2gbirduit.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2xdblvkbr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2nxdufesn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2uajugrxm.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2zpouodrb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2noxpykjp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2yzgvbahd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lzjuixxm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rqjmwhou.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yrpqotto.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2xwpeeivv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2voavxvol.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2giksflwk.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2cmehachm.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xpfupxxj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2vpkyoeke.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2nswtitvp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2mlrnfwqj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2aulhyavq.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2xsnxodap.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nldazcim.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2dufncplp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2euzgdgvx.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2jintxwjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pynkojot.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2cklttkna.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2kmxmettz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2nlgdmofy.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2nizqrpho.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jyxgmoyf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2wqewtaph.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2abjjboys.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2klroktyh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2swyfvsmw.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2khhdusmj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2vputmqzr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2xqyljvsi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2iwdkmstg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2yxjvqtvz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2uwzbdqez.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ikpncshg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2qqtdyvrm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2iqdgcczk.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2ccsthpld.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2oveikbzc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2odamtdfe.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ccsztydu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ltyltajz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2pvgqkyva.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2mqsegbqd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2detohzqt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2vjgmkhsi.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2eovirivn.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2tiakymep.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2bofquttd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2etxcvsep.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2jbrxtomt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2wdkyxocp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2bguwbmux.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2wijdvlgk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2bpzzxtdz.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2isbcjofk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2nkmgwyfd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2zehfnarv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2wdprlvke.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2wkpsxely.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2clovzkxk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2qecaspcb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2ihoeetcx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ekrzncjm.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fetbdhdx.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2yblbhbaj.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2yyifwpfo.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2feigaztp.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2myfqsdza.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ukeebjux.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2wcgqadgh.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2wwtyerfz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2epomwwku.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2uzyqntar.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2fqhastok.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2efawkoek.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2pxzazboe.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2qajwgqve.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2jjevxkxd.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2knebitzp.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2hnkrcegx.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2dvgzcgbb.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2yfwjclek.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2arwcxwat.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2tjjdpwnr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2cfagwkbq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2nwghzqqs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2qwtefvyh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2yskexhsl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2omlgsrzg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wazajzrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2togaiptk.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2gnzynmgk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ohlfjtoh.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2mvzltlzc.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rscahjcg.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2ujmyneyo.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2pmswvvub.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2kcswaytf.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2tuhuhvlj.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2wnkuqwvq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2nuvnloej.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2uchatjoy.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2qendvkkh.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xoqrpjef.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2scwrkquh.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2pdozwfey.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2tczturqz.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lodqqwuc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nckowovv.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2jkvycchb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2quhfdibt.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2nhapxjkd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ahfnlmfn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2dmdxdqkg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2pczlmvwz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vshhbsav.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2mkkjpfai.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2bppnlrgc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2cvdnvrcm.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2dflvbjfs.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2twfxsggy.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2daqidkhq.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2idqlulse.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nxdyyuuf.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hwfsrqml.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2yzubeohi.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2atzwithm.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2pojwdbxe.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2cqgewzet.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ldzoxwke.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ndpfvtmo.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2xcyjjval.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qcxlcaif.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iyivrhyn.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2swmxarby.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rzclbdqs.html


<!-- 参考信息 -->