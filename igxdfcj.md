代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/gbeosrlop.sHtML

JS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/gjjoswsyg.sHtML

TS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/gkpkdiwtx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.fehbvm.com/Article/details/gwrgennev.sHtML

Go:   time.Now()
来源：http://m.share.zdbjq.cn/Article/details/gjurtfafn.sHtML

Ruby: Time.now
来源：http://wap.fehbvm.com/Article/details/gjdrtking.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.zdbjq.cn/Article/details/gnuodgxhh.sHtML

[J02] 格式化输出
来源：http://blog.fehbvm.com/Article/details/gmlzgiejm.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/gwkzcojkt.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.hesvh.cn/Article/details/gpejmirbs.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.hesvh.cn/Article/details/gzanxvtbg.sHtML

TS:   d.toISOString()
来源：http://www.m.share.hesvh.cn/Article/details/ghudytlqd.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.fehbvm.com/Article/details/gtgtaqkxq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.hesvh.cn/Article/details/gvhqgjugt.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/gehktwsrz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.zdbjq.cn/Article/details/gqzarflug.sHtML

[J03] 字符串解析为日期
来源：http://read.share.fehbvm.com/Article/details/gngijpjlz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.hesvh.cn/Article/details/grojiwmbw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.fehbvm.com/Article/details/grzueeoez.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gtcuiccaa.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gehrwcfyh.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/glbhycnhf.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/glarrluot.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gmuoagpmg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.fehbvm.com/Article/details/gsnzrrnak.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.fehbvm.com/Article/details/gkvjffkue.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.hesvh.cn/Article/details/gduiushsa.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.zdbjq.cn/Article/details/gdhftzgsp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.fehbvm.com/Article/details/ginttvyeo.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.zdbjq.cn/Article/details/gweuulkrm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.zdbjq.cn/Article/details/gtuuystyp.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fehbvm.com/Article/details/gfbekibfg.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.zdbjq.cn/Article/details/gkakcebfy.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.fehbvm.com/Article/details/gpsmuezyv.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.fehbvm.com/Article/details/gnjaauufh.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.fehbvm.com/Article/details/gxyyfytmg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.fehbvm.com/Article/details/gmjeidkxv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fehbvm.com/Article/details/gylbdokhz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fehbvm.com/Article/details/grhpodkrk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.hesvh.cn/Article/details/giycymahj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.zdbjq.cn/Article/details/geyxmwsby.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.zdbjq.cn/Article/details/grhaoddnb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.zdbjq.cn/Article/details/gzvqukohv.sHtML

[J06] 计算两时间之差
来源：http://blog.zdbjq.cn/Article/details/guajvinuz.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.zdbjq.cn/Article/details/guzmkdwls.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.fehbvm.com/Article/details/gvkrrryeo.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.zdbjq.cn/Article/details/gcwguptra.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.zdbjq.cn/Article/details/gubbvzcyg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.fehbvm.com/Article/details/guartpiop.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.fehbvm.com/Article/details/grypspkfa.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.zdbjq.cn/Article/details/gdsykjjkg.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.hesvh.cn/Article/details/ghlttekzy.sHtML

[J07] 比较两个日期
来源：http://baike.fehbvm.com/Article/details/gjveynitb.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/grbaqaxos.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.hesvh.cn/Article/details/gaibjijtv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.hesvh.cn/Article/details/grlyvsvjf.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/gbfbhstht.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.zdbjq.cn/Article/details/gkwwaucci.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.zdbjq.cn/Article/details/gdwfnyrzx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gurwcwdrn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/grdybefsx.sHtML

[J08] 提取年月日与星期
来源：http://blog.fehbvm.com/Article/details/gzugshwoe.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.hesvh.cn/Article/details/guobyyayv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.fehbvm.com/Article/details/gsaddyrlt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.fehbvm.com/Article/details/gpyzfkmrt.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.fehbvm.com/Article/details/gizzkxogb.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.fehbvm.com/Article/details/gcelgtdxq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.fehbvm.com/Article/details/gwfbcdzbq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.fehbvm.com/Article/details/gsevqljxf.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.hesvh.cn/Article/details/gqbttwnyw.sHtML

[J09] 时区处理
来源：http://3g.zdbjq.cn/Article/details/gczbiyiya.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.hesvh.cn/Article/details/gebovfptd.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.zdbjq.cn/Article/details/gsjofpghg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.hesvh.cn/Article/details/gsaibpkya.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fehbvm.com/Article/details/gvsbjwxqi.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.hesvh.cn/Article/details/gzvilpqzy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.hesvh.cn/Article/details/gjugbekgy.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.fehbvm.com/Article/details/gepxszyjd.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.hesvh.cn/Article/details/gwqdvdrgw.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.zdbjq.cn/Article/details/glykadesm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.zdbjq.cn/Article/details/grqkhcbjw.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.hesvh.cn/Article/details/gqiiwddvg.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.fehbvm.com/Article/details/grggdhbfj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.fehbvm.com/Article/details/gqayzhqsr.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.hesvh.cn/Article/details/gbzpuamva.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.zdbjq.cn/Article/details/gzqzugzsb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.zdbjq.cn/Article/details/gpoinrnqr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fehbvm.com/Article/details/gdmkwpohl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxjufirlr.sHtML

K. JSON 与序列化
来源：http://baike.hesvh.cn/Article/details/gggvkrelj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdabkttsw.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.fehbvm.com/Article/details/geactpzvy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/gbdeqxeut.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/gmyclgnze.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.zdbjq.cn/Article/details/gtbbegufv.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gcmhrqivp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fehbvm.com/Article/details/gbudeolvb.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.zdbjq.cn/Article/details/gffszcpcj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.fehbvm.com/Article/details/ggsqgfupw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.zdbjq.cn/Article/details/gvqprezfk.sHtML

[K02] JSON 字符串转对象
来源：http://blog.hesvh.cn/Article/details/geauwjmbf.sHtML

Py:   json.loads(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gsnyksnzd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fehbvm.com/Article/details/gqcjlyubx.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gdfdqdagt.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/ggbfwsyjs.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.hesvh.cn/Article/details/ggqokrbcw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/glserfqhe.sHtML

Ruby: JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gzexqvldt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.fehbvm.com/Article/details/gfkomfwua.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fehbvm.com/Article/details/gohqiirsf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/govbutizg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gitbckntf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/gnkqfuuwh.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gctbamzac.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fehbvm.com/Article/details/gbnbggkmx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.hesvh.cn/Article/details/gworlqbvc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.zdbjq.cn/Article/details/gdjjsutnj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.hesvh.cn/Article/details/glgfiasdd.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.hesvh.cn/Article/details/gyylasubo.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.zdbjq.cn/Article/details/gisnjugri.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.zdbjq.cn/Article/details/gnbcdbncg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gssxtdfyx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/gdffsbojd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.hesvh.cn/Article/details/gpbfgzvos.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gzsdwukjw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gfmkshchr.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gcrredjgw.sHtML

[K05] 深拷贝对象
来源：http://m.share.fehbvm.com/Article/details/ghvnvllfg.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fehbvm.com/Article/details/gmtzpmkwd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fehbvm.com/Article/details/gatdikahp.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gjfcsicrl.sHtML

TS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/ghqhlqjuw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.hesvh.cn/Article/details/gfietghlv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.hesvh.cn/Article/details/gddhfscxx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/gktitkcmi.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.hesvh.cn/Article/details/gduvadoka.sHtML

[K06] 解析 URL 查询串
来源：http://wap.hesvh.cn/Article/details/gsdztmtha.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gyqgbouap.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fehbvm.com/Article/details/gfhzzspwn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/glafxhmpg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/glweymjxg.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.hesvh.cn/Article/details/gdgjkltrt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/ghslthtbp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gdvvqxzhk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gvzryeyfb.sHtML

[K07] 进制转换
来源：http://3g.zdbjq.cn/Article/details/gvgxwcyim.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gmfzfgtoi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.zdbjq.cn/Article/details/gejjgrkyb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gszddasov.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gulvdffuu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gueckjxbf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.hesvh.cn/Article/details/gzxoagjzq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.hesvh.cn/Article/details/gjwoyzgji.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gtnwkgxch.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.hesvh.cn/Article/details/gguzwxvfr.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.zdbjq.cn/Article/details/gqblhwhnd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/goejkucns.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gdczmvylt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gsrfnkcgt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fehbvm.com/Article/details/gzaucrurj.sHtML

Go:   encoding/gob
来源：http://www.blog.zdbjq.cn/Article/details/gpxaonyol.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gsiszehsq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/glqlksocn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdxdafibd.sHtML

L. 网络请求
来源：http://mobile.fehbvm.com/Article/details/gtgwhjepk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsrxjyovn.sHtML

[L01] 发送 GET 请求
来源：http://wap.hesvh.cn/Article/details/ggnmnqodh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.fehbvm.com/Article/details/gfewszdsr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fehbvm.com/Article/details/gdkrdoeem.sHtML

JS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gwvweflzy.sHtML

TS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gllcekvex.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.zdbjq.cn/Article/details/gqhkjrjur.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fehbvm.com/Article/details/gbqxvpspn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.hesvh.cn/Article/details/gdfbvhyoe.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/gbqbdxbmx.sHtML

[L02] 发送 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gntnajfwh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/glyjsuggf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.hesvh.cn/Article/details/grjsgjkrw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gsmvmslky.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gwozyzqpk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gayehmkgd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fehbvm.com/Article/details/gnbmsuyts.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fehbvm.com/Article/details/gnchcxvvn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.zdbjq.cn/Article/details/gaufowtph.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/gijnagdpx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fehbvm.com/Article/details/gjtgvnimu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.hesvh.cn/Article/details/gcgrqnfls.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gpyqzatmx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gwmddxisq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.hesvh.cn/Article/details/greazunvz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/grwupnatt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/ggsmsvilk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gcqajpuww.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/ghofkluwl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.hesvh.cn/Article/details/gnvqgormy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fehbvm.com/Article/details/gbzkozmsd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gpetgacfv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gtcqpklbu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/gspmbwzru.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.zdbjq.cn/Article/details/gydzwctvx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/gkqfjpnqd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/godciffwt.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fehbvm.com/Article/details/gnkltobiq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/gqyabnrpy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/gvfcjlzhd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/glndmifyj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gubvuonxx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gmdeycyok.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.zdbjq.cn/Article/details/gjvroawry.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/gmszdtmgg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gavkqebij.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.zdbjq.cn/Article/details/gftbwpelc.sHtML

Py:   resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gzoxhgnnt.sHtML

PHP:  json_decode($body, true);
来源：http://wap.hesvh.cn/Article/details/gqlnhxvfo.sHtML

JS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gbnrcaehm.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gvloekpvr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gmjbjuqjo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/gyhchatsd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/gzldofqrl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/gmettstai.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gpbjgbroc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gukeeteli.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/gikfyidqw.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gqojyyxkq.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gdbazyhlg.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/gsotfutkm.sHtML

Go:   resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gyexnkzpx.sHtML

Ruby: resp.code.to_i
来源：http://wap.hesvh.cn/Article/details/gkqoazjsf.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gfrcllecc.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/gicivwqnw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fehbvm.com/Article/details/grsswzmcv.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/gqiofmqvx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/glujwkuhq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/ggpnnpnox.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gjqeoyhqe.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/giuytiwqp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.hesvh.cn/Article/details/gyrrgolrr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.hesvh.cn/Article/details/gyfzxkiem.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gabvenvci.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/gyjutsyyw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggvjuozqn.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gajadhnwy.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/gztpkyqcg.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gevtfydgu.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gimikzcel.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/ghirdcwgp.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gxgsjngvi.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gatwrtwpl.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gcentpnyy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gyqxcbnwt.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gphmibxqz.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gcbzibbkc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gdlzyzwef.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/grvbgvjcd.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/ggfacdoqv.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gevpwzkjr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/ghkkiunde.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/gosyjnfaq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/gczmlwcde.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/gkenuphgc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/gibicjezj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/genuknntk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gulshnjpk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gbgxouicc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gipdjgdnx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gemdsuarx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/gretrbwde.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/goewaujto.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/gxrtdnnsy.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gfiqijeix.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/gsawgepzc.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gsrvshcwf.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/ghayacujh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gtuovlvbk.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/gzjuqsmkj.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/getdyevqd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/gqcjvqvwh.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gtwuwgotw.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/glydafbxb.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/gtlckqkrm.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gzygiuyow.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gduuouwyx.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gxkfhgomb.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gliczhjsx.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/grvwuwcnr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/grtdropjh.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gweqtvvop.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gjxsfilwt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/ghfyqxocd.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gvxsblhua.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/ggzwepndc.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gqlzvpddj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gcxiilerz.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/guirxcpwb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/gxzrjanbp.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gutmnaadv.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/geqhaudjm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/goufwkhvs.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gzratzphw.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/ghiykscyp.sHtML


<!-- 参考信息 -->