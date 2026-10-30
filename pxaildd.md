代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/gtlbvuime.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.hesvh.cn/Article/details/gotmfimvl.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.hesvh.cn/Article/details/gvltdttvj.sHtML

TS:   d.toISOString()
来源：http://mobile.zdbjq.cn/Article/details/gjnqaujrg.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.zdbjq.cn/Article/details/gkhtnuwoo.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.zdbjq.cn/Article/details/ggdgegtmx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fehbvm.com/Article/details/guycwrtnb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fehbvm.com/Article/details/gmpkpivpl.sHtML

[J03] 字符串解析为日期
来源：http://mobile.hesvh.cn/Article/details/gqsowirjd.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.fehbvm.com/Article/details/gsvsihjkc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.hesvh.cn/Article/details/gspvolvpu.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gphhmeeye.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gpnjkgizy.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/ggiyunntv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/guljbcweq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gbkoqzvzx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.hesvh.cn/Article/details/gmedajtcy.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.fehbvm.com/Article/details/gkoswypso.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.fehbvm.com/Article/details/gvlfbsgke.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.hesvh.cn/Article/details/gbttpykxk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.fehbvm.com/Article/details/geudhliik.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.fehbvm.com/Article/details/guyfyqeht.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.zdbjq.cn/Article/details/gfvbqcfwl.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.fehbvm.com/Article/details/gbgipbbgc.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.fehbvm.com/Article/details/gitjnqfkp.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.hesvh.cn/Article/details/gzeextris.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.zdbjq.cn/Article/details/glfxdtmro.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.hesvh.cn/Article/details/gmwpemwus.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.fehbvm.com/Article/details/gnmnpiqwk.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fehbvm.com/Article/details/gqipcpktj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/gowyefipt.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.fehbvm.com/Article/details/giwfwwioc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.fehbvm.com/Article/details/glnnbwozi.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.hesvh.cn/Article/details/gqitrbcyv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.zdbjq.cn/Article/details/gsgofkxdf.sHtML

[J06] 计算两时间之差
来源：http://read.share.hesvh.cn/Article/details/gdzfubrbl.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.hesvh.cn/Article/details/gxidwdmpc.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.hesvh.cn/Article/details/gackpagcm.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.zdbjq.cn/Article/details/gpxafwycg.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.fehbvm.com/Article/details/gcsndsxfg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.hesvh.cn/Article/details/gwjhgzckg.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.fehbvm.com/Article/details/gdbtzdhze.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.hesvh.cn/Article/details/giiaydcvj.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.hesvh.cn/Article/details/gswkqlbgb.sHtML

[J07] 比较两个日期
来源：http://3g.fehbvm.com/Article/details/gakzqrmnb.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/ghnsojstg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.fehbvm.com/Article/details/gndpsgegw.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.fehbvm.com/Article/details/gfbweafjo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.hesvh.cn/Article/details/gekoeihgp.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.hesvh.cn/Article/details/gyrzsremw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.fehbvm.com/Article/details/gnnunkiis.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gwexbonqy.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/grwlnopej.sHtML

[J08] 提取年月日与星期
来源：http://baike.fehbvm.com/Article/details/gpwheywsf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.zdbjq.cn/Article/details/gjqblrdpd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.fehbvm.com/Article/details/gwypcveyv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.hesvh.cn/Article/details/gjmrasbds.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.zdbjq.cn/Article/details/gzedbeklj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.zdbjq.cn/Article/details/gnfizbxls.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.fehbvm.com/Article/details/gcvweuusn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.zdbjq.cn/Article/details/gmxlryzky.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.zdbjq.cn/Article/details/ggcqpemhr.sHtML

[J09] 时区处理
来源：http://www.m.share.fehbvm.com/Article/details/gmtgtcanz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.hesvh.cn/Article/details/gxslmoerj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fehbvm.com/Article/details/gprfapodl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gbybnylyd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fehbvm.com/Article/details/gjoqosqnq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.fehbvm.com/Article/details/gkwlzpmqn.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.zdbjq.cn/Article/details/grxxrwauo.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fehbvm.com/Article/details/gnrlhicah.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.zdbjq.cn/Article/details/gyqsjxpqs.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.zdbjq.cn/Article/details/gqrnuypyk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.fehbvm.com/Article/details/gwfkuzekg.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.fehbvm.com/Article/details/gkntuixhk.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.fehbvm.com/Article/details/grmopoawi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.hesvh.cn/Article/details/gttbbdyiu.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.zdbjq.cn/Article/details/gxtwltudz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.hesvh.cn/Article/details/ghpzsycnv.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.fehbvm.com/Article/details/gastrudpd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gaxiodsfz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gccampogw.sHtML

K. JSON 与序列化
来源：http://blog.zdbjq.cn/Article/details/guskrsene.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gliiszwij.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.zdbjq.cn/Article/details/gwlwmsqlo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/ggqnccslk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gohylwruu.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/gubowypde.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/ggfhkxies.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.zdbjq.cn/Article/details/gljjvylct.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.hesvh.cn/Article/details/grbxdhkqu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.hesvh.cn/Article/details/guhyvgkwz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fehbvm.com/Article/details/gvkjmzyam.sHtML

[K02] JSON 字符串转对象
来源：http://wap.fehbvm.com/Article/details/gjqklrenh.sHtML

Py:   json.loads(s)
来源：http://www.share.hesvh.cn/Article/details/gpzpqnskw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.zdbjq.cn/Article/details/gryjxgmaa.sHtML

JS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gkxsdftbk.sHtML

TS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/guudexqch.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/ghfjjhzoh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gkzdtirkc.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gonzckiif.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.zdbjq.cn/Article/details/gbjbnqhqn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.fehbvm.com/Article/details/gphvldozq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/gmxqqcdwq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.zdbjq.cn/Article/details/guseewcdl.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/gbwdnamiu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gbkklztsu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fehbvm.com/Article/details/gqaguqhwt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.zdbjq.cn/Article/details/goivgmshv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fehbvm.com/Article/details/gwmauduay.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.hesvh.cn/Article/details/gccdkerbd.sHtML

[K04] 读取 JSON 文件
来源：http://baike.zdbjq.cn/Article/details/gkpdfxrdo.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.zdbjq.cn/Article/details/gyedztfte.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.zdbjq.cn/Article/details/gjfymaixq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/ganlsraqo.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gwdinvapi.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gnwxzvnhl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/gdrrzqkhm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fehbvm.com/Article/details/gbinmeswq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fehbvm.com/Article/details/gcrwojizd.sHtML

[K05] 深拷贝对象
来源：http://m.share.zdbjq.cn/Article/details/gjcgjbldi.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fehbvm.com/Article/details/gynladxrt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.zdbjq.cn/Article/details/gmeqdsfij.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gucitljal.sHtML

TS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gbtyojeqz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fehbvm.com/Article/details/ggoreezsn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.zdbjq.cn/Article/details/gprxhlheh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.zdbjq.cn/Article/details/gdkikieli.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fehbvm.com/Article/details/gbrjzsqhe.sHtML

[K06] 解析 URL 查询串
来源：http://wap.hesvh.cn/Article/details/ghmqcshbm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.hesvh.cn/Article/details/gnqkajnim.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fehbvm.com/Article/details/ghtxttiah.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/ggldtgqpu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gaekbuxvn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.hesvh.cn/Article/details/gmfqjoxjd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gvfamagnf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/ghfcryfji.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gktjrutwy.sHtML

[K07] 进制转换
来源：http://3g.zdbjq.cn/Article/details/gkylqengy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gwmqbfkmg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/gvnuoknts.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gykjadiyd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/glmybdcns.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/glgnegeqv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.hesvh.cn/Article/details/gzuwyqhfl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.hesvh.cn/Article/details/gkacjctki.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/goytruizf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.hesvh.cn/Article/details/ggjxzsgnn.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.zdbjq.cn/Article/details/gfsktvvdt.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fehbvm.com/Article/details/gyplmrbxb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gbkpkypjt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gvkkzksyq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fehbvm.com/Article/details/gjkciuewr.sHtML

Go:   encoding/gob
来源：http://www.m.share.fehbvm.com/Article/details/gmjitarro.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fehbvm.com/Article/details/gfpehkmpn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gwfcpwful.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzpahxanl.sHtML

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/guvtumwha.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gycbsfxtc.sHtML

[L01] 发送 GET 请求
来源：http://3g.zdbjq.cn/Article/details/gnposgtjw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gcqpvjzlp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.hesvh.cn/Article/details/gqmhvnxes.sHtML

JS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gwvpkopxh.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gvmcogepb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.zdbjq.cn/Article/details/ggfbhmgka.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/ghnqcypkb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/ggboizdqc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.hesvh.cn/Article/details/gdvkbwktt.sHtML

[L02] 发送 POST JSON
来源：http://wap.hesvh.cn/Article/details/gvplxpuyk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/giycmyzmc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/gwusbenjd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/ghkxovekl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gqqwofhmb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.hesvh.cn/Article/details/guypuqyha.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.zdbjq.cn/Article/details/giveylxuv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.zdbjq.cn/Article/details/ggfetufzv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.zdbjq.cn/Article/details/gycezxbun.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fehbvm.com/Article/details/gjdmdbdph.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.zdbjq.cn/Article/details/glqjnjlvz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.hesvh.cn/Article/details/gmvknxrur.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gcsqyompm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gecjfodfk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.hesvh.cn/Article/details/gdbcubrwc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gqbriydxz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.zdbjq.cn/Article/details/gvmdfoaxp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gfkojfnpm.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gjvljdgny.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.hesvh.cn/Article/details/gsccdehvc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.zdbjq.cn/Article/details/giacunqgc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gdbviekjx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gxdflnjcy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/gkqkjelax.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.hesvh.cn/Article/details/gpewgkurs.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fehbvm.com/Article/details/gnzajfqhm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/gmcdodyeo.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.zdbjq.cn/Article/details/gixjqlfcm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gzaxonvtj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/glhmxwxvy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gdnifytxa.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gqgrbuhyf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fehbvm.com/Article/details/giclqwjvk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/ghaspjijz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/gfdrrohqh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gocxgdajs.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.zdbjq.cn/Article/details/glnjsqyge.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gafazeegn.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/gqdsuwnow.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gaqorzmpl.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/grgbmmvdd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gvbagaxkn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gdqhjiagn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/gupqsxdao.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fehbvm.com/Article/details/gdkphvweg.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/ggkqajrsy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gxlyqqvmz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fehbvm.com/Article/details/giyjonuby.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gokwyovsl.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gsjyelzgw.sHtML

Java: resp.statusCode()
来源：http://wap.fehbvm.com/Article/details/gcxrpfkpv.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gxqyturhf.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/gvymanxcu.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gbonmzvmt.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gokuwcjua.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fehbvm.com/Article/details/ghyhdjaje.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/gcebysodb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gbcfaticf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gsnkikrix.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/ggmznlvzp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/ggrjphpag.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/gfcuwkcof.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/gdsppbkws.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtdqdkgvw.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.hesvh.cn/Article/details/gbhxfgswh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gprfbqssk.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/glgqixmlp.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/gbzjataud.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/gmiwrxljo.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gksbuomul.sHtML

TS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gqdqezivg.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gfwwevrhq.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gmiatfppf.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/gsjgrrsxw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gekjewomu.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gaurzqygb.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gjjprwghs.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/ggcchrlik.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gnbbpzqpd.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gazikfhpt.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/giikbrupj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gjjpdyykc.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/ghxtezbyg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/gpthrvthh.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/glfvuougu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gtkjiwynm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gijbykpwo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gwfwxtxyx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gijeaidqc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gagrfmmpf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gzfdwbehl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/gmijwpphk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gxmqqcaoa.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/gzutbnaij.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gswypefgk.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/gaeofsipw.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gkhkztqaf.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/grnjlfihb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gunihcixq.sHtML

Go:   os.Getwd()
来源：http://m.share.hesvh.cn/Article/details/geugvzdmy.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gvblcanoc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/gzyojwure.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gwpoxafel.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/glcjsxeea.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gzwrvnbxa.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gwsyjhmcc.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gknpcqdho.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gvotanole.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/garvyadlw.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gwqvoavmg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/gsmqvswcw.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/gdtssynpl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gnshzxjrq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/guxcguubu.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gpdegzqrr.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gjbvxmlmk.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/guhtcipxy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/gpoaocgab.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/guqabwusm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gvxpcbabp.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/gqyegripa.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gidjwcwne.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gmyfjqlcl.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gjehsttjl.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gstmaavhb.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gbesmmqxc.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/glrlyfhym.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/ggynixjce.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/gwjrbguvv.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gnasyjvnr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gtikpkyld.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gypnljesa.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gavdbzmrm.sHtML


<!-- 参考信息 -->