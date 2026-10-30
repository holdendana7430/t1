代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fehbvm.com/Article/details/gtyrlapwm.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.hesvh.cn/Article/details/gserbhlac.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.fehbvm.com/Article/details/gnhmwsdlb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gebbhbtux.sHtML

J. 日期与时间
来源：http://read.share.fehbvm.com/Article/details/gsdlprzhw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gofrnvmrs.sHtML

[J01] 获取当前时间
来源：http://baike.fehbvm.com/Article/details/gnapdniyn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.fehbvm.com/Article/details/gmpotbgxk.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fehbvm.com/Article/details/gjczctuov.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.fehbvm.com/Article/details/gpsugagla.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gdaklmjfy.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.zdbjq.cn/Article/details/grjrjxgno.sHtML

Go:   time.Now()
来源：http://baike.fehbvm.com/Article/details/gzdisseyu.sHtML

Ruby: Time.now
来源：http://www.m.share.zdbjq.cn/Article/details/gwzhfhwzp.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fehbvm.com/Article/details/gmmdbxxup.sHtML

[J02] 格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gzaotovih.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fehbvm.com/Article/details/gteylbbfb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.fehbvm.com/Article/details/gzdbjrfss.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.fehbvm.com/Article/details/gmbrcuggv.sHtML

TS:   d.toISOString()
来源：http://www.blog.fehbvm.com/Article/details/gutiaemcq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.hesvh.cn/Article/details/gciebxsvg.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.zdbjq.cn/Article/details/gtimqahbw.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.zdbjq.cn/Article/details/gysdabdnd.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.zdbjq.cn/Article/details/gmlzgkfbb.sHtML

[J03] 字符串解析为日期
来源：http://3g.hesvh.cn/Article/details/guexgkgjm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.fehbvm.com/Article/details/gqaxrxyfa.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.fehbvm.com/Article/details/gnnuxsjtz.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gzsmlislz.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gzytqhvxi.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gwcpjmxwi.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gtupqbxeb.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/grsxkksab.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.zdbjq.cn/Article/details/gcdgvexud.sHtML

[J04] 时间戳与日期互转
来源：http://baike.hesvh.cn/Article/details/gstupttxf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.fehbvm.com/Article/details/gdnobebdh.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.fehbvm.com/Article/details/gzhbfufnq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.hesvh.cn/Article/details/gusbkfknc.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.fehbvm.com/Article/details/gysxwmome.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.zdbjq.cn/Article/details/gbpxlknnz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.hesvh.cn/Article/details/gdsaayndg.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.fehbvm.com/Article/details/glhfiedcb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.hesvh.cn/Article/details/ghhxwzozr.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.hesvh.cn/Article/details/glnbtgsze.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.hesvh.cn/Article/details/gdyxbqysz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.zdbjq.cn/Article/details/gjopopeiy.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.zdbjq.cn/Article/details/gtfysqqrs.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fehbvm.com/Article/details/gjvrpzcmj.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.fehbvm.com/Article/details/ggncxqrtg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.hesvh.cn/Article/details/gxxevmxiw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fehbvm.com/Article/details/gfgplhbap.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.zdbjq.cn/Article/details/gckpxxnwi.sHtML

[J06] 计算两时间之差
来源：http://www.blog.fehbvm.com/Article/details/glueitlut.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.hesvh.cn/Article/details/gxgngpiia.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.hesvh.cn/Article/details/goacavkcm.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.hesvh.cn/Article/details/gfcroxory.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.hesvh.cn/Article/details/gnfbeqmvs.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.hesvh.cn/Article/details/gpdxpctcw.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.hesvh.cn/Article/details/gxshmbith.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.fehbvm.com/Article/details/ghuclohuj.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.zdbjq.cn/Article/details/galveohcn.sHtML

[J07] 比较两个日期
来源：http://3g.fehbvm.com/Article/details/gqzlxapoh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/gquclhhhn.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.fehbvm.com/Article/details/gwxialshk.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.fehbvm.com/Article/details/gugtmbofz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.hesvh.cn/Article/details/gfczfejfo.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.zdbjq.cn/Article/details/gjjhomrlq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.fehbvm.com/Article/details/gyodttmdh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/gpixyhvab.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/glvuqwnon.sHtML

[J08] 提取年月日与星期
来源：http://3g.fehbvm.com/Article/details/ggpajdyzq.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.fehbvm.com/Article/details/gdeyejkdj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.zdbjq.cn/Article/details/gtwfqygxi.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.zdbjq.cn/Article/details/gcbmojlyy.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.fehbvm.com/Article/details/ggktmaood.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.hesvh.cn/Article/details/gtkygrjwx.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.fehbvm.com/Article/details/guyzcjvjw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.fehbvm.com/Article/details/guylkmwzv.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.zdbjq.cn/Article/details/gtsqbvzdm.sHtML

[J09] 时区处理
来源：http://www.blog.fehbvm.com/Article/details/gknlcfqsq.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.zdbjq.cn/Article/details/ghjlvigra.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fehbvm.com/Article/details/gyfbpovme.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/gpunnewth.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/ggzcdeazb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fehbvm.com/Article/details/ghzdmisol.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fehbvm.com/Article/details/gfvhuardw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fehbvm.com/Article/details/gkuepyiep.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fehbvm.com/Article/details/gawfcgmeg.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fehbvm.com/Article/details/gtuwccxgb.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.zdbjq.cn/Article/details/gzqsbyhtu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.hesvh.cn/Article/details/gvunvilvq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.zdbjq.cn/Article/details/grvcazebj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/goeibfnol.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fehbvm.com/Article/details/guptoycst.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.zdbjq.cn/Article/details/gzbjleqyf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.hesvh.cn/Article/details/gnlnxvues.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.fehbvm.com/Article/details/gwtupzybu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzsjachhb.sHtML

K. JSON 与序列化
来源：http://3g.fehbvm.com/Article/details/gfcblkxwr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gptydltyv.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.hesvh.cn/Article/details/gmqvtwzmp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/gknsemlcv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/ggpzfxivz.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gqsixtybf.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gcxvbqigr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.zdbjq.cn/Article/details/gqlovvxqp.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fehbvm.com/Article/details/gbjelrtzi.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.zdbjq.cn/Article/details/gwkjaikkd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fehbvm.com/Article/details/gpfrldeeu.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.hesvh.cn/Article/details/gwuiqgeka.sHtML

Py:   json.loads(s)
来源：http://3g.hesvh.cn/Article/details/gylyyfkvf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.hesvh.cn/Article/details/gspjoeydb.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gpggqsbet.sHtML

TS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gunqwuinf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fehbvm.com/Article/details/ghbgcxorw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gweissyog.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/ggulkklnx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.hesvh.cn/Article/details/gpjinyngc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.hesvh.cn/Article/details/gyynezxvt.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gdyvzlqou.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.zdbjq.cn/Article/details/guwoeixvw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/gzipjqssh.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/guzfmuxrk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.hesvh.cn/Article/details/gyiifnflj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fehbvm.com/Article/details/gylzmzawt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.hesvh.cn/Article/details/gkxfvywqr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fehbvm.com/Article/details/gzqwhctfa.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.hesvh.cn/Article/details/gibfwfrat.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.zdbjq.cn/Article/details/gnazrmdml.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fehbvm.com/Article/details/gznxqndou.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/glncetxor.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gpclmwwfu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gdpbuzmsl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/gtawfmlbz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.hesvh.cn/Article/details/gezypjfxk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fehbvm.com/Article/details/gtyheluou.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.zdbjq.cn/Article/details/gpimsbgrb.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.hesvh.cn/Article/details/gfowpqxer.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fehbvm.com/Article/details/gngjvhxfe.sHtML

JS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/geuykhpep.sHtML

TS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gkfcekpjq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.zdbjq.cn/Article/details/ggsekrfbm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.fehbvm.com/Article/details/gtstmnyvv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fehbvm.com/Article/details/gigdwgagl.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.hesvh.cn/Article/details/gcfbbpucj.sHtML

[K06] 解析 URL 查询串
来源：http://blog.hesvh.cn/Article/details/gdzpkkzvy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gyxwkchae.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.hesvh.cn/Article/details/gjphknsxv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gwawthzav.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/geyunvcrv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.zdbjq.cn/Article/details/giogohxxr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/ggfxbdtwl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/goenhdtsi.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gkmyalhpx.sHtML

[K07] 进制转换
来源：http://wap.zdbjq.cn/Article/details/gglsnavmm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gcmqjkpek.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fehbvm.com/Article/details/gxlplblfn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/guklfcgkj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gkuqiporg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/ggsvcnewh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fehbvm.com/Article/details/gusvhdzhv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.hesvh.cn/Article/details/gawzlzscg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gjtmcwnch.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/gqdeuownq.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.zdbjq.cn/Article/details/gywibuoat.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.zdbjq.cn/Article/details/gskcpwddo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gqyyhovvm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gotdlpbxq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.zdbjq.cn/Article/details/gnpiizfwx.sHtML

Go:   encoding/gob
来源：http://www.m.share.hesvh.cn/Article/details/gujbtetvo.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.zdbjq.cn/Article/details/gevodackp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gbprjmecv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gijkffliz.sHtML

L. 网络请求
来源：http://www.m.share.zdbjq.cn/Article/details/gjnngdeoq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbanuihet.sHtML

[L01] 发送 GET 请求
来源：http://3g.fehbvm.com/Article/details/gjmcwiixu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fehbvm.com/Article/details/gnvmbastu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/gncqdlrik.sHtML

JS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gxpcwuubx.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gtlmkbhyz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/gpxlgyfyz.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/guxjtexke.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.zdbjq.cn/Article/details/gfxyedhro.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.hesvh.cn/Article/details/gzrglwlze.sHtML

[L02] 发送 POST JSON
来源：http://baike.fehbvm.com/Article/details/gaffrizql.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.zdbjq.cn/Article/details/gsfaxvujo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fehbvm.com/Article/details/geuhwyqbw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/geqytevao.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gcwkwkycm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/gzobbymmi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.hesvh.cn/Article/details/gcrioxphh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fehbvm.com/Article/details/gtlxjbbpl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/guojzezfj.sHtML

[L03] 设置自定义请求头
来源：http://blog.fehbvm.com/Article/details/gkcmdvkne.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.zdbjq.cn/Article/details/gikxzjird.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.zdbjq.cn/Article/details/gndpjgwaq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gnucdxhth.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/govqsdjbr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/gonpnicbc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gxazepfay.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.zdbjq.cn/Article/details/gahcezzlb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gwjckwrnl.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gqitfchpo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/ghekwdbxv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gqucoicgy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gxoylaaye.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gtvqydvep.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.zdbjq.cn/Article/details/gqbqsgsip.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.zdbjq.cn/Article/details/gvrzhgzkv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.hesvh.cn/Article/details/gfgeicugg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.zdbjq.cn/Article/details/gbqtxnonl.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/gcwbodllv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fehbvm.com/Article/details/gadprtrby.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.hesvh.cn/Article/details/gqarzybwt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/ggtiwvcss.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gvytblsre.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.zdbjq.cn/Article/details/gmystzyzh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/ggefjaxwy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gdriwjljj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gpxfpanpc.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/giqodotbp.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/gzxcqdtkn.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/gqneuyuwq.sHtML

JS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gmkezryjn.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gttpgwxaw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/grptllmtb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.hesvh.cn/Article/details/gqiqhtnxd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/grywlwidb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/grgxpvqxz.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/giicsonsh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gsqtziwjk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gggchkhdm.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gaujqqwbx.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gvzjdjswp.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/ghhuzxamq.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gjpzrzffz.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fehbvm.com/Article/details/gvbyiaxjg.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gfxqzuwdv.sHtML

[L08] 并发请求多个地址
来源：http://3g.fehbvm.com/Article/details/grawtynut.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/gvamlabfm.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/guhytjqlx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gibjkjzqh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/ggaprssnr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gdsorwafp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/gdlcpfgvq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gsdyhepyu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/gwogpyzdb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggyjpgomn.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gndvpvrzk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvfacbggv.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/goaphcolt.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gpwsnslkp.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/gyevplzwi.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gxnbddaxy.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gqlacaabz.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/girhdkqzg.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/ghqeoqpfd.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/ggsecmfjy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gauyeqooq.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/glfasmths.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/gfruedvee.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gwoeitdcf.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gwxjmpejd.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gotsnqbyu.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/glqbodgzl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gjuvhwckm.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/gvxthyjpk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/ginlixjzn.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gygkxhbrz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/gvrggrorv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gteudtywf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/givmslvlj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gsxcyqfkr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gynykwspf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gbelexhqm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gjwoekyac.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/gbbkmfckd.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gnmrjwraa.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/grjkpcphv.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gfgyawwdc.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gjdprpili.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gmpfndnwu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/gaiioshes.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gcnonulpp.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/gsqqveckx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/glbrnvuym.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/goczhqiht.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gppxcchnb.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gfrbdhduv.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gegsxbuqy.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gwcofynjy.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gbxvuqyjo.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gzrghdvng.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/gjcyvhhby.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/gmxhxnkyx.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gazwaytqd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gcoxzqqli.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gmuqjloro.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gjxxibkgy.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gawrvuwja.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/gmdbsoilm.sHtML


<!-- 参考信息 -->