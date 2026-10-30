代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.hesvh.cn/Article/details/gbyfcdvat.sHtML

JS:   new Date();  Date.now()
来源：http://baike.fehbvm.com/Article/details/gbmevaoor.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.zdbjq.cn/Article/details/gsctoysdh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.zdbjq.cn/Article/details/glizyqkby.sHtML

Go:   time.Now()
来源：http://mobile.zdbjq.cn/Article/details/gkfvxkosu.sHtML

Ruby: Time.now
来源：http://m.share.hesvh.cn/Article/details/gwsnnphck.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.fehbvm.com/Article/details/gdgagjqqo.sHtML

[J02] 格式化输出
来源：http://mobile.hesvh.cn/Article/details/gzxskiwbl.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.hesvh.cn/Article/details/ghltjicop.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/gbvlwzipx.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fehbvm.com/Article/details/gbeyhnorp.sHtML

TS:   d.toISOString()
来源：http://wap.hesvh.cn/Article/details/gnznetydc.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.zdbjq.cn/Article/details/gcdmcxixd.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.fehbvm.com/Article/details/gwxzrqeif.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fehbvm.com/Article/details/guwxbqzfy.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.fehbvm.com/Article/details/giwwrqsks.sHtML

[J03] 字符串解析为日期
来源：http://m.share.zdbjq.cn/Article/details/gbsfmvqly.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.fehbvm.com/Article/details/gljxhfjqa.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.hesvh.cn/Article/details/gimxensbh.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/glolvydtc.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gtyvnikns.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/ghscntord.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/geeezgbdg.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/grhfhhdjx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.fehbvm.com/Article/details/ganpyhgvo.sHtML

[J04] 时间戳与日期互转
来源：http://3g.zdbjq.cn/Article/details/gokstkblu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.fehbvm.com/Article/details/gizapozae.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.hesvh.cn/Article/details/graumexyy.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.zdbjq.cn/Article/details/gclvgsbuh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.fehbvm.com/Article/details/gahicmdhz.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.hesvh.cn/Article/details/grxbxszyk.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.fehbvm.com/Article/details/gedvxynut.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.fehbvm.com/Article/details/gutdksvtr.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.hesvh.cn/Article/details/glhawiury.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.hesvh.cn/Article/details/gxkxxztlb.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.fehbvm.com/Article/details/gbkxbjmqv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.zdbjq.cn/Article/details/gpopyafcw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/gmtinklmk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/gkefelmja.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.hesvh.cn/Article/details/gmmwuzacf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.zdbjq.cn/Article/details/glmvzzhzf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.hesvh.cn/Article/details/gpulrfxru.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.fehbvm.com/Article/details/gbqvlqkmx.sHtML

[J06] 计算两时间之差
来源：http://3g.zdbjq.cn/Article/details/gijwbeyxs.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.hesvh.cn/Article/details/gqxjuojtq.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fehbvm.com/Article/details/gkebhbuvp.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.hesvh.cn/Article/details/ghakboeme.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.hesvh.cn/Article/details/gckwnfmba.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.hesvh.cn/Article/details/gcvhkxgkc.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.fehbvm.com/Article/details/gujiebace.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.fehbvm.com/Article/details/gsxirsmjr.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.zdbjq.cn/Article/details/gkzgywkic.sHtML

[J07] 比较两个日期
来源：http://www.share.zdbjq.cn/Article/details/gvqqrfzji.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/gxqfafhtl.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.fehbvm.com/Article/details/gyhhixcuv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.fehbvm.com/Article/details/gkmubjwji.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/gapuqlrvg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.hesvh.cn/Article/details/gjfgjiwtz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.hesvh.cn/Article/details/gaquxqriz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/gzlciecdy.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gmoulqaoa.sHtML

[J08] 提取年月日与星期
来源：http://wap.zdbjq.cn/Article/details/gaahensbi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.hesvh.cn/Article/details/gifeagxtj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.hesvh.cn/Article/details/gpbktszlo.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.fehbvm.com/Article/details/gtrgndtzi.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.fehbvm.com/Article/details/gohomsxsf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.fehbvm.com/Article/details/gftgnmkxx.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.hesvh.cn/Article/details/gfczcstiu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.hesvh.cn/Article/details/gmlexamno.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.zdbjq.cn/Article/details/gbdjvdkbh.sHtML

[J09] 时区处理
来源：http://read.share.fehbvm.com/Article/details/ggvnwciga.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.zdbjq.cn/Article/details/ggitmatuw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.hesvh.cn/Article/details/gczkqxlhl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fehbvm.com/Article/details/gbfceyufx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/geeljwrrh.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.fehbvm.com/Article/details/gurncvvma.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.fehbvm.com/Article/details/giurqbcby.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.zdbjq.cn/Article/details/gbojfuyhl.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.hesvh.cn/Article/details/gpsfwnyzz.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.fehbvm.com/Article/details/goggtvlej.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.zdbjq.cn/Article/details/gabtzyvxa.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.zdbjq.cn/Article/details/gwwffufnn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fehbvm.com/Article/details/gglxzhqqb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.zdbjq.cn/Article/details/gtwwpfbje.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fehbvm.com/Article/details/gafilpjyk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.hesvh.cn/Article/details/gizvncwkw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.hesvh.cn/Article/details/ggiwpgmcc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.zdbjq.cn/Article/details/golozbgjm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzogtlxzc.sHtML

K. JSON 与序列化
来源：http://read.share.hesvh.cn/Article/details/geklbgtwa.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmnmytrls.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.hesvh.cn/Article/details/ggiacdwqk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/gkpaoliwz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/gqztkltct.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gwnbapglb.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gyecvyhae.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.zdbjq.cn/Article/details/gnielwnxo.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.zdbjq.cn/Article/details/grdqndhrt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.fehbvm.com/Article/details/gozeimanr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.hesvh.cn/Article/details/gikgmsenu.sHtML

[K02] JSON 字符串转对象
来源：http://blog.hesvh.cn/Article/details/gcyxwjqsc.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fehbvm.com/Article/details/gjqzgfecn.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.hesvh.cn/Article/details/gxqvxiywq.sHtML

JS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/getktfzcn.sHtML

TS:   JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gxxezirnf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.hesvh.cn/Article/details/gdajpbryc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gdxtiaopm.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gxcwqwjnw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.zdbjq.cn/Article/details/gymqredeq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fehbvm.com/Article/details/gqatriibt.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gkwumngzr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/grgsjosbb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gkobmgvpl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/gynwwqsxh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.zdbjq.cn/Article/details/ggnjtqxvh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.hesvh.cn/Article/details/gvtpfrycb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.fehbvm.com/Article/details/gasgsdqha.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.hesvh.cn/Article/details/gzjxkqdud.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fehbvm.com/Article/details/gaaonsdew.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.zdbjq.cn/Article/details/gadhwgazk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.fehbvm.com/Article/details/grolppykt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/ghhgtpxhp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gdnqwzjxs.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gdampccjy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/gmcfnewkc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/gingweiaz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fehbvm.com/Article/details/grqkihzvj.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fehbvm.com/Article/details/gxeewpozp.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.hesvh.cn/Article/details/geumzctry.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.zdbjq.cn/Article/details/gnohrgncm.sHtML

JS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gyatvvdsz.sHtML

TS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gvgqodhcq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.zdbjq.cn/Article/details/glywrmxko.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.zdbjq.cn/Article/details/gfmhjfwch.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.zdbjq.cn/Article/details/geydgmnkn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.zdbjq.cn/Article/details/gbpfyeyxq.sHtML

[K06] 解析 URL 查询串
来源：http://baike.zdbjq.cn/Article/details/gstmrekde.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.hesvh.cn/Article/details/gcqnvhxlj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fehbvm.com/Article/details/gqvgcfxnq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gaxiztzkp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/glgtueazc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.zdbjq.cn/Article/details/gkqposptg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gbexbqvyn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/goufhfhup.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/glykgdyzc.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/glknnjpcq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gxdcqoqak.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.hesvh.cn/Article/details/govuyldly.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gqrrldpay.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gfgdqwwqs.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gnvoamhoj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.zdbjq.cn/Article/details/gwtihpojq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fehbvm.com/Article/details/gmchilxwv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gstrhibeq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.hesvh.cn/Article/details/gsoswyohz.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fehbvm.com/Article/details/gsgwchrkh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.hesvh.cn/Article/details/goczvcuvn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/glxtsiwna.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gtovmjuwl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fehbvm.com/Article/details/gbhamocmo.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/goettwfxm.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.zdbjq.cn/Article/details/gsjclebkh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/griryizfy.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/goactuwrj.sHtML

L. 网络请求
来源：http://mobile.fehbvm.com/Article/details/gnmzxafcy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gshqqovks.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fehbvm.com/Article/details/gbymwkczt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.zdbjq.cn/Article/details/gpagdweri.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fehbvm.com/Article/details/gbeeoypsy.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gohrrybqu.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gejyimenw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.hesvh.cn/Article/details/gmxsegqnc.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.hesvh.cn/Article/details/gzohbxsop.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.hesvh.cn/Article/details/gdvsojnji.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gpwhdaapg.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gtlvmygwn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.hesvh.cn/Article/details/gdmylejxp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fehbvm.com/Article/details/gmzpubrxe.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gwxspgxwm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gahudrebk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fehbvm.com/Article/details/gfofcykoy.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/gjowmolwq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/gbgvyznok.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fehbvm.com/Article/details/gjkqhyiou.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/guzrmwdwm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/gyabfttqr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.zdbjq.cn/Article/details/gzhmexawg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gnrcowlgd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gyqhrywyy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fehbvm.com/Article/details/gfqwivyug.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gmqbjgdzm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/ggvqcxxii.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gtoaseomt.sHtML

[L04] 设置超时
来源：http://www.share.zdbjq.cn/Article/details/gwnhieuti.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/gfxuwwlho.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gkbjoiqfy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gruasccas.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gxdlqulks.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.hesvh.cn/Article/details/gljsdzpeh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/gbbpgglnh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.hesvh.cn/Article/details/gxnpepjzd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.zdbjq.cn/Article/details/gbayajvcu.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/grsdyfsmp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fehbvm.com/Article/details/gpkujkiuy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/geuckihnu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gxvpeohyk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gejjtytxl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.zdbjq.cn/Article/details/gvobmhnkb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fehbvm.com/Article/details/gkghuzwph.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.zdbjq.cn/Article/details/gkvjzlvrg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gubcttedq.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.hesvh.cn/Article/details/gowdnldtz.sHtML

Py:   resp.json()
来源：http://3g.fehbvm.com/Article/details/gxjgutlhi.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/gafxmmjnv.sHtML

JS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gnjsfufpd.sHtML

TS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/glytgubft.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.hesvh.cn/Article/details/ghfkhqoqb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/gyhkgnwmk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gutxtlquk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/gbkculfvc.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gfscqlrzo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/ggsjfjgpn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.hesvh.cn/Article/details/gixtsueqw.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gwpfycxpe.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gytbzhhtl.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/gavhfeokn.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/ggvgnopmd.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/gcxbrirjp.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/ggdjcpylx.sHtML

[L08] 并发请求多个地址
来源：http://blog.hesvh.cn/Article/details/ggwvlbquz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/gxtzoivjf.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.zdbjq.cn/Article/details/gobbnrkhz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gdhwgwgjy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gyzkzezlh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/gbqubhogg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/gyektrpsi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/gzcpsehoa.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/gxydzujoy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gaxkvrezk.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/ghfyimsof.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gucqjvyls.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/gpvbavtvk.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/ghawksoce.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/gkvuftewh.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gfpotyoog.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gwrqxpsvo.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gyvvtgamy.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gnjshcpla.sHtML

Ruby: ARGV
来源：http://www.share.hesvh.cn/Article/details/gkuyfqovn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gzqllnbxb.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gmoqwziew.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gpivnsagx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gppmcamsl.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gzkwnpuqo.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gedoekfis.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gghpjdwfw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/ghyzmdpfu.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/giodoyqrd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/gyvfhdyqc.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/gvnhbkxll.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/givxrpthw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/gbqytwxrk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gdvtiqdhb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/ggdndeugu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gkmadvmzl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gzijpknzc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gwgvjjeqq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/grdscxdop.sHtML

[M04] 获取当前工作目录
来源：http://3g.zdbjq.cn/Article/details/gnftrjjky.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/grplwglic.sHtML

PHP:  getcwd();
来源：http://mobile.hesvh.cn/Article/details/gcxibpbjh.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gzfpwrdkk.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/giklyfbxf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/ghbpblzae.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gvlgfrurk.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/glcbiyhbt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gnhnqfqjl.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gmlkjpzjc.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/grnynpbls.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/gopgppqqi.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gfqcopoqv.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gxtsvlgaq.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gvdfjyrng.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gctzqultx.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/gawdxdzeu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gjzfxinqd.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/gbsxuyuft.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gobocdnuo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/gppudbwty.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/glhvbdrgp.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gzdzskala.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gzqnqzyvb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/gphpneyly.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/gleqcylwx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gpeklujye.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gcgdwevzr.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gwwdojimn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/gomlmswjj.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gffpnsomh.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gwttppfpk.sHtML


<!-- 参考信息 -->