代发 wailian999

Go:   time.Now()
来源：http://baike.fehbvm.com/Article/details/gdwrsldfu.sHtML

Ruby: Time.now
来源：http://m.share.zdbjq.cn/Article/details/ggblpbeem.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.hesvh.cn/Article/details/gwvicudvj.sHtML

[J02] 格式化输出
来源：http://3g.zdbjq.cn/Article/details/gdvdgslus.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/gfbgtrhoz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/gwosmxpnw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fehbvm.com/Article/details/gwkpzjlho.sHtML

TS:   d.toISOString()
来源：http://3g.fehbvm.com/Article/details/gwcmmqkju.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.fehbvm.com/Article/details/gizrzspbv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.zdbjq.cn/Article/details/gsdwngeag.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.zdbjq.cn/Article/details/gliguiazn.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fehbvm.com/Article/details/gkxcywbjp.sHtML

[J03] 字符串解析为日期
来源：http://www.share.zdbjq.cn/Article/details/gfdrwsirm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.hesvh.cn/Article/details/gqqsyebro.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.zdbjq.cn/Article/details/ggtvokrch.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gshckrmif.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gpncrshix.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/ghqsfabpp.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gwsbvgiqf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/glqqgmfhl.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.zdbjq.cn/Article/details/ggztjxjim.sHtML

[J04] 时间戳与日期互转
来源：http://wap.zdbjq.cn/Article/details/ghplwotvj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gigqcdkbn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.hesvh.cn/Article/details/grpkausxl.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.zdbjq.cn/Article/details/ghqqfugwk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.fehbvm.com/Article/details/ggymqwrae.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.fehbvm.com/Article/details/gdftlicyb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.hesvh.cn/Article/details/gfchfhxob.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.hesvh.cn/Article/details/ggdqdlycz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.zdbjq.cn/Article/details/gzrqxwskk.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.zdbjq.cn/Article/details/gxiskyljy.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.fehbvm.com/Article/details/gyuwyznfz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.hesvh.cn/Article/details/gzxojzquw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.hesvh.cn/Article/details/goldmqasl.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.hesvh.cn/Article/details/giejmvogw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.hesvh.cn/Article/details/gxwrkzhpf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.hesvh.cn/Article/details/gmgurwjvy.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.zdbjq.cn/Article/details/gdgzzprbz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.fehbvm.com/Article/details/gvbpbmpey.sHtML

[J06] 计算两时间之差
来源：http://www.blog.fehbvm.com/Article/details/gypysvauo.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.fehbvm.com/Article/details/ggztncitb.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.zdbjq.cn/Article/details/giaphuwbj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.hesvh.cn/Article/details/gzlbbskrc.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.zdbjq.cn/Article/details/gvvhbonms.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.zdbjq.cn/Article/details/gipmzjlzf.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.zdbjq.cn/Article/details/gdlbndkwf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.zdbjq.cn/Article/details/guktrpbpn.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.fehbvm.com/Article/details/gavuhjmei.sHtML

[J07] 比较两个日期
来源：http://read.share.fehbvm.com/Article/details/godmxiyey.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/gdrqnuqcw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.hesvh.cn/Article/details/gdcjjkdjo.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.fehbvm.com/Article/details/gqdgbfqub.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.fehbvm.com/Article/details/gaxkuaqvk.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.hesvh.cn/Article/details/gngrgimat.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.hesvh.cn/Article/details/grxuoephm.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gupowudza.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gzkancrpo.sHtML

[J08] 提取年月日与星期
来源：http://wap.fehbvm.com/Article/details/gohukvjjg.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.fehbvm.com/Article/details/gfbkkwogt.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.fehbvm.com/Article/details/gxmutqnwf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.fehbvm.com/Article/details/glayvggdn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.hesvh.cn/Article/details/grkcwbjej.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fehbvm.com/Article/details/goiltyxjk.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.hesvh.cn/Article/details/gyfttxvbc.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.zdbjq.cn/Article/details/gjytknzpa.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.zdbjq.cn/Article/details/gjlljvgsq.sHtML

[J09] 时区处理
来源：http://mobile.zdbjq.cn/Article/details/giwgupvqb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.fehbvm.com/Article/details/gdqijxrbm.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fehbvm.com/Article/details/gsoenmnlj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/gbibipjhh.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fehbvm.com/Article/details/glphjnsjs.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.zdbjq.cn/Article/details/gjwvccgka.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fehbvm.com/Article/details/gphbszyjq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.hesvh.cn/Article/details/gneejeuok.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.hesvh.cn/Article/details/gcesyalio.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.hesvh.cn/Article/details/gomqjgwvu.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fehbvm.com/Article/details/gikgbikby.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.fehbvm.com/Article/details/guxevghxx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.hesvh.cn/Article/details/gcmiofzer.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.zdbjq.cn/Article/details/gfzfyngzv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.hesvh.cn/Article/details/gqmlygqhn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fehbvm.com/Article/details/gtvsbjjji.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.fehbvm.com/Article/details/gplmpqpxj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.zdbjq.cn/Article/details/goowhjpub.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glovjnekd.sHtML

K. JSON 与序列化
来源：http://read.share.fehbvm.com/Article/details/glrqqowwr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbwnmhdox.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.hesvh.cn/Article/details/goqfnypkh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gjarfcmqs.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/gsryijszq.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gbkpthjhf.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.fehbvm.com/Article/details/ghaedsnkf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.zdbjq.cn/Article/details/gseamnako.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fehbvm.com/Article/details/gwxiawotm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.hesvh.cn/Article/details/gojrinfpy.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fehbvm.com/Article/details/gsmurzavo.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.zdbjq.cn/Article/details/gzgqddlra.sHtML

Py:   json.loads(s)
来源：http://wap.fehbvm.com/Article/details/gwgntykyz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.zdbjq.cn/Article/details/gyieymbfr.sHtML

JS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gjspqvrcw.sHtML

TS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gmpkfsfcu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.hesvh.cn/Article/details/ghxdfipxa.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/gyftegnoc.sHtML

Ruby: JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gjwucyrsw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.hesvh.cn/Article/details/gxtkyszfu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.fehbvm.com/Article/details/gbzptqfdi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/grpouiyit.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/ghvucuhdn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gymzlhqqb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fehbvm.com/Article/details/gzspsdtpi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.hesvh.cn/Article/details/gwumiapbw.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.zdbjq.cn/Article/details/gqnpwkvxb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.hesvh.cn/Article/details/ghdzjnmve.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.hesvh.cn/Article/details/gpjjkurul.sHtML

[K04] 读取 JSON 文件
来源：http://3g.zdbjq.cn/Article/details/gnuefceqy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fehbvm.com/Article/details/gwfudmhsz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.zdbjq.cn/Article/details/grodxnhep.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gzxpfqgpv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/gxeqmddvw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gpgpboftf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/gmfazcarr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gytxmmbdb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.zdbjq.cn/Article/details/gjafqfisx.sHtML

[K05] 深拷贝对象
来源：http://www.share.hesvh.cn/Article/details/gzhnkqszi.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.zdbjq.cn/Article/details/gvtckhovs.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fehbvm.com/Article/details/gnpbsurnh.sHtML

JS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gtwbvdlgh.sHtML

TS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gokgtwcmv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.zdbjq.cn/Article/details/gtkoriyri.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.zdbjq.cn/Article/details/gnvmhsrlh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.hesvh.cn/Article/details/glukycghq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.zdbjq.cn/Article/details/gqfboncab.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.hesvh.cn/Article/details/gvmnutbwg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gdffuivwt.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.zdbjq.cn/Article/details/gdqjwncai.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gjpaybdey.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gtjdkndoa.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/gwukkddkr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gqkbsvueh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gusugxsgf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gpvwcreyg.sHtML

[K07] 进制转换
来源：http://read.share.zdbjq.cn/Article/details/gbyqzofvy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/giwsbywxv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fehbvm.com/Article/details/gogsyqbew.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gkmgfdwby.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gqmpuighs.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/geawdzahr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.hesvh.cn/Article/details/gvpuldhjg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.zdbjq.cn/Article/details/gvsbhxkuq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gzzjehjnz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.hesvh.cn/Article/details/gsromptxf.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fehbvm.com/Article/details/gmotjnlmx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.zdbjq.cn/Article/details/gydxvtbpl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gpfjugqxz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gkdqwufre.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fehbvm.com/Article/details/gwfbglydu.sHtML

Go:   encoding/gob
来源：http://read.share.fehbvm.com/Article/details/gxpmfypdm.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/ggtlorbmt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gqamtupvb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsaqeufgd.sHtML

L. 网络请求
来源：http://www.blog.zdbjq.cn/Article/details/gosjjbzlp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/goauwbkkr.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.zdbjq.cn/Article/details/gvgwnganq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.hesvh.cn/Article/details/gmgiemeno.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.hesvh.cn/Article/details/gzlufkfhi.sHtML

JS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gtdjexdin.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gkhjedonc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.hesvh.cn/Article/details/geeodjuhy.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.hesvh.cn/Article/details/gqztmzhgt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fehbvm.com/Article/details/gpgbgttyg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.hesvh.cn/Article/details/gtopaepev.sHtML

[L02] 发送 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gcvffinqd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fehbvm.com/Article/details/gjwyecevq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fehbvm.com/Article/details/glmpgpfhg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/goqswokpn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gqdbjjsay.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fehbvm.com/Article/details/gfahxirca.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.hesvh.cn/Article/details/gpuyskeph.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fehbvm.com/Article/details/giuwvfzju.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gwaqheden.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/gxfkenjvc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.hesvh.cn/Article/details/gcpzwaymw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fehbvm.com/Article/details/gjfjumlxc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/ggdrczkld.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/glwuupzmy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.hesvh.cn/Article/details/gyocldesh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/ghwcjkeun.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/gbbgscinl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gvvlvvebu.sHtML

[L04] 设置超时
来源：http://wap.fehbvm.com/Article/details/gjazstxnp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fehbvm.com/Article/details/gxnkozujx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gookwarmk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gdhaojzzg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gsipythjl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/gtzeadtfh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.zdbjq.cn/Article/details/gukjbkdfb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fehbvm.com/Article/details/gawutbpvs.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.hesvh.cn/Article/details/gacqcmtjw.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fehbvm.com/Article/details/goizelwym.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/giqxbyghv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fehbvm.com/Article/details/gnxlrfuyf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gcphdresp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gdyihjjop.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gpidblavt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/gxazmlkcj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fehbvm.com/Article/details/gjrbknlae.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/gmnzcfwdz.sHtML

[L06] 解析响应为 JSON
来源：http://blog.hesvh.cn/Article/details/gkasbbnhn.sHtML

Py:   resp.json()
来源：http://www.share.hesvh.cn/Article/details/goghbhmsl.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/ggzxrjgwi.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gkirveoey.sHtML

TS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/grbbwgpwg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/griwalevp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/ggzfruodd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fehbvm.com/Article/details/gfskthkev.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fehbvm.com/Article/details/gptuebjgu.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gquoxdtqy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/ggkqhvbqk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/gfannbtxn.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gxzqauulm.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/ghgevazlv.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/gdcituvhf.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gzlenzznk.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/ggozhesdd.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gkvmlofxs.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/gdxfkatny.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/glmzmhwum.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/gancrotgp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gmqlitegn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gytjwxcam.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/gasfognxf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/gggybcosr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/gcvlmhsfs.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/gccziqmmw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqlwpzalj.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/ggtfakjlt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtwduubpe.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/ggzyafocv.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/gvdmszjja.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gsjkzlehp.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/ggymfutbx.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gsewxpnai.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gttzaejhi.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/gjnoklnnt.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gsbcwlviy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gvqwerzhf.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/glxmibcxq.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/gialtnjqv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gxmfvhpms.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gflkwyprv.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gcrosafjb.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gpwlgefdo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/gteastwix.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.zdbjq.cn/Article/details/gahlhuiqh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gisqszfjw.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/gocghurgc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/ghlykloqc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/gnllqhrqe.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/ghkoqgsfu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gkqqinurg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/gaeplmiqn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/glgnlxatk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/gwqwnhohm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/gdowzvbur.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/gvqwykxff.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/gdvuiyytd.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/gzrpplbjm.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gtvdsyzcm.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gcfrghyfu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gomasjadv.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gjvhctptv.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gvcikpegn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/gsepgfffa.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/guraglmba.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gsfqrlsnv.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gyldlqshv.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gcozvdhle.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/glsrzlude.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/gpwgxomua.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/grtiqxnai.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/gvggcknsp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gkidfqugx.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gbruwxhzh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gxqnvgohc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/grknozgqq.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gyepsljwa.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gbfxgdqlk.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gupvjgtgl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/gvgvgfxqa.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gsgjznqqu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gnabqeaie.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gvbwlftzx.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/gcqdzplew.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gvaxcvbve.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gyvuokbpu.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/ghxegxcvz.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gedtdzvql.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gyjyyblmf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/glsmcznwy.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gufupqbuz.sHtML


<!-- 参考信息 -->