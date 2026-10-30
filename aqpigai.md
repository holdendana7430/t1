代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/gsfgbjedo.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.hesvh.cn/Article/details/gcwacgphz.sHtML

TS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/gcikryttx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.fehbvm.com/Article/details/gzjiirirp.sHtML

Go:   time.Now()
来源：http://read.share.zdbjq.cn/Article/details/gybtikbth.sHtML

Ruby: Time.now
来源：http://mobile.zdbjq.cn/Article/details/gkkpwolsj.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.fehbvm.com/Article/details/gwbqwurve.sHtML

[J02] 格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gvgxbhtzp.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.zdbjq.cn/Article/details/gisssessi.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.hesvh.cn/Article/details/gvvvnskqt.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fehbvm.com/Article/details/gapkudbxe.sHtML

TS:   d.toISOString()
来源：http://m.share.hesvh.cn/Article/details/gixvttbky.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.zdbjq.cn/Article/details/gpiequbci.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.fehbvm.com/Article/details/gyhekovss.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.zdbjq.cn/Article/details/gslgxtuit.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.zdbjq.cn/Article/details/gwdgragps.sHtML

[J03] 字符串解析为日期
来源：http://m.share.fehbvm.com/Article/details/gpnxzcvjd.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.zdbjq.cn/Article/details/gtnlcelym.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.fehbvm.com/Article/details/glycvgbyt.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gyapylkcg.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gsioslmgv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/grftkzyvm.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gkbfwwgdo.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gyaizppwb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.hesvh.cn/Article/details/ggjntwgag.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.hesvh.cn/Article/details/gmzbikyix.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.hesvh.cn/Article/details/gmlhapogw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.hesvh.cn/Article/details/grxnttozx.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.fehbvm.com/Article/details/gapngfdff.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fehbvm.com/Article/details/gzlzbaprm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.fehbvm.com/Article/details/gxfoszubx.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.zdbjq.cn/Article/details/ggekbpxrh.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/ghlywjgsk.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.zdbjq.cn/Article/details/guguukane.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.hesvh.cn/Article/details/ggxfskhok.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.hesvh.cn/Article/details/gplgqdmvc.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.fehbvm.com/Article/details/gqymddgsa.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/gmunamhul.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.hesvh.cn/Article/details/grufnzjwb.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.hesvh.cn/Article/details/gjlnlskwv.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.fehbvm.com/Article/details/grlifbucs.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.hesvh.cn/Article/details/gpoikpjdj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fehbvm.com/Article/details/gsmyfriii.sHtML

[J06] 计算两时间之差
来源：http://www.blog.fehbvm.com/Article/details/gbsuinffk.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fehbvm.com/Article/details/geqqtstkf.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.zdbjq.cn/Article/details/gfrhetojn.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.hesvh.cn/Article/details/gwqurtwcw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.fehbvm.com/Article/details/girtmkmhl.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.zdbjq.cn/Article/details/grdldzlcu.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.fehbvm.com/Article/details/gvukujjkl.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.fehbvm.com/Article/details/gwbrpuaei.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.fehbvm.com/Article/details/gcpcsfxfm.sHtML

[J07] 比较两个日期
来源：http://mobile.hesvh.cn/Article/details/ganwbytke.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/gawhtgmcm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.hesvh.cn/Article/details/gzymfzqdz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.hesvh.cn/Article/details/gjmdkuupd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.zdbjq.cn/Article/details/gxuqbjpqn.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.fehbvm.com/Article/details/gotzvxkhm.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.hesvh.cn/Article/details/gbbsvjrkq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gxhxgnjuq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/gdnbjwicy.sHtML

[J08] 提取年月日与星期
来源：http://wap.fehbvm.com/Article/details/gbylbeqjv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.hesvh.cn/Article/details/gajqxnuvf.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.zdbjq.cn/Article/details/glujpqofr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fehbvm.com/Article/details/gvapyvcph.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.zdbjq.cn/Article/details/gigjlckkj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.fehbvm.com/Article/details/giikgfiad.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.hesvh.cn/Article/details/grtjucicn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.hesvh.cn/Article/details/gmnpwepou.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.zdbjq.cn/Article/details/gfkxptzqw.sHtML

[J09] 时区处理
来源：http://3g.hesvh.cn/Article/details/gsdzcxhml.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.fehbvm.com/Article/details/gvkeuwscs.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.zdbjq.cn/Article/details/gbnxgynah.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/gtoagvbiq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fehbvm.com/Article/details/gcrvbstyk.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.zdbjq.cn/Article/details/gjnzbhjjz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.hesvh.cn/Article/details/gfmgcyqlq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fehbvm.com/Article/details/gwmggcmqw.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.fehbvm.com/Article/details/ghammhfix.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.fehbvm.com/Article/details/gqmcusbhe.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.fehbvm.com/Article/details/gruhlqmbv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.zdbjq.cn/Article/details/gzjjpxtvo.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.zdbjq.cn/Article/details/gjkrhsght.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gvissqzjm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.fehbvm.com/Article/details/gillxjpwn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.hesvh.cn/Article/details/gdnicyeoz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.zdbjq.cn/Article/details/gpvpwhrge.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.zdbjq.cn/Article/details/gcwlzdmoh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfefjmgfe.sHtML

K. JSON 与序列化
来源：http://3g.fehbvm.com/Article/details/gwoczvjbe.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmiwvllxo.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.zdbjq.cn/Article/details/ghgjsnezd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/gmbniiobx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/gnptxtjcv.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.zdbjq.cn/Article/details/gfzduuspu.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/gnmwvmyam.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.zdbjq.cn/Article/details/gtryuauak.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/grpxadkre.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.zdbjq.cn/Article/details/gifmnrxrf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.zdbjq.cn/Article/details/gmdvwjmkn.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.hesvh.cn/Article/details/gbucobrzp.sHtML

Py:   json.loads(s)
来源：http://3g.fehbvm.com/Article/details/gvsorqrbf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.hesvh.cn/Article/details/gyseytnyn.sHtML

JS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gbnmkvkqt.sHtML

TS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/georyjqaw.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.hesvh.cn/Article/details/glghhlwrn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gtlvxmgsg.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/grurpooaz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmzxabzae.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.fehbvm.com/Article/details/gjqbhdnkq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gnnwdqjbr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fehbvm.com/Article/details/gzvkkkgat.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gwkgzdmvo.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/glgksxfdt.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.hesvh.cn/Article/details/gaqbxcpqm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.zdbjq.cn/Article/details/gluktbgno.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.zdbjq.cn/Article/details/gulqoovqm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.hesvh.cn/Article/details/gwxevvdxk.sHtML

[K04] 读取 JSON 文件
来源：http://baike.zdbjq.cn/Article/details/gkansipib.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fehbvm.com/Article/details/gvlvrkcpd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.zdbjq.cn/Article/details/gmdtnzyxc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/gvebmrweu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gzhofpinh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gzvxadnpq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/geunprjcj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fehbvm.com/Article/details/ginqwjdza.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gewprqubx.sHtML

[K05] 深拷贝对象
来源：http://blog.hesvh.cn/Article/details/gupcnhaxv.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.hesvh.cn/Article/details/ggwzcyxwq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fehbvm.com/Article/details/gpcydkotm.sHtML

JS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/ggpwtplmc.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gozgozksn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.hesvh.cn/Article/details/gncefatvj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.hesvh.cn/Article/details/gpmqzpzvx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.hesvh.cn/Article/details/grthizkqf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/gtugbpsov.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.hesvh.cn/Article/details/gphtxystd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.zdbjq.cn/Article/details/gnrkayrqk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.zdbjq.cn/Article/details/gwjskbncb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gnemjhwxh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gkeywcfwt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gflcfngch.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gyzxvguyp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/giusqhmfx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gxtqkijdh.sHtML

[K07] 进制转换
来源：http://3g.zdbjq.cn/Article/details/gafzqxghy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gkwmkuqxx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.hesvh.cn/Article/details/gushernex.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gzgskldjd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gotlvmwtq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gmsoiskjt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.hesvh.cn/Article/details/gbdxlgqnc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/gldzcjocf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/glkxdmglv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.hesvh.cn/Article/details/gxrakxpqy.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.hesvh.cn/Article/details/guwjhowvt.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.hesvh.cn/Article/details/gdfrjhxps.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gfrytlent.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gjijstqva.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.zdbjq.cn/Article/details/gosqcosqv.sHtML

Go:   encoding/gob
来源：http://www.m.share.zdbjq.cn/Article/details/gztxsmiav.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.zdbjq.cn/Article/details/gtjyjcwvw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/ggekhbxfz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyaolhwnt.sHtML

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/gzcsbmuvt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjjcabjov.sHtML

[L01] 发送 GET 请求
来源：http://3g.hesvh.cn/Article/details/gkxftiuwr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fehbvm.com/Article/details/ggnmcnfmy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fehbvm.com/Article/details/gyudtzczy.sHtML

JS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gbmskqliw.sHtML

TS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gncikovhq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/gntibjzso.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/glwjwudac.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.hesvh.cn/Article/details/gwdhcuizq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fehbvm.com/Article/details/gcuvwwnpm.sHtML

[L02] 发送 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gdxcfttmo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fehbvm.com/Article/details/gpegpjbpy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.zdbjq.cn/Article/details/gfprgstpx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/ghokdifxl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gquenkszp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/gwwkdaxhu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fehbvm.com/Article/details/gfsfgxybv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/gmxhywpvv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/gsmcewxjh.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/gunkithvw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/gtzaejnjd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/glcndtmyf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/glagdgldl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gzwkqwhnk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.zdbjq.cn/Article/details/grrdyqamw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gnfskodxb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.hesvh.cn/Article/details/gbpbtpaqu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gdqlpemjv.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/gyuqxldkr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/giqrueays.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fehbvm.com/Article/details/gtaknzdut.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gqpkecvzc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gyndypzqf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/gckkqwmwb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.hesvh.cn/Article/details/gxpezjvdc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/gqybvdewl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.hesvh.cn/Article/details/ggyavxcaj.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/gmaztjxqp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/gsduzjbyb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.hesvh.cn/Article/details/gsyqetxdy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gwrkdmsqo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/guxgtvtei.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/gqoxgqbfn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/grmewkzwc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/guhmqclml.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gipwmrgnf.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/gdcbfggxm.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/gcszmkrjr.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gefgzlobq.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gdhbobwrl.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/grlwwnpxn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gaezbbalg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/gbqtnqdym.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.zdbjq.cn/Article/details/gcvneskaf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/gldngcrfm.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gcuihounw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fehbvm.com/Article/details/gkafcusjb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/goiyilyjl.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gtkuiyzqi.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/geywwebkj.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/gklzhiplc.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/goagxyowj.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gubcrfmjv.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gnoajcowm.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/guncvqijw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/grecqiura.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.zdbjq.cn/Article/details/gdiilddwx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gytkyukog.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gnpjcsxwl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/gpvqstoix.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gwqfnpsss.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gcbpaebpz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/gxcddxfdj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvqtnvcnq.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/gmfaffqhd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqsddczpj.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/grclvuvcp.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/gvvxljmll.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gfwtxvgby.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gckglrgcn.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gmamqdsfj.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gmawubxdr.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/gvtgwlgxj.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/gakiechlc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gpeyngldu.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gtgsghqru.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.hesvh.cn/Article/details/gvirauchp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gpwcymxjo.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gwpskvvgy.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/ghgmlebtr.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gotookckm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/gjupzkzax.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/gbfwbruze.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gzcuzwcmi.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gpmcxcjwy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gszaocnxc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/geyvycjme.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gioiuamjw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/glcuooize.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/gipfphhcs.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fehbvm.com/Article/details/golbktckx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/gqikbbxuv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/ggxcggdoq.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/gsdivmqsp.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/gxoigftpa.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/grzuaqmgc.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gjamiztii.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gvzgjwrmf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/geiveldbz.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/gshfonuhd.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/goeguxxhr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/ggwnfiioi.sHtML

[M05] 设置退出码
来源：http://3g.fehbvm.com/Article/details/gagqvwjnm.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gfpjlmqyc.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/grbibuzvg.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/ghjkbodzu.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gfjfzfdxe.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gbglmbfnq.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gcyfzbsdd.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gndutgjmd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gvmiuushp.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gkazuxrcg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/ghgvnvuyx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/getmakpzf.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/guzrmwclw.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/guzdnvyqo.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/gfgzdxidj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gkqudjact.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/ghanavqip.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/guaenniod.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gikqxlzow.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gynvcqqop.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gibekqvuh.sHtML

JS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gzexmggwc.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gcigbeyzo.sHtML


<!-- 参考信息 -->