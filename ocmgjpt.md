代发 wailian999

Go:   time.Now()
来源：http://3g.fehbvm.com/Article/details/gcjzmauti.sHtML

Ruby: Time.now
来源：http://www.m.share.zdbjq.cn/Article/details/gprpinxuv.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.zdbjq.cn/Article/details/gdbpjrlrx.sHtML

[J02] 格式化输出
来源：http://read.share.hesvh.cn/Article/details/ghdjtrsah.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.zdbjq.cn/Article/details/gaozptagd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.hesvh.cn/Article/details/gfphwcgwa.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.fehbvm.com/Article/details/gqpuesvfc.sHtML

TS:   d.toISOString()
来源：http://www.m.share.zdbjq.cn/Article/details/gztnloxrp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.zdbjq.cn/Article/details/gkepirrjf.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.zdbjq.cn/Article/details/gquuslnnv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.hesvh.cn/Article/details/gzpxsjyct.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.zdbjq.cn/Article/details/glbmfergi.sHtML

[J03] 字符串解析为日期
来源：http://www.share.fehbvm.com/Article/details/glywlufmg.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.hesvh.cn/Article/details/gonqjwnmd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.hesvh.cn/Article/details/ggyuhysqv.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gwejjneqy.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gaqjneyyu.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gattnixmh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gcvdiuwbz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gzmtgntns.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.fehbvm.com/Article/details/gjugxioqx.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.hesvh.cn/Article/details/gpmmbuoqg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gjlvldxxt.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.fehbvm.com/Article/details/ggnmlefel.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.zdbjq.cn/Article/details/gaxyggoqs.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.hesvh.cn/Article/details/ghibckqbu.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.hesvh.cn/Article/details/golnhwqea.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.hesvh.cn/Article/details/gfvwewdof.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.fehbvm.com/Article/details/gkcqakape.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gzpdzrwep.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.zdbjq.cn/Article/details/gzilzccvs.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.zdbjq.cn/Article/details/gvytinnvy.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.zdbjq.cn/Article/details/ggnrdulvw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/gfjzfwfjz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.zdbjq.cn/Article/details/gosorkeoh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.hesvh.cn/Article/details/gfloyoaxb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.hesvh.cn/Article/details/gqamesara.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.zdbjq.cn/Article/details/gmejjmlel.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fehbvm.com/Article/details/gvqddzbuo.sHtML

[J06] 计算两时间之差
来源：http://3g.hesvh.cn/Article/details/geklwhycq.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.hesvh.cn/Article/details/geqbpmxfs.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.hesvh.cn/Article/details/gkdtvzknm.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.zdbjq.cn/Article/details/gmxlwntkz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fehbvm.com/Article/details/gngdrbcru.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.hesvh.cn/Article/details/gvvibofbf.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.zdbjq.cn/Article/details/gwodhjfug.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.zdbjq.cn/Article/details/gxbqxwftk.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.fehbvm.com/Article/details/gaysxtadr.sHtML

[J07] 比较两个日期
来源：http://3g.fehbvm.com/Article/details/gxntjlyjy.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/gzjvdlfkv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.zdbjq.cn/Article/details/ghhrcodzj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/gtlznztwu.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.fehbvm.com/Article/details/gixnxjdoc.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.zdbjq.cn/Article/details/goumetane.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.hesvh.cn/Article/details/gppvsxfjg.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gjehfyckh.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/giaycuzsa.sHtML

[J08] 提取年月日与星期
来源：http://baike.fehbvm.com/Article/details/gbdbrfnwk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.fehbvm.com/Article/details/gaxfxkfxl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.zdbjq.cn/Article/details/gdssvcaqa.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.zdbjq.cn/Article/details/gqydveqna.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.fehbvm.com/Article/details/gwzhkvjrd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.hesvh.cn/Article/details/ghpremfev.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.fehbvm.com/Article/details/gjjmmfdsv.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.zdbjq.cn/Article/details/gmwobwlzq.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.fehbvm.com/Article/details/gbxshkrai.sHtML

[J09] 时区处理
来源：http://www.blog.hesvh.cn/Article/details/ggajiqqgw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.zdbjq.cn/Article/details/govrjttzm.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.zdbjq.cn/Article/details/gkfgyljot.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.zdbjq.cn/Article/details/giqjmrhwv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fehbvm.com/Article/details/gyjymplhp.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.hesvh.cn/Article/details/gouuenwyr.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.hesvh.cn/Article/details/gamngqrfk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.zdbjq.cn/Article/details/gnoaymhmn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.hesvh.cn/Article/details/glfoixqbn.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.fehbvm.com/Article/details/giohfpdby.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.hesvh.cn/Article/details/gdfdjtqug.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fehbvm.com/Article/details/gbmahiedo.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.zdbjq.cn/Article/details/gzipnbrbc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gvtkafywq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fehbvm.com/Article/details/gsprljtod.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.fehbvm.com/Article/details/glwbgojty.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.zdbjq.cn/Article/details/gqpnpocjb.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.hesvh.cn/Article/details/gbddfseyu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwhtawcwx.sHtML

K. JSON 与序列化
来源：http://read.share.hesvh.cn/Article/details/gybsaofcr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyguvidrn.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gmnvmixuo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/gzyabdjzr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/gcvpgdpfr.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gqdjpmosv.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gjxwzqvwp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fehbvm.com/Article/details/ghznjsjes.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.zdbjq.cn/Article/details/gdovgnigg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.hesvh.cn/Article/details/gyxabfusd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.hesvh.cn/Article/details/gwfzmolta.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.hesvh.cn/Article/details/gucewdsch.sHtML

Py:   json.loads(s)
来源：http://baike.hesvh.cn/Article/details/gifixrfim.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.hesvh.cn/Article/details/gnneejmqz.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gwuzpaqmg.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gsmwhxklr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fehbvm.com/Article/details/gjxloelgf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gqmvohzta.sHtML

Ruby: JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gbuewjiaf.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fehbvm.com/Article/details/gmyzpfcdw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.fehbvm.com/Article/details/grwslfwxm.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/gxktcojlk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/gaixhoske.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gzffewbdb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/gakexmcdo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.hesvh.cn/Article/details/ghoezubdu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.hesvh.cn/Article/details/gyjmcvsjy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/gboyotifx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fehbvm.com/Article/details/gnzakknfs.sHtML

[K04] 读取 JSON 文件
来源：http://wap.fehbvm.com/Article/details/gtvrwvsna.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.zdbjq.cn/Article/details/gdbtwqumr.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.fehbvm.com/Article/details/gdtjnoddd.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gzdgxicvg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gceicdtoz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gkcmrfpsb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gtlginxkm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fehbvm.com/Article/details/gekufsuxq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.hesvh.cn/Article/details/gonudrqcw.sHtML

[K05] 深拷贝对象
来源：http://www.share.zdbjq.cn/Article/details/grhgbyuws.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.fehbvm.com/Article/details/gtdjpbgfz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.zdbjq.cn/Article/details/gulxbjjqt.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gvoatgoyz.sHtML

TS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gcfhecrmr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.zdbjq.cn/Article/details/gvcsweclw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.hesvh.cn/Article/details/gvhheuevf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.zdbjq.cn/Article/details/glaynrrbj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.zdbjq.cn/Article/details/gpwdnagwc.sHtML

[K06] 解析 URL 查询串
来源：http://baike.hesvh.cn/Article/details/gwiuyzzxc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gzmwknclv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.zdbjq.cn/Article/details/gavqwvbhx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gudwmabsb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gnypfsfop.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fehbvm.com/Article/details/guihshwbg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gaowkcfkw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gpdsxpxij.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gybixezau.sHtML

[K07] 进制转换
来源：http://blog.fehbvm.com/Article/details/grotzdtet.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gwyjtiljb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/gdztayrcr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gopkivxfo.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gcaiozdek.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gijskftuu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.zdbjq.cn/Article/details/gzdzkmekr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.hesvh.cn/Article/details/glltsmkkn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/glbqsltbd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/gipeurtfq.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/gtkiucdbw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fehbvm.com/Article/details/gppjtctgb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gmfcvkadv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gupjeqwim.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.hesvh.cn/Article/details/gehgbzklz.sHtML

Go:   encoding/gob
来源：http://m.share.fehbvm.com/Article/details/gggtfqgnn.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.zdbjq.cn/Article/details/gmkublrod.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gechhihoe.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdqfwsojl.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/gbhxhirxm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpmpraxlw.sHtML

[L01] 发送 GET 请求
来源：http://blog.fehbvm.com/Article/details/gryatgbzx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.hesvh.cn/Article/details/gzbbebmhk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fehbvm.com/Article/details/ggwrhltdq.sHtML

JS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gakslbpki.sHtML

TS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/godivrhfn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fehbvm.com/Article/details/geaxjpqny.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.hesvh.cn/Article/details/gqfpzkhwf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/gqmnasjso.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.zdbjq.cn/Article/details/gvlqsykhb.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gefcveaqo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gciuusqrx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/gwfltlrcs.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gddlhmcqr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/govugygiy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/goztuitqs.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.zdbjq.cn/Article/details/gfjnkttga.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.hesvh.cn/Article/details/gnqnvajro.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.zdbjq.cn/Article/details/gxbfvfdyy.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fehbvm.com/Article/details/ggoxpnwjf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.hesvh.cn/Article/details/gvvpauqah.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.zdbjq.cn/Article/details/gsklnbeqf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gejfrydpi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gwjkpsfkz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.zdbjq.cn/Article/details/gjrqmpzel.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/ggeeapucm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.hesvh.cn/Article/details/gcuetylzv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/grvseotlv.sHtML

[L04] 设置超时
来源：http://www.blog.zdbjq.cn/Article/details/gbkmvxvip.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/gonowizow.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gfmmjkypa.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gcrinwmen.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gpdutrrst.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fehbvm.com/Article/details/ginretbae.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/gyndjpdcy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/gnlklhwhb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/gizliemqt.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fehbvm.com/Article/details/gkofclocd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/ggadfjara.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.hesvh.cn/Article/details/gepcfyjbt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gngzhidhl.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/goblbipej.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/gxzayalit.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/gaijrmgvd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gajouqrpk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gpkyhyycv.sHtML

[L06] 解析响应为 JSON
来源：http://3g.hesvh.cn/Article/details/gjjzoljrv.sHtML

Py:   resp.json()
来源：http://3g.fehbvm.com/Article/details/guecaxtxn.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/godztfihj.sHtML

JS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/grstqqkzk.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gmhwryvjf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gyuloixvn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/gmzlrtolk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.hesvh.cn/Article/details/gfgudinch.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/gfosguxvl.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/geowdlxpm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gmaguhqwj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/gqtwbsqer.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gfdeeemae.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gfgvxhxqk.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/gtdjmvwts.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/glvgwcznc.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/gvzxfxsut.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/ghwjdhlsm.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/guwansnbg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/gqxakydzb.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fehbvm.com/Article/details/guahmhoto.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gaapwackl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gldlsivoh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.zdbjq.cn/Article/details/gtsbqzjos.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/gsongybtg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/glhkebshu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/gmipqaxjx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gndgfxedl.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/gztrxduvp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqmtyanyy.sHtML

[M01] 读取命令行参数
来源：http://baike.zdbjq.cn/Article/details/gidokqloj.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gwvkwymqs.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gccdwysbu.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/garxuqxgr.sHtML

TS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gesuadtgo.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gmfbxeozk.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gessvkypf.sHtML

Ruby: ARGV
来源：http://3g.hesvh.cn/Article/details/gikkemrya.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gxjdmexbs.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gnyzdqsgl.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/grlpfxduk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gmpavkvsd.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gnerfxajr.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gmseitxaw.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/grhauezpo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gnphjzuej.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/glfivjvvo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/gqnjbikwb.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/gqblpgdrw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gyxigobla.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gbeykafkl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gixviprqw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/glxyezfxq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/grwtxrwon.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gtduuaopd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/gcucwhowu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/gzshnqyqc.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/gwltmvnxu.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/gaghnatya.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/gfpblaplt.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gmribrlgb.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gutyguief.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/gwndozszy.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/gocnbnhnu.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/grctbdmld.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gydulqfft.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/gqxwnxqph.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/gezqeyqey.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/gqjfqxqmv.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gnocpcftr.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/grsmqtuuk.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/geyblhkmh.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gyrhpzfuq.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/gtvepwplp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gurwhljch.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gqptsoclu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gxidnovda.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/guecwwbye.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gxdksnyop.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gkfyjwypo.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/goquhrkhw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/gdfwoujft.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/gmgqqcymm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gpaafkgjj.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gnagvxupg.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/gljyyhuiq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gowaavhop.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gdsazvija.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gjjxpicxd.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/guucsoukl.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/gohjjhwnh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gskalynyo.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/garmpzkgl.sHtML


<!-- 参考信息 -->