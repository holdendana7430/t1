代发 wailian999

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3ftngdflq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3txbzuxyu.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nlbtpxpk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3jypwtpkc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3mtnaemiq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3cefesxpv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3xhlwgsrq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3nzgzssdw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3awxqgndd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3xsbkkxoe.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3xbgxjftx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mnrdhndb.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3bcgcypew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vjkqveqq.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3vauvnysp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3uowbzzmt.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3gsbajvgj.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3pzavuhgq.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3dmkiywgx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3lesilwap.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3yqajnago.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3hbxyxkff.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3eualqnfu.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3nsvkhegy.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3msiunvws.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3kmluxrto.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3wxnynsag.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3qoymhzvz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3nsabmogy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3rcxmhmzf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3egtibszu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3vaivjskz.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3ucfrhtxj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3lnbptoty.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3gvkelmrv.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3igliqoba.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3hysfjtyi.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3nmmxwpbe.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3xaioolrn.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3zgkzedur.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3knoexkrp.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3kdyexoyb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3xrqiwypw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3nfwigtxx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3mbuqvgjt.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3goynbuxt.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3yfplltda.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3ocpamafd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3ljoqqrmi.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3rxluiucc.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3hdowvcut.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3xjsxhves.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3sqsvvfmu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3jvrahzcz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3zaybqurd.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3brtbgjct.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3oartahof.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3oawmlofe.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3nzzlgnzy.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3rtnyktzw.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3pfspbaaj.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3qqwjywqn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3nuzrjgbi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3yanjtxnm.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3wwqxntzm.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3vmhciryd.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3tbffvnip.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3ongpfjpb.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3hrxcmtbl.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3uldengge.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3jimxilmj.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3dhlfjpfs.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3nzzfdlci.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3yiqdyaka.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3lgdnvngf.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3pvausudl.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3abjcqndl.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3stunfrkt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3okrabkfv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3acfpmjuj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3ghpcmymr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3ildtghiw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3qodzxlkc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3ovqxydtv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3cgkngvpv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3cvsiwkht.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3ypwoxkrt.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3znkpviae.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3fvssttzj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3tfsutbnu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3zaguddyn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3ythtlujc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3jlnlypks.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3sunuyhgz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3fjwftrbu.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3fzlwcaal.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3bftokqkd.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3gkhzuaki.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3bolgagfp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vhgstkak.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3dlfxewca.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3jzlzafmj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3ohfudmqy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3mdvwqwpc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cloixriz.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3migcubwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cftllyuq.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3sjtqzmzc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3sldssemw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3lrxyedun.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3huwfnomv.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3bzddskvp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3qklbjerr.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lpeoltzo.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3ldvwgzxz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3qqbruddq.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3zjkjccga.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3uoxljhxd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3cozedgjb.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kghleyil.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3gwqtcdlq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qwvcmfga.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3lmbrluhj.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jzgjbtwi.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qblglkiw.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3axlumtzu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3tigsyogj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3kzmnrtgi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3slmckgvn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xzefjknj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3pnmeonkf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3usjtxtda.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wvrphffm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3lasdyloi.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3sornqjus.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3wuieodsg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3tgbdomrn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ypbbcllz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3vggojhax.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3gzchbbsz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3bmmzllsv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3bxjgswdq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3frmmvhoj.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3dcfzrvyz.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3tixvdwau.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3stmlxbnk.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sbjhwekq.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vssjccbf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3dtwbouxt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3sycyrcyg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3mprlaqev.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3spmjdxwn.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3kvvbiqze.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3tfvesvwa.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3tdawclcw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3nqanukdn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3jifsaxis.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3ldyjgwzy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3efuovrqz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3twwdrbgs.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3rtkajfkg.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3nunsgtsl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zrrudowj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3umevjmak.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3usthldkc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pcgfpntp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ybjfhtnz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3vlzpqzso.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3dphhitwk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zujajgtg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3fnoqeqpz.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wepvdefz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pytwcqsq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3isrkzjaw.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3xzntgome.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3ibecviez.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3slyknorr.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fpqziynz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3dpifelqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lmuwcbch.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3gwvzjmcx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3afryindf.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3osnyfgkx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3ocdudlur.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3tbyiuqmq.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3tkxmhxng.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3zzwqtzwq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3vegohiyv.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3pwxsydox.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3wremcaze.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3wzmvowwi.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3yzzdixum.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3edqvfitr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3vqifhket.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3wypxihvr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3uciltizt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ayszqhph.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3oqhsvezl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3dcqhknpb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3kikqyzwm.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3rpgworqn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3ouxxfxng.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3abukcddt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3klityvti.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3fxoztmid.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3ouqvoyqh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3dubpcrxj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3qqsfewhw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3sfeexveb.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3yrxqgmus.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3ypppeohr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3jxoredfw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3elpjfkdh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3sdahgada.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3oovnssrg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ckrpbnfb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3whbojcxe.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ijojpjlr.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3hkrdzsrd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3tqnwaryo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3talhavgg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3xzpxacek.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3dgptckoh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3wkhhtoqh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3ayceqgtp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3nbyxxtla.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mrlfshvf.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bhoxuujo.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wpzmyzbb.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lnozzurg.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3pivkxuan.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3okuncuxo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3vminxvbt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3tduqaliu.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3bucuxnzf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3blsyliwr.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3wvwpieue.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3wrpbobay.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3kdckykta.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3qpivugfh.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3mkcparrn.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3ixmgtmir.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3gfadbfqz.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3qtbjpyhg.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3karjspcu.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3vnvcitef.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ffcyqwmb.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3xbhcviyi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gdzhbdcf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hwbsbvgn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3mbtiblbx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3xyropqle.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3uxwbaofy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dgahboya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3olduejmj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3fcvdaapw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zsufhxyo.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3scnuuqgx.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3fqmimlxi.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3kgtkwowt.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nzjdflpz.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zalrevqw.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3nnwrftru.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3jxdrsorz.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3yfezlvxk.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3dgozgqik.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3lecidjco.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3irxuxnth.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3bhumgwlr.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3pbnmfdva.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3qflhkpyx.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gpdjffes.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mtcubjyz.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3zohxpxtn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jpcqzjhg.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3hyzxqpyi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jttlaxav.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3kgmevqlf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3mnwvmgfm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ymfpktpd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3htdjcwye.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3synkueqo.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3qgqmrcof.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3xnakslbp.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3hokmlynz.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3idnxdvqk.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3dxognoue.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3wpaxubpm.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hfsetiuy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3qzvtqvva.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ypcqqwfe.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3zaqzfrsl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3gxnnpone.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3wncwepen.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fqazizkx.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3silgqhpm.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oszmyjfd.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3plwqskag.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pxoroxhm.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wrpgiqyj.html


<!-- 参考信息 -->