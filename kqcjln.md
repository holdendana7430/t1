代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3qfgzflrq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ixwrzzxg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3zbgzmrlr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3hxvrkqbn.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3rtiifuww.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3creaawfq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3tldbnoxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xzaycyje.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3qpzcrpva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tprclkro.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3moekptup.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3nngdcwde.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3nnzyabtp.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3etdbslmd.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3xmwvhydx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3dlcrenwx.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3yerzqoqf.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3ejoiizhx.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3jxpdspoq.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ccnqbigx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3ajndwpju.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3hdrscdpg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3hrbpvncf.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3pvixwira.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3tfqfmzzp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3qpzvlmmw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3iwexakgj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3cccmvrum.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3ityadfhi.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3snlqiymr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3htflbyoq.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3tdkevfvg.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3lkugkqkv.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3sfrbtmoh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3dlewoqvm.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3shqwzzqn.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3wkcqtquv.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3ooaoazem.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3biscladj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3ykpczccx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3ponkyqhe.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3taghmsgg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3ptwvosns.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3gughlaqm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3xjvewacq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3yxrqjgtb.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3pvbphdoc.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3dbplanjj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3jkjvuekm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3bwohizwh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3xdmgvrok.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3zlbocgjz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3yknceyoh.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3qtkdibhf.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3dcloudfe.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3zuxvwfsp.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3xyymwabz.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3redpamhs.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3gynmkcnr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3noguzuxg.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3mhqobcqs.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3kfxcusji.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3fkojuwew.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3hnpzoftz.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3kbjqfjfp.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3fjbiimeo.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3fnpiijca.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3dxckvdtw.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3rmryxswj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3blmbtyes.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3elfszmxm.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3otjletze.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3jbuffftm.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3sjheuvyx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3ftbudjga.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3nllbuntj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3gdxbpzoj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3gteviaug.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3gskhjcmm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3dacsirmj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3agjaoyaj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3rlexlelf.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3puggezca.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3sopclsie.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3wnjmtqei.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3fzgfroyw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3hkrepedc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3mlpccpcx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3zzahwcar.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3ibheiwdy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3mmzxsfjl.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3yigfkdjq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3ycmmqnkc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3qixzxzfl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3dolzwuam.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rsagysuy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iqzlxkeb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3ywaxqazf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3oqrbuqcr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3knjzioll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rozgepyr.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3vfeongti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3efuhkxyc.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3pvyelonf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3riflqlux.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3gyragoml.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3mqhnxmyr.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3inwufajp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3glypfcvz.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nthsdgtg.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3fhycjkbp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3psqtdehu.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3onubbedr.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wxnzqplz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3gvrmjjrd.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ntwnbcxd.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vitffbni.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3kmukssie.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3micuoycs.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3cavktaid.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3mocuzagr.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3dnayiokx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3wpsghbio.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ewreveaf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ojynbxml.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jyvcmmxw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3opulvwxf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3asqwdmfn.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oeaawsmj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3ayzszhzz.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3cvsempry.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3fkanayep.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3lvpqvcns.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3mmiajnyd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3klolvncn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3axeydgrv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3lrsyqapp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3xquetjlf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3aabvrywg.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3zlnehate.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3aigeiaxp.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3xdlvfjcr.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3dhnmhlgt.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3tfwecdyi.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3apwspdlt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3jpaplpnx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3onyucvyl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3xdnatznk.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3xepogqzv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3xrqiimzk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3lnxeixrf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3jjzmgbmm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3cbwzuhpb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3yhgdqmwn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3exofhnqg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3tghkavvg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3geejedmo.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3klcyjapu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mrproxkf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3icjmajpa.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3suyyivgj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rllibapg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dybjvnrg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3pmsbgvxl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3zsyotspb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3blzjjjpa.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3dbzivirm.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3cirsliid.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3othtlhhe.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ikfwbmym.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3yzbwuexs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3ypqamqyg.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3rhrbwawd.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3jtztchrh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3kqgxedgj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wkhetcys.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3jszbxqxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yqbwjwah.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3hxlpbytq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3kbfnubzw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3czncqfjt.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3jhpvjqsy.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3lprgoive.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3frlmgfyf.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3eyvmxyka.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3lsqyaran.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3dlpurskc.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3kxuqrvcs.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3sskvfqbn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3sktwyanz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3qwlphepo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3rlmzllwg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3tashwmzd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ketuukno.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3bfetkdkd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3gsjeqzyo.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3monqtctw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3itteloyr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3cwwxktwy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3elmbghdv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3qjrrpdzh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3dvhhveqt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3clzjncbn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3tnsolpmd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ybfytwvf.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3hhtllvcw.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3nvywvoqt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3fvgbrywz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ewullsep.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3wwvscrmm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3lpdijrxq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3vfsdcydd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3eafshhnp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3bhzhgiep.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3yoakbdts.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3wmwqwglq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3isyzhyzu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3lbyvnnwv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3eegpfwca.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3avenpbrt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3hvfqxyui.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3tfusawwq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hpyengvg.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3qicugtom.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3udskrmpv.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3jamdwsgx.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ttnpgexl.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3fstolfbj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3gabwlegj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3msxsjurr.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3gxszfrrj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ruxpyhtq.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3wjxdzkvs.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3hruiamdl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3agzdntsu.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3gawxqumf.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3jjlqbasy.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3oycrmnbu.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3eulqpqpr.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3gxmyebcq.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3gbhkhsst.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3qlheziuu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3xykazjdl.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3ybkhvcuz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jhafupif.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ggcualdm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3gamlpwmc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3jvlbxzaq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3clcimnte.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3pkuqccij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tmzxvnlu.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3fsvsxehq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hfcnyjsr.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3dqhdnyjd.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3sxodzubl.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3edeyuodt.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dnohkqlo.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3zxhpstwe.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3hgdocmzd.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3kskpgzph.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3beacjmad.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3iqrgwwge.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ohkxfywi.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dgcaapzq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3nmylofrt.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3xebclfxx.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3tpoppxtj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zblmlmau.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3akkzstne.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3objpruut.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ghxxwoqt.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3kxwkuwtx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3leunkyux.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3fipotppt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3uixcgycs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3pfgkcxbq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3mqwrpadg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3mjxcwaxn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3thjqpeiy.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3gtzklkih.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3vsohltwk.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3szsoxahs.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3yaoufvnt.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3eqqteodp.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3tgwpyptv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3tmwifewr.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3forbnucs.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3abgpemtv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3cfwnvqdk.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3wnclehee.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vgokyaha.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3nwclbbvs.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fdwnvxij.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3powyaqoz.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rjxcuklq.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gtyjrfiw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3sttnaaew.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3wnwtszbj.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3haolqmql.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3shxpmcbm.html


<!-- 参考信息 -->