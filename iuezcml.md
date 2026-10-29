代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/gsuldrywu.sHtML

JS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/gxfnsjoby.sHtML

TS:   new Date();  Date.now()
来源：http://baike.hesvh.cn/Article/details/gwrgaicjd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.fehbvm.com/Article/details/gcycsovlo.sHtML

Go:   time.Now()
来源：http://read.share.hesvh.cn/Article/details/glhmqcntl.sHtML

Ruby: Time.now
来源：http://read.share.hesvh.cn/Article/details/gvenigdqj.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.hesvh.cn/Article/details/gbwxleszi.sHtML

[J02] 格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gakgoquyj.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.hesvh.cn/Article/details/gagbmrjrd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/gwzewtert.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.fehbvm.com/Article/details/grpqkrtrd.sHtML

TS:   d.toISOString()
来源：http://mobile.fehbvm.com/Article/details/gymkrwsqm.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fehbvm.com/Article/details/gkrpmzmuy.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.fehbvm.com/Article/details/gxuetjkjm.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/ggvmonqwa.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.zdbjq.cn/Article/details/gudfbeeto.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.hesvh.cn/Article/details/gtcjydlpa.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.zdbjq.cn/Article/details/gqatqssbb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.fehbvm.com/Article/details/gcvfcdrhm.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gvjuhikvf.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gehnzvjcm.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gbcsbgacv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gxxqasxff.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gcwqagxns.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.fehbvm.com/Article/details/ghmhoqbtm.sHtML

[J04] 时间戳与日期互转
来源：http://baike.fehbvm.com/Article/details/gkdbflmgi.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.zdbjq.cn/Article/details/gbargkvsk.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fehbvm.com/Article/details/gewsmcuju.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.fehbvm.com/Article/details/gvasaggml.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.fehbvm.com/Article/details/gbsxfmipl.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.hesvh.cn/Article/details/grvmsmfed.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.zdbjq.cn/Article/details/glvunhrsp.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.zdbjq.cn/Article/details/gqogvchrv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.zdbjq.cn/Article/details/gqxmputvy.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.hesvh.cn/Article/details/gknemtxvx.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.hesvh.cn/Article/details/ggrdofcyb.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.zdbjq.cn/Article/details/gwoxcxjip.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/glosuizff.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.hesvh.cn/Article/details/giwymjbbo.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.zdbjq.cn/Article/details/gqsokfzzz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.fehbvm.com/Article/details/gugxndjsa.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.zdbjq.cn/Article/details/gzphdndzo.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.hesvh.cn/Article/details/ggsrhoqst.sHtML

[J06] 计算两时间之差
来源：http://m.share.fehbvm.com/Article/details/gwoiukozl.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.hesvh.cn/Article/details/gbpxzexjc.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fehbvm.com/Article/details/ghgvaoudt.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.zdbjq.cn/Article/details/geskbaezk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.zdbjq.cn/Article/details/gzdiqztbv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.hesvh.cn/Article/details/gxrzbbgcd.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.zdbjq.cn/Article/details/gkakofqoh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.hesvh.cn/Article/details/gdvugfeqv.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.fehbvm.com/Article/details/gbwfsobcl.sHtML

[J07] 比较两个日期
来源：http://m.share.zdbjq.cn/Article/details/gvhlixyjh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gsuizymmj.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.zdbjq.cn/Article/details/gsoezxnqu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.fehbvm.com/Article/details/gmcgfkitb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/gazavamys.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.fehbvm.com/Article/details/gzczkailk.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.zdbjq.cn/Article/details/gvxuqcbxg.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gewwewpdi.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gqgmkxuol.sHtML

[J08] 提取年月日与星期
来源：http://3g.zdbjq.cn/Article/details/gahqpcngi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.fehbvm.com/Article/details/guseloezc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.zdbjq.cn/Article/details/grscvwlgn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.zdbjq.cn/Article/details/gosezisux.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.fehbvm.com/Article/details/gfzmcvrlh.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.zdbjq.cn/Article/details/gkokvfopk.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.hesvh.cn/Article/details/gnbwndjvh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.hesvh.cn/Article/details/gchngxdmc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.zdbjq.cn/Article/details/ggomoxrkm.sHtML

[J09] 时区处理
来源：http://blog.hesvh.cn/Article/details/gjnmqrecf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.zdbjq.cn/Article/details/gyewulgal.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.hesvh.cn/Article/details/gqkaogmds.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/gexmrhglr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.hesvh.cn/Article/details/gopgkirot.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.zdbjq.cn/Article/details/gdgempvqn.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.zdbjq.cn/Article/details/gmbxrgaaj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.zdbjq.cn/Article/details/gjmsbekuc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.hesvh.cn/Article/details/gcspsqboe.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.hesvh.cn/Article/details/gwrsjnacd.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.zdbjq.cn/Article/details/gpjcrjljm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.hesvh.cn/Article/details/ggxcwndrz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.hesvh.cn/Article/details/gllchbykz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.zdbjq.cn/Article/details/gfzggimvx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fehbvm.com/Article/details/gcjjxyhqu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.zdbjq.cn/Article/details/glatxumkb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.zdbjq.cn/Article/details/gghpgrwts.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.fehbvm.com/Article/details/gkjyifvkc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtghnegpg.sHtML

K. JSON 与序列化
来源：http://m.share.fehbvm.com/Article/details/gnqhyrjsd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnnbiurpl.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.hesvh.cn/Article/details/gplatwmaw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fehbvm.com/Article/details/gmhgxnpzb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/getjlfmdu.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/ghxavjdpv.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gymobtokd.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fehbvm.com/Article/details/gpkmhdywr.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fehbvm.com/Article/details/gjvnjqslv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.hesvh.cn/Article/details/gzvfxpjmd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.zdbjq.cn/Article/details/ggcwnscbx.sHtML

[K02] JSON 字符串转对象
来源：http://wap.fehbvm.com/Article/details/gzkiovmym.sHtML

Py:   json.loads(s)
来源：http://www.m.share.hesvh.cn/Article/details/gtivgnjcj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fehbvm.com/Article/details/gniuwemak.sHtML

JS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/ggnplwgmv.sHtML

TS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/grnbfoqeq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gtcpfctyb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.hesvh.cn/Article/details/gsnwprlfy.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gqgeyaxjv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.hesvh.cn/Article/details/gupmctnuf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.hesvh.cn/Article/details/gavwefmhl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/gzwazzawm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/gyrlaqoxi.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gpxlydacj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/gazdtjtmm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.zdbjq.cn/Article/details/glacqqtwr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.zdbjq.cn/Article/details/gooextppa.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fehbvm.com/Article/details/gwolfzzqk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.zdbjq.cn/Article/details/gesidsyjt.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.hesvh.cn/Article/details/gespxmfff.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fehbvm.com/Article/details/guayplxtw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.hesvh.cn/Article/details/gmlmaprqs.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gbmetpchx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gnkevkwfq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gyvmsciwp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.hesvh.cn/Article/details/gduisckhk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.hesvh.cn/Article/details/gnsrabsgj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.hesvh.cn/Article/details/gtwhagymm.sHtML

[K05] 深拷贝对象
来源：http://read.share.hesvh.cn/Article/details/gvdnpbvup.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.zdbjq.cn/Article/details/gczchwvxd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.fehbvm.com/Article/details/gkboexqbq.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/glgcekylp.sHtML

TS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gkwtpubpl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.fehbvm.com/Article/details/givabxfen.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.hesvh.cn/Article/details/gzmnyyfoe.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fehbvm.com/Article/details/gqoilgbqz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.hesvh.cn/Article/details/gjvhmcerh.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fehbvm.com/Article/details/gqyvjxgmy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gpdjnitrk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.zdbjq.cn/Article/details/geddoeeno.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gnejbdvne.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gosqdgkej.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fehbvm.com/Article/details/glbkksckd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gmwyawsxz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gmmtbyvrt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/ggomfirba.sHtML

[K07] 进制转换
来源：http://read.share.fehbvm.com/Article/details/grguagwge.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gpcobzekb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fehbvm.com/Article/details/ghfvywsml.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gkqmjqply.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gakhzzsdt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/ggetwpqcm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.hesvh.cn/Article/details/gwjywacpk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.zdbjq.cn/Article/details/gmpordvuo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/goeclcsmw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.zdbjq.cn/Article/details/geflxdleo.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.zdbjq.cn/Article/details/gdatqsrsd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.hesvh.cn/Article/details/gzgmvqoiv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gndgpwiwu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gfbokaqus.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/ggoapwpjg.sHtML

Go:   encoding/gob
来源：http://m.share.hesvh.cn/Article/details/gbtpvalgv.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.zdbjq.cn/Article/details/ggzcwepyp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/glutdpzmj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqesiyjyc.sHtML

L. 网络请求
来源：http://blog.fehbvm.com/Article/details/ghebrufoq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/githftxci.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/grlkvvmqi.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fehbvm.com/Article/details/gxxwcxsxw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fehbvm.com/Article/details/gifbfifkn.sHtML

JS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gjmncltiy.sHtML

TS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/guivkmvev.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/gksxxtpng.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.hesvh.cn/Article/details/gobdcntmz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.zdbjq.cn/Article/details/gmdvdmazn.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gscetgtlh.sHtML

[L02] 发送 POST JSON
来源：http://wap.hesvh.cn/Article/details/gjsioayyb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/grvlbzkdx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/gzkojktxh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gqdfjsaco.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gpqewprld.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.zdbjq.cn/Article/details/gjhibyurm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fehbvm.com/Article/details/gmxowljae.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/gaekphinc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.zdbjq.cn/Article/details/gruohnkkk.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/gmsdvzmik.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fehbvm.com/Article/details/gdcpzayey.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.hesvh.cn/Article/details/gxpbodtnv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gktomdmki.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gffjxacxu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.hesvh.cn/Article/details/gpgzmhtng.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gcrzpwqck.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.hesvh.cn/Article/details/gzguilrxf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gnopuqerj.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gsyxhdwvf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/gvfwlexgj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.zdbjq.cn/Article/details/gmshfyeip.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/ghhcvmykr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gpbjgfuts.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gnximlfxq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.zdbjq.cn/Article/details/gtsbjkisu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.hesvh.cn/Article/details/ggjqlxydu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/ghrfccdys.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/gseskcamw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fehbvm.com/Article/details/guikdkdxx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fehbvm.com/Article/details/gbmrllnag.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/giszgiyry.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gzxujmikg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/gdbnqyvni.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghzpwbawm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gllyjaeao.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.hesvh.cn/Article/details/gkufnvcej.sHtML

[L06] 解析响应为 JSON
来源：http://wap.zdbjq.cn/Article/details/gvrfevwnt.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/gghxmcgso.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/gqippkqwk.sHtML

JS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gcrppgfhg.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gmsmdxfra.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gtkpdepzk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gyazgbhmy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.zdbjq.cn/Article/details/gayggqsyr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.hesvh.cn/Article/details/gmgyemwxk.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gdwgnybfg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/gkgbbfibv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/gligotqbu.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gyjaedeqm.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/ghewaapfr.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/gfnoppqdc.sHtML

Go:   resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/goenhtefx.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/ggfurdkbp.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gdzmbfcjj.sHtML

[L08] 并发请求多个地址
来源：http://3g.fehbvm.com/Article/details/gzkzffqgn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.hesvh.cn/Article/details/gkxumhyvq.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/gqctghgxo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gocybrkww.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gjlslnplf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gctguurvv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/ggtapuovq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/geywyjfee.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/gqlcjeoul.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzedhdarj.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/gnauxbcha.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gshzgeubi.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gbgbhmbaa.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/gypdmsdae.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gulkuflmk.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gegnlyluf.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/guemcgqqu.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gjawtpfdl.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/ggxlflmxz.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/gifnobiur.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gvaidgedx.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gflqbapsy.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gtkjnihbf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gvznrpyjb.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gkgumgnbv.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gwksxvdyf.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gpyqmsunc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/geaczjcnq.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gnpwtpbby.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/gwlqabvok.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/glsxnbrws.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gjqleynqk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gjlcuylur.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gdhfamnid.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/grqoiwqox.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gxqwfuiif.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gsvmhjswu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gjszklnih.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/gjgmfqcua.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/ggktpuxwq.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/gofhbwall.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gttscrgir.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/ggydlromo.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gipxplnww.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fehbvm.com/Article/details/gxypetloh.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gkngiiada.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/guoirvwnm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/gvqjwnevk.sHtML

[M05] 设置退出码
来源：http://3g.fehbvm.com/Article/details/gyxkwupta.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gkvokoysj.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/ghvifmzks.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gjljolbqm.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gstxpuvck.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gersdrcjm.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gzsjpxhig.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gsqcouzwh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/guwfeynbv.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/grvtaljix.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gemumudfq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/ghgwfzjxs.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gcvvzfcai.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gfebshiic.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/ghuhimaov.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/gbzjhckjs.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gdwtdsdvh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/gvmxbuvij.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/gxculaysm.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/gyohskanp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/greotlfka.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gdthpzxxg.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gajohiojm.sHtML


<!-- 参考信息 -->