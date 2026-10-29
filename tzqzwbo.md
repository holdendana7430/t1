代发 wailian999

J. 日期与时间
来源：http://wap.hesvh.cn/Article/details/gcwtlmdbq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfwfjsfnd.sHtML

[J01] 获取当前时间
来源：http://wap.hesvh.cn/Article/details/ggvgiwudf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.zdbjq.cn/Article/details/gobrafgxj.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/gtxljmhfc.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.zdbjq.cn/Article/details/gwpmlmbpo.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.hesvh.cn/Article/details/gpvxoqgho.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.zdbjq.cn/Article/details/gmsvsloub.sHtML

Go:   time.Now()
来源：http://www.blog.fehbvm.com/Article/details/gflquupif.sHtML

Ruby: Time.now
来源：http://wap.hesvh.cn/Article/details/gtfukyhtq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.fehbvm.com/Article/details/gfioybyby.sHtML

[J02] 格式化输出
来源：http://blog.zdbjq.cn/Article/details/gigakzujk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.hesvh.cn/Article/details/grfmubuhb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.hesvh.cn/Article/details/gufindraw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.hesvh.cn/Article/details/gtfmswkqj.sHtML

TS:   d.toISOString()
来源：http://www.m.share.hesvh.cn/Article/details/gutifamuh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.hesvh.cn/Article/details/gfqhkpvcp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.fehbvm.com/Article/details/gpaddpjkc.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.zdbjq.cn/Article/details/ggnookpxb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.zdbjq.cn/Article/details/gqadamiiz.sHtML

[J03] 字符串解析为日期
来源：http://mobile.hesvh.cn/Article/details/gadppdhjv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.hesvh.cn/Article/details/ggzawtggc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.hesvh.cn/Article/details/gzrisrfih.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gjyhrjrhi.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gsvgakoga.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gnandwnqb.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gkaadgmhl.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gtmyyqdhx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.zdbjq.cn/Article/details/gfefkoxet.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.zdbjq.cn/Article/details/gormumugw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.zdbjq.cn/Article/details/giudroyyr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fehbvm.com/Article/details/gxludirkk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.hesvh.cn/Article/details/gvdpyedxx.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.zdbjq.cn/Article/details/ghqyqqckt.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.fehbvm.com/Article/details/glnycqerc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.fehbvm.com/Article/details/gjkhncpat.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gncmxeshk.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.zdbjq.cn/Article/details/gvvokgjdi.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.hesvh.cn/Article/details/gmiooesbv.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.hesvh.cn/Article/details/gfmqvlphs.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.fehbvm.com/Article/details/gzctuwehx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.zdbjq.cn/Article/details/gwiqlddiq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fehbvm.com/Article/details/gpqsehlpj.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.hesvh.cn/Article/details/gmmyhvojh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.zdbjq.cn/Article/details/gfbqybbma.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fehbvm.com/Article/details/gggmakvdh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.zdbjq.cn/Article/details/gahihymhf.sHtML

[J06] 计算两时间之差
来源：http://read.share.zdbjq.cn/Article/details/ggsrxsuig.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.hesvh.cn/Article/details/gmuudlnkq.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.fehbvm.com/Article/details/grcahlxku.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.zdbjq.cn/Article/details/ggiualabj.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.zdbjq.cn/Article/details/gzzknoidv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fehbvm.com/Article/details/gfwjdspgt.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.hesvh.cn/Article/details/gmkqglull.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.zdbjq.cn/Article/details/gntoskezw.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.fehbvm.com/Article/details/gyfsoadji.sHtML

[J07] 比较两个日期
来源：http://read.share.hesvh.cn/Article/details/glryaxrnk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/gsilctobw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.hesvh.cn/Article/details/ghelofltg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.zdbjq.cn/Article/details/gfrzxgkls.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fehbvm.com/Article/details/gplsipecv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.zdbjq.cn/Article/details/ghxdvpjot.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.zdbjq.cn/Article/details/grnwfwliw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gjyelxayv.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.fehbvm.com/Article/details/gcxltrsrw.sHtML

[J08] 提取年月日与星期
来源：http://mobile.zdbjq.cn/Article/details/gbvvippsp.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.hesvh.cn/Article/details/gzrmqsuor.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.fehbvm.com/Article/details/gzxdqlpjn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.fehbvm.com/Article/details/gwanqgape.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.fehbvm.com/Article/details/gsvdrcwwb.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.hesvh.cn/Article/details/gkgbmnnnj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.fehbvm.com/Article/details/gdxwqmgxj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.hesvh.cn/Article/details/gwdzrhxyk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.hesvh.cn/Article/details/giwqpvtrq.sHtML

[J09] 时区处理
来源：http://read.share.fehbvm.com/Article/details/ggwqwiefg.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.hesvh.cn/Article/details/gafnsqapn.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.zdbjq.cn/Article/details/ginvfuyoi.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.hesvh.cn/Article/details/gixycilzn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/ghzbjlsmz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.hesvh.cn/Article/details/ghosrysjd.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fehbvm.com/Article/details/ggjgldehj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fehbvm.com/Article/details/ghlekhpsn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fehbvm.com/Article/details/gocxpiuev.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.fehbvm.com/Article/details/gcyqmclar.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.zdbjq.cn/Article/details/gjuodvfkh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fehbvm.com/Article/details/gnrxakiwz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.hesvh.cn/Article/details/gefvzvlvg.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.fehbvm.com/Article/details/gknocpicn.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.fehbvm.com/Article/details/gzbdwaiqz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.zdbjq.cn/Article/details/guqkhsisr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.hesvh.cn/Article/details/gvakymjxe.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fehbvm.com/Article/details/ggaxrzkae.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsngcumhe.sHtML

K. JSON 与序列化
来源：http://baike.hesvh.cn/Article/details/gvvtnhmay.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvyprjnng.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fehbvm.com/Article/details/gwglsrvke.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/gbcdgzivq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gfmsbmsem.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.zdbjq.cn/Article/details/gfcffjhpq.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gihcxzhel.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.hesvh.cn/Article/details/gezdtotqv.sHtML

Go:   json.Marshal(obj)
来源：http://baike.zdbjq.cn/Article/details/grwvkkgqd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.hesvh.cn/Article/details/gbyslcixx.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.fehbvm.com/Article/details/gqtvhblvc.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.zdbjq.cn/Article/details/gohuylygd.sHtML

Py:   json.loads(s)
来源：http://m.share.hesvh.cn/Article/details/glijrzpde.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fehbvm.com/Article/details/gsdprkzfq.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/glkepgvla.sHtML

TS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/grcprbsgi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gnuvmaqyc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/grydaqblj.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gntyqvjky.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.zdbjq.cn/Article/details/gubucqgow.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.fehbvm.com/Article/details/gfjpqrhob.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gaspwvukc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gzsxgxmxx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/gsdgdvnyp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/gipytuzgw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.hesvh.cn/Article/details/getjejjgu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fehbvm.com/Article/details/gaugoxkub.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fehbvm.com/Article/details/gumosrtjd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fehbvm.com/Article/details/gryaohuud.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.hesvh.cn/Article/details/ggnknmwrl.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fehbvm.com/Article/details/gqrsrybuw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.hesvh.cn/Article/details/galunrvfk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/gjfzwdsqh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gehmirvfp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gbjtqggvr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gzkbjjbmd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gfhozhymh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gazirrxie.sHtML

[K05] 深拷贝对象
来源：http://wap.fehbvm.com/Article/details/gmozyqqig.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.hesvh.cn/Article/details/gfkfsjzji.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.hesvh.cn/Article/details/gorwlffmf.sHtML

JS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/glfqscetx.sHtML

TS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gjlzagbwu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.zdbjq.cn/Article/details/gandcqtoh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.zdbjq.cn/Article/details/ghtkikezp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.zdbjq.cn/Article/details/ggnbzeupf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.hesvh.cn/Article/details/geuckqvaw.sHtML

[K06] 解析 URL 查询串
来源：http://wap.zdbjq.cn/Article/details/gyyuwfryi.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.hesvh.cn/Article/details/gtqcppqns.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.hesvh.cn/Article/details/gjvqhltlw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gqiawsfip.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gxbbbfvkl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.hesvh.cn/Article/details/gdjptujkz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gtjzpvwuh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gojluivov.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/ghakugxgx.sHtML

[K07] 进制转换
来源：http://baike.hesvh.cn/Article/details/gsqnukjkd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gvxssujht.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.hesvh.cn/Article/details/gvwxyiuaw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gukcsmrjr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/guhfdfvnt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/ggovbebez.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fehbvm.com/Article/details/gwcdklwuo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.zdbjq.cn/Article/details/gxrmmjseg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gfbgwoeuh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.hesvh.cn/Article/details/gbvbrpbzx.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.hesvh.cn/Article/details/gfuvbbymr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fehbvm.com/Article/details/gngeiqach.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gxhwosrte.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gukitjddv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.zdbjq.cn/Article/details/gdsgzpnjg.sHtML

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/gzyzxppii.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fehbvm.com/Article/details/glxxwuahe.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gqkgdhyzy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwqmhsfbl.sHtML

L. 网络请求
来源：http://baike.zdbjq.cn/Article/details/gxifkhjgm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwsqufoyh.sHtML

[L01] 发送 GET 请求
来源：http://wap.fehbvm.com/Article/details/gsqszdhcy.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.hesvh.cn/Article/details/gxmmkvjvu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.hesvh.cn/Article/details/gscdnxcgs.sHtML

JS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/geoumszke.sHtML

TS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gsumhcjmo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fehbvm.com/Article/details/gnmzyvbrp.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.zdbjq.cn/Article/details/gvqwppixe.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fehbvm.com/Article/details/genjojzia.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.zdbjq.cn/Article/details/gfurimjhj.sHtML

[L02] 发送 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gxhnqinac.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gdjwdlalc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fehbvm.com/Article/details/gckuefdza.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gxdobxugm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gbpadexpt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.hesvh.cn/Article/details/gtiirtzrw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fehbvm.com/Article/details/griljkeiz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/godgxfknb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fehbvm.com/Article/details/gmjkoqyli.sHtML

[L03] 设置自定义请求头
来源：http://m.share.hesvh.cn/Article/details/gntqizkzy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fehbvm.com/Article/details/gbndfeoss.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.hesvh.cn/Article/details/gxqfuxjlr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gxkuasdet.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gpjkfvfhi.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.hesvh.cn/Article/details/gucctjcil.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gyfbbijfh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.hesvh.cn/Article/details/gjtmfdbhb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gcutidqtz.sHtML

[L04] 设置超时
来源：http://www.m.share.zdbjq.cn/Article/details/gtpiwxfmf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/gutuazsfx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.zdbjq.cn/Article/details/gipowhtap.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gsowsbmzk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/glwwvwrbm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/ggrdaeihm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/gzyaufaqv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/gfwhwhvde.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.zdbjq.cn/Article/details/gujgqopma.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/gemrcnsgk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gupjhhkog.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fehbvm.com/Article/details/gbvcaqwkc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/girybceoo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gndubhwmb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/ggkjqsaim.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gcrjyifrf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.hesvh.cn/Article/details/gkjydoykf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/gltlhagrv.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.zdbjq.cn/Article/details/gsbmrjcwq.sHtML

Py:   resp.json()
来源：http://www.share.zdbjq.cn/Article/details/ggjfflzlu.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gkscuwfhb.sHtML

JS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gnxuldzxp.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gkndoeiqv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gsizaxxfn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/gvhujuncy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fehbvm.com/Article/details/gxkqrbnja.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/gdviktbyx.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gprjsxngi.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.zdbjq.cn/Article/details/giwlpvqaf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fehbvm.com/Article/details/gmjxrvmnm.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gugpoznml.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/grcvvlpcg.sHtML

Java: resp.statusCode()
来源：http://wap.fehbvm.com/Article/details/gkdhmdlij.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gvoralhwe.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/gjswatozg.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gfgeebmdk.sHtML

[L08] 并发请求多个地址
来源：http://blog.hesvh.cn/Article/details/gjarssqxm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/gzibefdub.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/gbeiifbpt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gqoequxjp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/ggejmpgtu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gylhzwnoq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.hesvh.cn/Article/details/gfdjqbabl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gpddnfijp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.hesvh.cn/Article/details/gngjatneb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gavhzrwkt.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gtprcnnva.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvudsahtk.sHtML

[M01] 读取命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gsrvmcqgp.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/gcozzbelp.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.zdbjq.cn/Article/details/gkezzhcub.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gnvuzhedn.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gyrvzbspt.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gkpjqxrea.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gcsnquuoo.sHtML

Ruby: ARGV
来源：http://wap.fehbvm.com/Article/details/glzbvvkez.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gndvamjwp.sHtML

[M02] 读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gaonsjuwy.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gqkdpixjd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gegdwbrpi.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gpkackoop.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gdderlfio.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/garfmumiv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gbrhxsdmq.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/gandapgei.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/gprolmgzg.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gyjyjeguh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gmsgrwsdc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/glkevtmel.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gwdzbjuin.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/graieafrq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/ghodlljdp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gpazjmpad.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/gxorsjxoj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/gmlnvvcyd.sHtML

[M04] 获取当前工作目录
来源：http://3g.zdbjq.cn/Article/details/gdhcqaahb.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/ggduwutom.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/gypuzspnm.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gpzuotaux.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gxyscjsgb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gtikgwree.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/gcwttvvms.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gspfgyfgo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gtozddiwe.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gooaiqsng.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gushqzqti.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/gokgnnbqc.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gpmysghjf.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gdkfgsnlz.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gxmvphixt.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/gygqdaqss.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gruacplnp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gpygbfarz.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gbrjuongd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gxpleytqw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/gbtjbhwaw.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gzrdcgycc.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gcoizlyyr.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gealggfzh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gcbqaenyn.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/ghdncqpyu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/grzhkquck.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/ggypdrgrp.sHtML


<!-- 参考信息 -->