代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3weuelrrk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3qwzsjkau.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3jqvhumag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sepkwrxk.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3gtekyemq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ptutzmpl.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3umhjoeoj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3cbzitjhr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3rfvqftey.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3woaktfjm.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3anroeuys.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3fjskbwlj.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3fzwfqitg.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3vnuqpmoj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3rhfmbrru.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3penjbhdg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3wypmxzas.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3cofqzisk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3ajmwfglz.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3advyyugl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3gxhudexq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3mjwvgylu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3cwjhjjuh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3knviahha.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3gvfvgtmw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3vrwnuagk.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3wsdvmaoo.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3jgehmabo.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wthsdbdx.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3azuynama.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ntrrtdgd.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3cudatodk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3ogkmliri.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3qfhmmxed.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3trljfjkt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3qiatjcsb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3skugwzep.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3nmvmlrlj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3tqsjxcui.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fcwskoov.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3xfillkxg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3fvklewyf.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3pdkvuwof.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3uhehyhyd.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3bnuvftvz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ebkttipp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3foppsyrb.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3ccgkanpa.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3tznjipap.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3avdxedxk.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3auuawesj.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3slkfavpy.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3jdrikhco.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3tbohwngo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3mmnahjnq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3uqtrjbid.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3fxxinxgx.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3qrfoyuyt.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3mrcektgl.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3lokmskoj.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3ympfmylw.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3qtszldaw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3npdibuqm.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3edrmulba.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3dkwefogd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3cpvqeyds.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3mrmrhvnv.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3scoacjee.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3bmeyqkzt.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3nyobzigk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3hxcfqsds.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3asixpgmj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3hybprbis.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3mqagaehf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3beaaljkw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3vccgubrt.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3uumehvag.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3tfcisbfk.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3osqflmag.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3nlxhoxgi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3antbsaal.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3eqdtqnte.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3cqbicidu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3lgejbeay.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3vbvchjbw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3bamcckfl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3eqbaculd.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3fqajydcl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3xfjcumfk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3igjzlstc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sonmtlyd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3fslvfvpo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3hnvidnrm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3fpbookac.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3vqwcjkst.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ecrybtls.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tfezsesa.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3jhfkjbty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jvngcxcx.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3phamjgdz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3ifkunafn.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wvmzxcdy.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mmvdqgtc.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3zmohnhus.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3kydsmddv.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ftphztez.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3zdkdlzsz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3hmqmdtyv.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3oviagiiw.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3jvtilhpe.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3rvqspvzj.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3onrkizup.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3prycbwvp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3dszjgcpj.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3gsoeqqpw.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ewuvpqbc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sbbeoqzl.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3iwoyoztl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3mdjwaovt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3kotzgxsm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iozfouuo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vditvqnn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3rvlnxcjj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3qalzydlq.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qdtjyfve.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3kwbtrsuv.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3wwkeyxcc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3wcdddvkg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3lbmshppp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3pncvyrku.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3qoeuvrjh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3hjenfffk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3gbzphkdi.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3juolycik.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3tzudbjaz.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3tcrzgusf.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3bxrkxwnr.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3lunqrepg.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3essikmxe.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3kstxmmwg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3meayrndz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3uptkaiiv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3jzmyrttf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3twdlvjgo.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3byavnsdp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3bxghhhqi.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3haetazks.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hfobaxov.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3legsbgwl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3dorcsfrg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3aqetxymc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3kpyyrnxj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3tbgairxm.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3ogeorkaj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vcprulaz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3lvazpedz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ceyojkrz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3soyunqhj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ltcitruj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3pdvvmasp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3myyubvfc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zadljfnn.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3jhyggaay.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3wixfvkgk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3gayeftyw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3sucvvtdi.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3qubkyitk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3dhpsvsco.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3vqbpggok.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vpbngqsx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3nzoxcuic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3spuiqdvr.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3qcakigqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wayzhoyy.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3uazwkzli.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3dndytmsl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3mkfbgndi.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3bwkovojg.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3vkgwbqaj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3zksjhpul.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3aoavhqrm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3whasfwfk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qvwlyykh.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3akiddnfz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3aukinpul.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3myuosuvt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ifsjgnsq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3dztefurr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3tyknviwm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ucepaskd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3opeqpgcz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3tedgplyp.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3hxgzjhzf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3dkzuolcp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3munhojye.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3laphputh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3fgqiyskd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3tlstenoq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3tqqzwkbx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3ksnhgina.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3focefhbm.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3neamjctt.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3hemrsfrn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3lkganpyd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3rztjletc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3homtfdto.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3uwariakc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3qskvurwf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3hirgdvct.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3yrgnoetx.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3cxbxbinj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3sotmoyod.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3albecgtd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3vrfgkbis.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ejjcuzhs.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3ovrtngjz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3lyoipvgr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3rtmjknjd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zcnsctjx.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3spoketrh.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mjmmbnpm.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3anjkbvwz.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zerpqabe.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xsltqtic.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3lapmibzt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3wgrlfwge.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3nzdirgue.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3wmiuxzzi.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vzeebfys.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3cjwmvvzr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3dsmxindm.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3zryqyzpw.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3owiqwqto.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3rrfisyxt.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3gnktpdew.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3pgygtcyc.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3okzvcpvj.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ohvownqu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3pluugasa.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3mptxgnxn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3pejwklwm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3eblkbdkr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3iumovauu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3aafssmcf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3inisyyia.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gwgewkkk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cwwdwaub.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3unhbzumh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cxzktypu.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3zxilmzox.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ryqhylab.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3txnbdheu.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pxnsyjxu.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3eqdtmlji.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3snwvvaqm.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3iwjpguky.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3lslgfnly.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3yeevtveb.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3bmblfmph.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3czsfvlel.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3exuwifde.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3jqditlyc.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3fetpuxhi.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hcbegkxi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gywrgepy.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3fkelkkol.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ztklnfng.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3ntpmejpa.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3uqkmyskv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3vzjraody.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nuiuktbr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lyxnevmc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3iyigjysx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3lgcdemtx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3fzhrklnm.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3kugtjjjy.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3psgspbyn.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lfbvsmhp.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3gnerwapf.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3bxdyzypc.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3nmecvfic.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3fabuwqdz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3hrzojtik.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3rihxrmmw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3kikrbtpq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3kvkcynbl.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kghnnuif.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3waxrzrrf.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3duguscbz.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kmnfkjdn.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wrfldowx.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zwrqdrnp.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3yddwivbh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3ebupbkew.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ejbxyzhf.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3kexnhklk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3bxhinabv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3aawizvpq.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ldcoqdhe.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3wewkboyd.html


<!-- 参考信息 -->