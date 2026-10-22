代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2tdjqysdj.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2xjvjzcbt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2mhojvesp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2znavklfd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2ajdcbpgj.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2ijykwibh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2rhmtsfcf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2hiuactqm.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2dffsnvve.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2lmodoiwe.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2gplzyxzw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2ngrwcwxt.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2sgrzeauj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2efcblkff.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2qupaxghz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2neifhdyx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2mxwtrpxn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2nnrinali.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2rgdqydcu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nekyeqzk.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2erubvdwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ixatbnbj.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2psilqzgz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2ckptmprr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ukdjqvjo.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2cnvizmgr.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2bdspgipi.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2csitmyir.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2owacfiws.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2hbfvbvyo.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2arkicpxd.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2jhcojikb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2eknabwfv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2hpdvjqlc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2pxokspyg.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2vnlpzqja.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2qrcvbqve.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2cqlczpcx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2tancctmz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2ttcrefht.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2jvlluekt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2ombnnohz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2weeqywxe.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2kwctwrdr.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2aorednrc.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2aqefxnbz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2gkmxsntf.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2fqrxuueq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2jdholdmj.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2ultqftlv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2gddhqfdt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2ioppjytq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2gegxhspz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2quxxjwgf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2dygadyvo.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2slwvjfrv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2osupztdw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2kcgolsfc.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2pcxfysdo.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2rmvdvgsz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2ssybzzae.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2bphphuvi.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2knkjaxhv.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2jtjhahvk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2bmxlqkdl.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2aikfdxqh.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2eoiwdvks.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2prxfrwox.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2fdvhpkmu.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2hfpygxxs.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2bgtuxzry.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2bbxbrvon.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2enqdvokd.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2nqwgracy.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2drpxczht.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2omgvgobj.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2qdihplpx.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2wlycsykf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2cdkeozyh.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2blgiglxz.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2vhzlvdct.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2iniqmtff.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2gyvnhklz.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2zofbujwa.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2skspaaui.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2dvuzooah.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2zhfirlzb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2xviozwqb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2afcnmxuu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2chilrvdg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2mvmqugvs.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2xukspdsl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2lfmspbyt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2xomotmef.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2lpjhbrcf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2cfwdtgbf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2bynzobqe.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2qtgktmjw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2shsoagde.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2pijwnutn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2lkhtgojm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2ntpwdvll.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2gbsimlau.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2wjibiwgl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2kcysruts.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2cipeopnd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2wstnqqrf.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2czhqkwvp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mnjpkksn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2qwykdfcd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2vdzhdcuf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2wdcwogha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lvvmoqbb.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2pczqeasm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2krpywolt.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ywiynxea.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2seiatrdp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2hsdrtpjc.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2orhamatw.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2owurwhto.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2pqpeemxb.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2icqetxgj.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2mhtfeuxl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2urhegtpa.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2dbuaprkz.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fysykzha.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2dsgsfygj.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2aqaesyle.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2czxvhduo.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2uhmfijoc.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2mecmnzix.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hfvxtuuz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2bbpszexy.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2rejlzbbp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2xgafepwd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ekqfwywd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qsyydpjk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2vfqgkqcr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nhnyzdbf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2husmdipb.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cjctcbrv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2cuwupmxr.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2jnsfowvs.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2rfezhqwk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2dztlchkc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2cztbphyv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2kxbehamj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2mzkjkqab.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2xghbpuki.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2mviucvyo.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2rxzuihik.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2nsclywiy.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2idxijleh.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2gelvzqcj.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sfftovoo.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qkhfzker.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2xufiluxd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2upquxvtz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2odruidwg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2znqrfewg.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2qukrkzzn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2odqvhaiv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2jsjplpvr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2xbbuixew.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rjsbedem.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2cdmrmufs.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2sicgiqeq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2cpwwvadx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2mesepcaz.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2rdzwfqru.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2yppedftf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2qvozjxix.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jcfrydwj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2gswrlups.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hzpmxuia.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2njyzdlix.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2hmeywvbt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yaiolwof.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2bedfqubg.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2esjnwjqr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2ajgvenwy.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2hbhofjdj.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2fqiodsox.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2bprnakis.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2slcoxpbq.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2asdxnriy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2okbewkod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uftvxrxl.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2tlsvvzww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dbbzdayl.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2vyqjpnwh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2yoaahypd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2mmmydeym.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2kaaedmky.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2sxeomuii.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2kxcgkafa.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ebuyqprh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2mkpdyyqu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hqaqjwcg.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2edekwqkb.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2lqabcjdx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2uqpfmubx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2hhwlkvtq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2xehlagdj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2xdtydcea.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2otnvsyca.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2ftdfaerr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2rcwslxbd.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2orycarsq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2oftbwqiz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hmicgvbo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2lgkkdhik.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2nduuupim.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2nkefrbys.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2mlhzznwi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2pubooznr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2vyhudklw.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2vetucytv.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2rpmumgjo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2yqlypchz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2zqlcnbgc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2qotlqdvi.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2icijpmwg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2bdipnkpd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2nciitfgt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2rrtnblkp.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2icbphmgx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2yfxfudfj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2atwkvoxl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2drnuhdqi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2kwnciken.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2qxrpmxby.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2wbwqczht.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2twbvyaoe.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hqkodxbn.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pwhyxwnw.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vovlnaim.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2dwcorpec.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hhhigftz.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2znfijcyw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ghuggnpd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2zcgcexkg.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ynqpoory.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2jdugwsvd.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ihzpmuta.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2dkvhqtqn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2cpfvrnwv.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2squjoiem.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2fgklgrxi.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ydwceopm.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2mdvlydsu.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2titrkvwq.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2isyfiehj.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2kwipawcw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2bhabuwdw.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2cuindsrx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2txouyoxj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2gcpzorfo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2imqaprjh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2ajnitivx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2brioeevn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2fyjdwwte.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wodljmso.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2mlpjdsjg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hhoupfng.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2pexeydad.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2tzytepyl.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2bwntuyzu.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2dvayqewq.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2woxuvxel.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2cbqszrgt.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2tozxayiy.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2qtvdytcn.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2xxiheldn.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ebxwmbzg.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2oigpscfo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2vqbskpgd.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2zemyedqd.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2xmxkayzu.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ofkkplpx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2cwesxtnu.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2wqlycpeo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dgtalyks.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2kbsjbfcs.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wkyrlamq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ewalckae.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tihecban.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2aayfshlx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2bbzjmvtw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2pizrrhzx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2gyiczzof.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ikbrnlmu.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2xewzzqrj.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2njznzqbx.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2fxvjmcwv.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2sbaweyks.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pojfqskb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2nfqcilqj.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2slnizrah.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ebbeegcg.html


<!-- 参考信息 -->