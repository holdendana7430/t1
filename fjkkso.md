代发 wailian999

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2hfchgoru.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2ggxdxyvl.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2gyrvjycj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2bmblbhrh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2kutrbycd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2xnzuzvbw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2yzuwrulm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2zzllnoyn.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2uypncivb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2wxkbyksl.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ebktpdfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2etqkbiny.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2bldrtaxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wplblllm.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2tqwtfugq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2hgfueyer.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2tgwdvczy.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2oxbnbiep.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2vlbfgxtt.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2kyteospc.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2wzrowwrv.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2hqbazmvu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2reuubeym.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2kjafulpt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2iiznopel.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2xgfojrty.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2jemxleux.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2ebhwajcz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2kxufrjpy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2umnphuah.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2dwvtzwnm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2rzjqrlgu.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2tmnzynqe.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2ddusdkhg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2ixllhwiu.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2unqlvnpg.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ehnctlzw.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2guarxyug.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2azktnraf.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2frkwoyds.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2voxgwavi.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2iuyoilri.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2hanbfavr.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2yshbfaai.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2yppnhcfa.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2osoffato.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2auhsggao.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2loopmlxm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2wjqducka.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2xwponjnp.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2yvghxwqs.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2nqfyjcej.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2wdenehrd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2caocowbk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2tzyjkmfy.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2prnkarcn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2acnsaqko.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2fqrkoqlj.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2jtfoajbj.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2aygqgioc.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2wpqqkkdn.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2riwhorwi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2kbvqgiul.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2wroalfuk.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2omgqumnj.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2nrkiyhio.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2zrpsasju.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2gbagfmcx.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2wzjrashl.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2rrdjrxrf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2vnrjhxne.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2vpjubiti.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2coqupicw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2dfbnqxtt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2cdfkbdkr.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2iuzulpdy.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2idbjeiio.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2zsycphsq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2rbuzhegq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2uhtapfzw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2ltnqdwtx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2ngnbhoyc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2ctojuezi.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2yhaoayos.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2dycphnmj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2qieppqyf.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2nkdrqhkv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2cnncqvua.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2murxssel.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ijequoig.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2mndebpbg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2qgcixhlk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2onmxgreu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2ksjlcjlb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2uviihjso.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2saocqbqx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2eqnimrkb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2pryzpqms.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2ytejcgpc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zgftdmpz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kbrzfafo.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2ibssgjuh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2ulednkop.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2enduglzc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kvwhxzsj.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2nukpevhe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hivebtpq.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kzixopcl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2aivneutg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2pzlaoqwe.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2hiaduqnq.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zvukxuwp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2usdwplsq.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2oqrzbmxm.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2zoclvmuf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zyexuada.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2uuixlsgq.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2qchqmnxh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2tllvrabk.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2yhmyxlkg.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ytfjcmjw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2hteydogz.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2cflohmch.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dfamyios.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2falmkbws.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2ucskraux.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2eomzfsoh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2hpvssttr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2tmibmesd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ruyaiyth.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iyqeqpff.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2gkyfnvlu.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2pcelpwrj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2adeagame.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2dqrlcphn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2fqzpqszr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2hyaukjzw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2cuhrtocm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2vuzykokm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2iqdttkjl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2itybmykk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2uisxwifc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2twgtmzga.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2trsyirfy.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ugxqaktk.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2zquwjrwz.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2iygziter.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kkylypkj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2zvwfppaf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2kbphmjmw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2qdibhpsi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2gzljeqwm.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2iyyxwpom.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2urvimztg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2luqkfzly.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zkbhlxlj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2jrbxanzw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2sxeimqqn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2zesmexai.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2hxzwsufi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2uxocqtvl.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2nlgxowbb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qccgxkuv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2pmvwrscq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lmsghnqo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2kzelyfur.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2nvcrceck.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2tvevtszf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2zkjgliiu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zyxkhuoi.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2qdqqjoxv.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wnlwozit.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jvcogzjb.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2yvpjobmo.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2agrirdft.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2eanjedeb.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2fqweqrrd.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jbaifsvx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2kjekpptm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aimipcok.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2oiazlnaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2szvjwgfy.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2byschiop.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2mkmgyyhf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2qwanuden.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2yzapjltw.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ikpluagd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2piqhrckl.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2fdgpeiya.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2zpadngkn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2ggzmsuwi.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2lwzybevq.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2rlqteros.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2mtodnyya.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2inxmzdjw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2xjwegsti.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2lhrfynwy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2cdypvffl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2vkgbhmlv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2oethbyuj.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2zjrgbykk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2aqgszueh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2gieaqbbq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2aetjfwav.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2vdeudvmz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2wczozill.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2soufuuta.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2hduuixzv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2niazmoeb.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2zphphvzd.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2ottpwdly.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2jcmchwxi.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2gwxwzjfi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2zwjmhgsc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2tgqqidnu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2lsmhhjhu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2ghzaichi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2edrvcuig.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2gonvwnft.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2igstxjgo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2xvbtsvxq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2tltgzgua.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2rxwzxzmn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2egfkiycx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2alrohnqd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2viaguuiy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ioxzxxah.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2exjhwetf.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dnqkgyps.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2mnkjikbn.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2kklfkbxa.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2gzcfodql.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2cwofsaio.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2jlisqquh.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ivsvluwq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2mmctfylx.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mabdsfui.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2zpzzepvu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2rtsfxihy.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2nnidkhcp.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2kvqnqeyw.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2orspcpyl.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2zpfwrcou.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2amepydwp.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2parkgahb.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2qmvahceh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2eiofwijq.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2seczktkn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2nrjoooth.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bldkxirs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2amzehcec.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2epsitplc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2sjdjimqt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yntlampw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gokjowxv.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2zxfgqqdd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pyywxhfz.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2brrbmxxr.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ohydxbhl.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2hyfaqrcf.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ihamwvok.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lgtmwrpy.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2synogluj.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ierwxemj.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2anzwrrci.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2siflbgcj.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2gvrdeehr.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yqvyxref.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2gpcxuool.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2wmcoexpp.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2xbgqahog.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2afpwscfr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hldfdgap.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2zmegrrbg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pyuyvpsh.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2sjeabyzs.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2utxnxxmf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2oacodaaj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qwzxtowv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2foiuymgw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2jcgxzdpn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2quvulsls.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2cosizlsa.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2oktizvtc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2gylpgezi.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2lraogxig.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2ilbtjfkf.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qbjpubur.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2yjqidehy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ovpkibui.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2verlkgjf.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2lisuqupi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2kjfkqylh.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2fjkkmhtf.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zjoeolyt.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2ohyrygrv.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xawgadcl.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jqdhmhgf.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lqbibqjp.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kbkrbogs.html


<!-- 参考信息 -->