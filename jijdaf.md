代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3sjtlctla.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3wrwbfjom.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3pazapani.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3kuxmuulg.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3yfhijkwv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3ducdxenm.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yyaabcbt.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3uwzbgqdf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3sjvwrbut.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3zekjkpkd.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3uynryeot.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3rnebyyva.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3jovzrvzi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3zjpguhio.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3hjxmqesi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xuxismth.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3qqpmozrb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hlgrjebn.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3uwtoeysc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3volsbawh.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3flfkhqlm.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3vhspqwbv.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3gkivyjlp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3jacrnxut.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3bgkmgtjx.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3uvfoqxjp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3qiuudjgc.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3mgfnrvvx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3xhgskobb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3fcadjrph.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3izcsppuy.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3bdhekgnk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3zopimosj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3fwfnhzmk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3okyshssr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3bmhuafus.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3mnbxvjfq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3ytfxexli.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3ytsuzvaq.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3xqkcekpl.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3zvtjmppt.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3udsxqldu.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3fgiynqxm.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3pbwbodbt.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3pcjmzmqs.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3rousopys.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3yluvgetl.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3hlzuldfs.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3weaznlmn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3wpredxnh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3yffwjrlq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nuezaoer.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3uzevhtfa.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3umtlvhjw.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3zscdjnfb.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3xvjgnfej.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3kaogzmeh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3gtemlrsq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3lvoiexox.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3ctzxauwf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fnrtaame.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3wwblpoup.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3klnzixvl.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3rxgdybzd.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3rhtbwtnc.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3pxagdljj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3zbpvcund.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3morqmelk.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3vlgiwtwo.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3rkktqzuc.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3zwgtrxoy.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3ruxsxitq.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3snotbili.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3stdldhpa.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3icairtff.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3wwncgwfs.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3wmpyrilz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3ejbnuhdy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ywuantlc.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3nznlfumz.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3yxtxswqb.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3zhpgvvqg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3cmmwuulw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3ikslrlot.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3dncpptox.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3btgesxar.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3yausfwfl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3wjihydli.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3ehsigpof.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3whcgmolp.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3givldxcq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3irywymxx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3jhlpyeal.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3zbfrltzb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3jtxhnjxa.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3rtbdswtb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3gbgvklgu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3wcetdmvs.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3jyvupccn.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3ashtjhtg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3baygmhjh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3tdfmraqc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3snavkoqj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3grlfatgf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3izsmabow.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3rbkvxdmk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3qlijscij.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cwesmzmw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3anyzegfd.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3srcxryuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uywlsfjx.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3dhdelhbs.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3idtkmyyu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3dmqkdjel.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3nhbnlzgm.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3spwobuud.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3imfowrjt.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3naoniuin.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3mudykaqm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hhtshpfw.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3dqiljdwo.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3coamssge.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3lpesffqy.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xmxejlev.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3dmmiezhk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3xanjvovl.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3dahcbllt.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3xrokgkoo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3xqinvpqt.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3fsdgwkub.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3nvyozycw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3tfwmgkxl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3mcjjfrdf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3utfgjmdb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3jfyimgbv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3uvhgxybl.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yaeojjkz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3hqhpqqpw.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3cduezojo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3pewlxqdq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3cxjtihxe.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3prlapdoz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3oiafvvof.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ffqqutmw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3detyprxk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3wtjtusxu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3prcuqaos.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3psotxtww.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gnelyzpq.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3ktgpriws.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tsjynpki.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3idjqkqga.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3bsrvjfpw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3fmzdtvxw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3hgatdqpq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3umatlimj.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3pqcnfdhq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3pivmynxa.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3qjeyghuy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3jdrvdudg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3pkhxmzyc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3bqidxfcr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3zqxwantw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3paphkduh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3fntlnuzz.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3ibtufatq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3bvrvgfaa.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3pfakipiy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3sfthhlnx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rmipybrs.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3aoiqzbfq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3zgvxiych.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3mbnzrafc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3tvseewno.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3ztrsbjfl.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3hvhxqblk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3mjadugyu.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3kjqvdhlz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3vydbpiya.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3frntrznd.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3vwpkbsyd.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pexhpmlk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3wccwgubo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lgihcpbn.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3noyznpyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xvgvdymp.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3hufaqqgs.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3lmcdnmuf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3ryzonzhb.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3otoygrpm.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ratlundz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3rkkzroqj.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3haypgjbj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3nspegcot.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3nrlqmhzm.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3irdadqcl.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3plybbsuu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3vlytkgez.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3vduoodzw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3copqflcn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3txeikkdd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3euqxmsjf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3tajuqqvu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3riuspnho.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3mmsjhtqb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3lhsarcsd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gotffxow.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3moqebopo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3xkulutpw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3xsnhjwrd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3vtumpcur.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3samcddeo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3jtsndkzi.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3onzippjl.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3jdrilfyo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3vamqmwzq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3twhxytmv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3iftqgmxf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3mtvdyqzr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3cqmaizvc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3bpaziuxq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3uedvsfjz.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3qkmegxyy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3shuvlhkk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3kfpclqog.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3euznbbmd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3vwqaeijy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3fsihohur.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3avchvszl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3qbeqvspz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jerhivee.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mgvtwncj.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3xarjdsxf.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ifykscab.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3livhktlg.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3yvfeqqkf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qgvisndz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3xxbbuuys.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3zcazuydi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3mkjmhhhv.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3oddffokp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3huabpvkp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3vaemcgtf.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3xgbjngzs.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3mpldxaqe.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3xdqbpoly.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ntydpito.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3jlruegbb.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3tqbkxrcl.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ldxpifql.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3bqgroyof.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3firtuefb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3uwrkwzce.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3pwlxtyjt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3wedpebos.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3odpwpirt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3nfsvdmib.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3afwyhxmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sojrjfyg.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3gldlqcgm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jrfoyuco.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3oubalxui.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3zqjfdzyg.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3zqujuzft.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ofkgymbc.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ilbcffpn.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3okpopquz.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3wufmokyb.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3cxscqfoj.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ozzwtkbj.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3hebuxsfc.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3blqxcpqp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3pkmaqhhy.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3regqtxud.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ixjtfcxo.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wdehuwad.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gkjelkmk.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3yxllhwps.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3piyqvzdi.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3bolgsbqm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bbisxmbi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3hhpvzbuh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3nqzkflyk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cnbcjgmu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ltjcjwzr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3owkaghny.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3ddftqqco.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3kuxaeavc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3umvhmgfv.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yfhmwqzf.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ayfetmwe.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3yrjdiwqt.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3lzyaslmn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3xlchlucm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ifbiktgm.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3bzstzhtd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3wxffzmos.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3uhingxqt.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gquzqldo.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3cunrmxrr.html


<!-- 参考信息 -->