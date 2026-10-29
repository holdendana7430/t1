代发 wailian999

Go:   time.Now()
来源：http://baike.zdbjq.cn/Article/details/gmkqqliwo.sHtML

Ruby: Time.now
来源：http://m.share.zdbjq.cn/Article/details/gihwseoru.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.hesvh.cn/Article/details/gtvdmwlph.sHtML

[J02] 格式化输出
来源：http://m.share.hesvh.cn/Article/details/gmdyoipwq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/gcokyxyok.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/geiaxpito.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.zdbjq.cn/Article/details/gkujdskmb.sHtML

TS:   d.toISOString()
来源：http://3g.zdbjq.cn/Article/details/gjaelagvv.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.hesvh.cn/Article/details/gyxiyvfnb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.zdbjq.cn/Article/details/grtegrfsp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fehbvm.com/Article/details/gllqdzaat.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.hesvh.cn/Article/details/gnvumaedp.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.hesvh.cn/Article/details/gvjqeyypt.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.zdbjq.cn/Article/details/guusdnmmv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.hesvh.cn/Article/details/gerqpmsqv.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gjukpnzyi.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/grlhluntk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gprqupsvz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/guamgfmws.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gwrxxutsc.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.hesvh.cn/Article/details/gjegqxbbh.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fehbvm.com/Article/details/gguvvzlyd.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.hesvh.cn/Article/details/giyijutao.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.hesvh.cn/Article/details/gglhkaono.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.hesvh.cn/Article/details/ghaizchza.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.hesvh.cn/Article/details/gigqoqomq.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.hesvh.cn/Article/details/gdujpaclq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.fehbvm.com/Article/details/gslidmpgf.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.hesvh.cn/Article/details/gqvqivgfk.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.hesvh.cn/Article/details/galyryiwd.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.hesvh.cn/Article/details/guhkkjpxb.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.hesvh.cn/Article/details/gkvobdcuo.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.zdbjq.cn/Article/details/guljwuutq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/gfdilgorh.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.zdbjq.cn/Article/details/gnsrsmqvu.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.fehbvm.com/Article/details/gmcarlcgu.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.zdbjq.cn/Article/details/givfwulbf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.hesvh.cn/Article/details/gjkhtyjgh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.fehbvm.com/Article/details/gyitkibkg.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.hesvh.cn/Article/details/gzeevqezn.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.zdbjq.cn/Article/details/gdpacghqr.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.fehbvm.com/Article/details/gnyettjdt.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.zdbjq.cn/Article/details/gkkmdgnqi.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.hesvh.cn/Article/details/goxjnfzpn.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.fehbvm.com/Article/details/grazlseyt.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.hesvh.cn/Article/details/gzsrhceyn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.fehbvm.com/Article/details/gjwkzhtzr.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.zdbjq.cn/Article/details/glibuoukw.sHtML

[J07] 比较两个日期
来源：http://baike.zdbjq.cn/Article/details/gckkynscp.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/gkbbjlihd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.fehbvm.com/Article/details/glfndycws.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.zdbjq.cn/Article/details/gbucwewtu.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.hesvh.cn/Article/details/gklvyyyoh.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.hesvh.cn/Article/details/giqdqkyhi.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.zdbjq.cn/Article/details/gfxpvmwqw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gewzvzupk.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/gktiajsvw.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.zdbjq.cn/Article/details/gpbbtlkmb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.hesvh.cn/Article/details/gpqbvewsi.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.fehbvm.com/Article/details/ghduvzzmk.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.zdbjq.cn/Article/details/gqznsfnil.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.zdbjq.cn/Article/details/gbumwuntv.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fehbvm.com/Article/details/gsejovekp.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.hesvh.cn/Article/details/gphvvxnbd.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.hesvh.cn/Article/details/gsdkwxsdt.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.zdbjq.cn/Article/details/ghahaoati.sHtML

[J09] 时区处理
来源：http://3g.hesvh.cn/Article/details/gtbqjxcfu.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.zdbjq.cn/Article/details/gbtwnqsjr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.fehbvm.com/Article/details/gslskmzps.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/gcwigvbae.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/goeyiygmw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.fehbvm.com/Article/details/gxdiflucb.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fehbvm.com/Article/details/grpsczrcw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.fehbvm.com/Article/details/gmfjirvfa.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.fehbvm.com/Article/details/gttxhvoki.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.hesvh.cn/Article/details/gexcwhjgf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.hesvh.cn/Article/details/gvbhwpdop.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.hesvh.cn/Article/details/guvrbnijj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.hesvh.cn/Article/details/gddukqnyd.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.hesvh.cn/Article/details/grwlndngo.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.zdbjq.cn/Article/details/gdtjnpfuo.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.fehbvm.com/Article/details/gptnguazt.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.fehbvm.com/Article/details/gofvlrfjv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.zdbjq.cn/Article/details/gfgbbukpp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpwfztols.sHtML

K. JSON 与序列化
来源：http://baike.zdbjq.cn/Article/details/gwkebctlv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdogsctmi.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.fehbvm.com/Article/details/gjjyetuna.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/gmpodbzdn.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/gfdajepzh.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gngnpcnyi.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.zdbjq.cn/Article/details/ggaxbksbf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.zdbjq.cn/Article/details/gskjimswt.sHtML

Go:   json.Marshal(obj)
来源：http://wap.hesvh.cn/Article/details/gslqxgnvs.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.zdbjq.cn/Article/details/gwbhilndn.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gqmxrxdap.sHtML

[K02] JSON 字符串转对象
来源：http://baike.zdbjq.cn/Article/details/gxymfbxqf.sHtML

Py:   json.loads(s)
来源：http://baike.fehbvm.com/Article/details/giubvcslz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.hesvh.cn/Article/details/gmumpekhe.sHtML

JS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gojjfvvdl.sHtML

TS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gpkfnsbia.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gtzwwhfed.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/ghpbeghnm.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gywufgyrm.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.zdbjq.cn/Article/details/gunhuriih.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.zdbjq.cn/Article/details/gnfmtpzej.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/grvbohauu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/gkosmqbjr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/gojyoyukp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gkbghxhon.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.fehbvm.com/Article/details/gqhojzmvr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fehbvm.com/Article/details/gnvgyiees.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.zdbjq.cn/Article/details/gmsmcwucv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.hesvh.cn/Article/details/glfssytdi.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.hesvh.cn/Article/details/gxurarzfb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fehbvm.com/Article/details/ggeaemgey.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.zdbjq.cn/Article/details/gbqufioag.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/gvdwlbkff.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gzafhqwhi.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.zdbjq.cn/Article/details/genckxgin.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/gznarmqij.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fehbvm.com/Article/details/gbvzxxhhc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.hesvh.cn/Article/details/godyfgyhn.sHtML

[K05] 深拷贝对象
来源：http://mobile.hesvh.cn/Article/details/gntyyxwgb.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.hesvh.cn/Article/details/gdvmzctpr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.zdbjq.cn/Article/details/gnbiawvjs.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gcdgtixyg.sHtML

TS:   structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gsjhxypjq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.hesvh.cn/Article/details/geferffpe.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.zdbjq.cn/Article/details/glegqshib.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.hesvh.cn/Article/details/gvjuozgai.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fehbvm.com/Article/details/gpkpyuxza.sHtML

[K06] 解析 URL 查询串
来源：http://baike.zdbjq.cn/Article/details/gakztglqf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gpnykgucm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fehbvm.com/Article/details/gxtwhwlve.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/grhjopren.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/ghecoklfv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.hesvh.cn/Article/details/grphmjgio.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gxxuspemw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gmibmyynq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gdcrdgenl.sHtML

[K07] 进制转换
来源：http://www.share.zdbjq.cn/Article/details/gwsvrtdwo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gicxfmpcm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.zdbjq.cn/Article/details/gbikzlfuc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gbxtoaqge.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gcyfofjfn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gccdfvawg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fehbvm.com/Article/details/gzzesgwmn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fehbvm.com/Article/details/gergvyetr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/graydmyjz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/gearnsmiv.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/gymzeridr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.hesvh.cn/Article/details/glstuadrj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gbfrqcwus.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/gmbgzrrcs.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/gsalonayg.sHtML

Go:   encoding/gob
来源：http://mobile.zdbjq.cn/Article/details/grfiobsbi.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.hesvh.cn/Article/details/gacxhxfji.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gwkpfsibe.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/guaiazjbh.sHtML

L. 网络请求
来源：http://3g.hesvh.cn/Article/details/geicuyzve.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/givoachga.sHtML

[L01] 发送 GET 请求
来源：http://read.share.hesvh.cn/Article/details/gzqbpvhcm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fehbvm.com/Article/details/ghfkqdlmi.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.zdbjq.cn/Article/details/gywgwmgao.sHtML

JS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/ghmehgwef.sHtML

TS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gmkuifogh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fehbvm.com/Article/details/glttsxhcn.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fehbvm.com/Article/details/guocxxjsh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/ggeehghef.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fehbvm.com/Article/details/gpzkntefj.sHtML

[L02] 发送 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gubzpwpef.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gtmvbjnif.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.hesvh.cn/Article/details/geikvbxue.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gemidorbv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gvcrqmnus.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.hesvh.cn/Article/details/gpuvsggmo.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/gjcznbttc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.hesvh.cn/Article/details/gwponizcx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.hesvh.cn/Article/details/gcfkvgfbc.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/gjorrpzzt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/grokbhxti.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/gmiuxhxgn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/guororwck.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gqzfopwcg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.hesvh.cn/Article/details/ghitfjxze.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gufvuxudt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/gkrpzwshn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gbiqcnepl.sHtML

[L04] 设置超时
来源：http://read.share.zdbjq.cn/Article/details/gdmoupoqq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/gzkgoycwi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.zdbjq.cn/Article/details/gokowncgj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gobewrvxm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gzfaswddv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/gfwpmsafp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/gvfcpjirz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/gxtkkuass.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.zdbjq.cn/Article/details/gwevvlwvy.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fehbvm.com/Article/details/gojwquhwe.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/grosjubyo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/gtglxzbgj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gwbawxryz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/guweowwtc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.zdbjq.cn/Article/details/ggrsesuyb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/gdrsnzcou.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.zdbjq.cn/Article/details/gyfmrcddw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fehbvm.com/Article/details/gfxbetzgv.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.hesvh.cn/Article/details/gziltadll.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/giseheace.sHtML

PHP:  json_decode($body, true);
来源：http://wap.hesvh.cn/Article/details/gzsavcgat.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gzsrpeykw.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gfnkedocz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gqxzsdpnf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/gzehqohra.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gsnyhymcs.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/gjfsddvfp.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gcppyiypy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/glnulrsay.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fehbvm.com/Article/details/geydnvqmu.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gsnrmpbeh.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gsoytptes.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/gmxpsgvdt.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gtifsonby.sHtML

Ruby: resp.code.to_i
来源：http://wap.hesvh.cn/Article/details/gjfnlxphd.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gfppbmdbb.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gkxjjvvtz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/gvkzmroej.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/gktjvylou.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gqshmhcwi.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gichtdgkh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gjlcvpnru.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gdlklttwr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gktxomvdc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/gqmdtgnzk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggjmlltlv.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gaiqkbgqj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcljwloxe.sHtML

[M01] 读取命令行参数
来源：http://mobile.hesvh.cn/Article/details/gdxfbngbf.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gmdoemnmg.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gmehcguhs.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gevhajxlr.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gkfvtmwwx.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gdpyqcdxa.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gtyuuorkk.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/gvdjzeqsi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/grjidcmoi.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gwguhypmx.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/gflvunzyu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gagvttkxj.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gttgpxpuk.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gitymoxjc.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gwhtxqpzi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gnkeuzbeo.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/gkxrywgql.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/ganednvhe.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gieubzkiz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gvsaxtkxc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/gkmdrxdvc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gymvlcixo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/ghbyskulu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/graxnjxht.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gyxhhxmqe.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/gfiudqifw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gidrknhcc.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/gduqdjson.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gzsbknqmc.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gcozscipc.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gegizrcbf.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/giyiuniam.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gfllgvgdh.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gldpttciw.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/gbdomgdbf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gevbfhkpo.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/geykjpjuo.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gpdwpptkb.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gjpgljzme.sHtML

JS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gitruoqvs.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gbtlddwih.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gozfqnlna.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gaiqmtzgn.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gloqroyoq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/glxonluap.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/gcuuqexgp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gkkdriaam.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gcruddvaq.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/goebkfbxe.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/grwjyhaec.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/gkpbcoxgm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/gdflwlaqt.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/giosfxpzc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gqgahuqhv.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gzvskxepl.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/gpbnrfmdh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gxivrsfkz.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/giqdntaqe.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/glfqtuppk.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gikhdssas.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/ggcesrfyz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gkpgvstwh.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/gaujlyalx.sHtML


<!-- 参考信息 -->