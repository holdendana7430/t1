代发 wailian999

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3zrofsayv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3wsfkisks.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ykuntcjr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3hzrobdah.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3ppznmhlk.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3xjjcfkaq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3mdwsrjnw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3vmaenmcq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3lbaptgky.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3kdfftxzo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3spsniopl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lirnvnsw.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3llhhjldz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3prgmpglq.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3fjpxgihv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3jkuzyzoh.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3dekryumz.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3pzqgftsf.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3foagelck.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3axkuewsq.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3grdwzkpe.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3cusjhcsc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3bdargtaz.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3mdryfkww.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3uwnujepz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3bmsvszpc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3hnvexxvu.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3lebzuodm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3xvqwccjp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3llvktutk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3kmwwqjkg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3fgynjbda.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3dlfzgwyz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3sopmvctq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3uodvsjeq.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3tdyyovom.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3jnmlawtc.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3iukjovxu.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3twrjlhig.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3cjxquzew.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3unwbejcw.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3klhtgjzx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3jdolbxmn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3epihsexy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3psdeqqgl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3fqomyzri.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3rckxerfp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3baaialov.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ktoilgaa.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3liyhtheb.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3dbudsrsq.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3crqyfvin.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3dckcegve.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3qhscniwt.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3wkudzeoo.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3cyijpalc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3yfoqgnmt.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3myvljzaw.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3lowpksbw.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3uppfxhqw.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3nzpfowza.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3lionxhub.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3yvqtwzqi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3kjwnuqmo.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3uaskyvst.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3ijfulefx.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3audltnxy.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3wnnobzcx.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3nelbuqvx.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3nbqrhgrr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3fxmnzkby.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3jcaaijye.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3cfwyftoa.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3thtzdwon.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3sictfdnm.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ydfeeuev.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3cgkpyqhq.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3yjtrfbws.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3byiuwxmi.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3fumovhwu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3pcjzkzwe.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3wdjbbwop.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3rozbghdw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3pqpceszc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3gvdpwlsy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3mqnlzjzi.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3wllnsirr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3hpptvjyq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3krhrbotw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3zjymiskc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3cetxbxcf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3feckgvjz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3maprpjtg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3oajyiwmw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3gfcnuinl.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3lellswbe.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3hdsxepsj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3nacqynme.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3qmsnvsia.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3jtlyoygt.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3isfhvfmu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3wwlhsfqc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3xxcfluhz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3kvywszrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pahfawhy.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3tpuhmhen.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wxqibxsy.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3mxbztlwq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3mpnetsak.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3zbjxxlpc.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3qfugccqa.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3juauuhhw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3zxsvrkql.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3outienuu.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3isufsutw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3tkrukoow.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3ofitkday.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dlafsasz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3sjnjbgro.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3uwqnnwyu.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3zxwzxxgk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3bjblqoiu.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3qumagwqm.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3guxicbmp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tmyvmydo.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3vjatqozg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3hnqrhgeo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3gwriehvj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3ljvreiut.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3ismhbvlu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3otrdplve.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3ueyriagh.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3lgtdnbff.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3yurhecma.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3oikzbltd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3abkjwrce.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3tpshpelz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3itkvzbpy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3dytzgnqx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3pjuohars.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3eswijezy.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3adaozsgc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ylblorep.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3qjidntac.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wlrlflxt.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3arnhbbap.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3aztxfchr.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vtekmzkd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3rlvqktys.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3vfgnadpf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3cybezcsu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3qymmswgg.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3tuoihsyk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3loijldko.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3rksksiij.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zrdtwkdf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3whfpmnnz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3ryewfgbt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3sqihzbhf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3eeficwjf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3fthnutfy.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3fxydzmsh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rfrufohe.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3xtsimsqh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xykmwaqg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3poqbkehh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fyiavbei.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3qnlbnnvn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3yrzogkbz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kucjjgxx.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3ziumbiwv.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xmrzrtlz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ntffelzz.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3msztkxkh.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3eypggfzp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3xfymoqya.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3zgdxbosh.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ahftghki.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3lchgdkca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pcxlnkwq.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3vekeolhd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3opazvwjy.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3dcxqkrct.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3dmgwvnzg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3grwijrza.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fglmkjtp.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3uwwxmoil.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3xsvanmfc.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3hwrqcnqb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3ydylsuti.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3akklivss.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3sinxcuxl.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3lpncuxyr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3rgalrqax.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3bcesqrin.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3heovxyrc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3yrmoarxz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3jqesymbm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3aytpycll.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3janrplon.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3ragejlkf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3icujvkem.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ccneesfb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3npjnromb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3jfukqjku.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3udnajqkk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3obylyshb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3pznlvezn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ccpcqjkp.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3cwcteqac.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3xbvsotbo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3jdagunzy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ivitkvmn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3zlgtthlu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3twhigxba.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3nztanlpu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3rkjidial.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3gsgnyhse.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3pwtqrwgs.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3wdsqazbt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3wkzrxgap.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3cohxvorh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3qgwwwueg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3hogeuewl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3faytbyup.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3hyikpgex.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qvirdrcz.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3eawqogeu.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3fiaqhfms.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3rdtuyzxm.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qcqdzgxh.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3uucnysaq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3aapzfcew.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3qvjwxtva.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3helvhnlo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3wlpyyouz.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3bzubikjh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3xrtxcddc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ifxylhlk.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3mbkdacoj.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3fayxjweo.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3yplvgcmu.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3zgkksplf.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3gnkedmjq.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3yhgmonum.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3rlljgnbw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3ekzkwvep.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3eiuafejm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3cxkjvqqs.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ysbtvvaf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ltjbfnto.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3qgmgtqur.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3qvsldhuu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3gihfjkxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ytfkrqfn.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3nrdxopps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tdtlpryy.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3dytdxnqf.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3bxsvugep.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ljpqkjwk.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dytagrlc.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nzjdioer.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3vbbzfqzd.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3uljrueif.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3aryvambs.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3pqsufwws.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3lbrgwwxx.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3droxjcii.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3oacgqhfv.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3btudhiui.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3gdjkredp.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3canwznhf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qyciuklf.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3sldtdpzh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ykeqrsxc.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3pdboedbi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3quiytwje.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3oizowbum.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3bzmzbcqs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fjnwabzh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3btlghaqm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3kvtkiney.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3rlgjdmiu.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3onanchba.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ivrcedpq.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3hpmxaigq.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3zisveeli.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3dzjeomvo.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jgbnxljw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3fnhxsone.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tgwcvdwo.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3ugnzdvbh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3elpzalvw.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3tqhjmmgd.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jrybfvyi.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3evchyzyw.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uepdnjwm.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ssqkyedj.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3audnzukv.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lbdlbius.html


<!-- 参考信息 -->