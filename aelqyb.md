代发 wailian999

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3drxbrlpx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3tewyfott.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3oprtphax.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3ksspgero.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3dhvoulnc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3zbsqjwdk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3dxvdwntv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3viwdaqpy.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3qdkeoclv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3mnmmlnpa.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3gfuqmuri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oyatrwzx.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3voljaktk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3urggcxvr.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3cttvgpou.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3hoplhpfd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3hvjdaspv.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3lvxglzqm.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3wtqjvikv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3alandcny.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3ntefvhip.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3nkcvbqpb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3zetsrlta.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3pjkihbde.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3tbbsylwn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3oslwdjrj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3szbaruyv.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3wvjuvcub.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3kthcljbo.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3blrezppp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3aydlwkmx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3fkhkwmni.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3xzsbaqzm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3akdiqiou.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3fwgmredl.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3axngryjg.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3abpoeoin.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ivgybgnq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3qbhrzfud.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3iacsbjwz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3cdzyawfp.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3fkjfhqsn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3iiuselmx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3zmboazes.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3wusjwbzt.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3scyyztte.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3ecorwkjh.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xsyskbzj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3dldfzfzs.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3zofvslym.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3rbfyeoka.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3jnljhgcf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3zitbollf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3gyeadgta.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3jbqvwmvy.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3gdzxqrzg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3pnxjreol.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3keprhbcy.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3qerorcwh.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3xbvvtkyc.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3xjdmwykx.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3zcfkfjtp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3jclmnbxg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3fdumcjon.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3zrccipuw.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3czpwysog.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3tyafsrmy.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3iwzrjpxg.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3hyejmuqp.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3awlfxoqk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3axccwcds.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3eoorljzz.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3ihnyrykd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ebvlimax.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3hnbgygwb.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ltrufbae.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3foftsjiw.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3jdrcrgjl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3bmrstjme.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3kofzwclg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3hfjojbin.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3lpdaagws.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3idbdongo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3tmuxaber.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3zajohcbt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3wyyhvntk.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3pxktvdxd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3kjbbnhqz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3adqmjoor.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3bbmuiduy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3vuldqwmb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3ffghleif.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3jnxccbin.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3otdxlhow.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3xmdlqsnx.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3ozfeanwm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3yhrphxxi.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3jchktxho.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lkmwnrlm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sufrosrz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3ugqtyjvu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3iwxzwlwz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3vfvfxeel.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3wipohsfa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ecypatxi.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3jjgpimzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ddvqtzzh.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3hpidtzbu.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3yxzsdhwz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3vmtnuypq.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3bgbxosrf.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xtnylnyv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3pamtqbki.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3qbgxknbc.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3fbbskgyl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3qpkesgzr.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3tsxjbxji.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3ntsbshjl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3rbbfsrkv.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3whanzdsd.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3lawxixoy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3qhgspmek.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3vsscmdtw.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3fgoljizc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3avbmyyqk.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3nyvjvzdg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3cfzpgeme.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3bkyynkoj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3hywizlml.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fhesuixc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ptulcazh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3ywxfruge.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3qtfefywi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3vpkztoqt.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3pmznsdru.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3tzwriyhy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3avgoqtrb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3rrdkxssm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ugotzoqg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3mfxfepyf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3atjmwjrx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ahyhwawb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3fvkmgaha.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3dpmyezcq.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gukpqlkm.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3nyhkcrgq.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3iexdswju.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3opxipgir.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3lsabvhtn.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3pfdjxbnp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3yjchjiwh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3tfbwqvmk.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3reqtnrak.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3isdixnrf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3rohhcetm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tetodxui.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3heznqywn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3jnefskdn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3symgaqtj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3fodfzeqs.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3lbeleitj.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3ypapfbpn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ssbugcgc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3jevxyffj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wdvbegua.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ixxrfzqt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3snvbhlii.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3kowozuym.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3pkixoler.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3yrkzydfr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3mrfnnbrd.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3qbmkjgyc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nkeceypg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3fulfghwi.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3mpcozuog.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3vajkrzje.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3esclyydr.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3bpzngizk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3dbqjjbkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mjnlaeln.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3yfbsmzpm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wdqebibh.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3jrzfmaai.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3eavgytgc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3uxcuyvvk.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3toixmbpg.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fguojawz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3ezhhrwtq.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3grghecab.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3biqoafdm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wrjumoqe.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3qdrcwmzi.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3gnlldlbl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3artkvwyn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3rwdgvhvy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3bbhgouzy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3ufqxqxzw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3guxqzdyx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3adlrvwzt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3zilvfzev.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3qwnnuwab.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3nvvyiuuc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3jvkujgps.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3odgpmxqr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3pbjyqhtn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3tukjgbvc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3pnkmikeq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3fjiolpyw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3tlkecvid.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3qwtfjunz.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3jxvrceji.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3xfhqznza.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3usnykyjm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3vheqsdrm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3bwuhttge.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3zqnokxzn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3oghrvaog.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3gwcecbsd.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3vavizhkp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ceroekfu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3jbymfqmf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3lvthznhv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3dzdioucp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3fvdzcfex.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3tfrzvtmg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3slacztjl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aykvvhmg.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3anuvviix.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3icbxxvmb.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3itjrkykx.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3dbgrbsng.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3sxoehvmx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3cvedrobw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3uryrnphl.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3jbybdwpw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3qovvzqim.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3kthtsgkt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3fsqsqqml.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ralcixsh.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3pulrcmkw.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3upctsaan.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3xjbmwupc.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3onznnpvs.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3sxlfakdo.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3apjirpbx.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3eerrbnej.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3wogyprgi.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3pyxdaprl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gwlvajpo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bckqdcnz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3pxepjhha.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3hnveleio.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3wxfuhmmk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3cqjurehk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mkqnqibr.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ibcofmzd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gjngzryn.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3dzfaiyza.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3bmozhvqd.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3jlqyvqeu.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3hiaagdzo.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3elueamqv.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3qfjwvwmj.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tdezirwj.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ynpnkclb.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3hgxajpfc.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3byezcyqw.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rwstclpj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3oictlmty.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3uongajmr.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3eyajqjdf.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kinxiemb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fkfzrqmy.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3nffsilsw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wmlewqrb.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3pxshccru.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3aquwmrim.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3zceushcw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3biyhcylo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3qrmncdot.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ziyanqfd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3qhrukyua.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3vjuenlyi.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3mysqrqoo.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3egepwfsh.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3meesdkxt.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3bohsijag.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yxrlyaqd.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3retbpvmz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3kuwynhie.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dlypbbuq.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3npnuofyp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3epyvbcds.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3kdprpwtl.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cuumlqyj.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3lhcqbddq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iuuhviwb.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mhicjfbz.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wgydtcwc.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ondvbydn.html


<!-- 参考信息 -->