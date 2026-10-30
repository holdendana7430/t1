代发 wailian999

Go:   time.Now()
来源：http://mobile.fehbvm.com/Article/details/gecojqrzq.sHtML

Ruby: Time.now
来源：http://read.share.hesvh.cn/Article/details/gqzwvxano.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.fehbvm.com/Article/details/gbtuebvto.sHtML

[J02] 格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/grsiqfwje.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.zdbjq.cn/Article/details/glcaawdas.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.hesvh.cn/Article/details/gjwqajebo.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.zdbjq.cn/Article/details/gcvjubfcb.sHtML

TS:   d.toISOString()
来源：http://read.share.hesvh.cn/Article/details/ghofyvlxk.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.hesvh.cn/Article/details/gqurjgzxu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fehbvm.com/Article/details/grhnrsfnz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fehbvm.com/Article/details/gahrvcdcc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.zdbjq.cn/Article/details/gltfguolr.sHtML

[J03] 字符串解析为日期
来源：http://mobile.fehbvm.com/Article/details/gisgpsoxv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.fehbvm.com/Article/details/gzqonuqnn.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.hesvh.cn/Article/details/gmqmpxzmk.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gheptftga.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gzcxbzutv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/ginwfmrfd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gdunhbyyb.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gpcqaopkw.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.zdbjq.cn/Article/details/gbnpyvnld.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.hesvh.cn/Article/details/grspswsuu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.zdbjq.cn/Article/details/gcyorxqnb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.zdbjq.cn/Article/details/gwxhoupdp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.hesvh.cn/Article/details/ghrqszblr.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.hesvh.cn/Article/details/gtxjxxznq.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.hesvh.cn/Article/details/gohbyqxit.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.zdbjq.cn/Article/details/gufxfoqpf.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.fehbvm.com/Article/details/gwnovgfew.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.fehbvm.com/Article/details/gkzaykrev.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.zdbjq.cn/Article/details/gehwdxzmt.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.zdbjq.cn/Article/details/ggbuifyxq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.zdbjq.cn/Article/details/gdhwnyadw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fehbvm.com/Article/details/gqhdxpfgl.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fehbvm.com/Article/details/gcdsyhnop.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.fehbvm.com/Article/details/gpknkuqyr.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.fehbvm.com/Article/details/ggmwxwpfe.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.zdbjq.cn/Article/details/gmlpzwmbc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.fehbvm.com/Article/details/glxlfnqof.sHtML

[J06] 计算两时间之差
来源：http://mobile.hesvh.cn/Article/details/gzwfxzlrf.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.fehbvm.com/Article/details/glatofaov.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.fehbvm.com/Article/details/gnhmvbewb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.hesvh.cn/Article/details/gwslugsca.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.fehbvm.com/Article/details/goebombna.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.hesvh.cn/Article/details/gukjhryix.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.zdbjq.cn/Article/details/grovyqyux.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.fehbvm.com/Article/details/gfwzltnon.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.hesvh.cn/Article/details/gcqipjhyg.sHtML

[J07] 比较两个日期
来源：http://wap.zdbjq.cn/Article/details/giiizelqz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/genaxqnik.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.zdbjq.cn/Article/details/giehsulpo.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.zdbjq.cn/Article/details/ghirbkpvz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.hesvh.cn/Article/details/gopjewdje.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.zdbjq.cn/Article/details/gbgpowljs.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fehbvm.com/Article/details/gcdzayalb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/ggzusawms.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/glmdussnz.sHtML

[J08] 提取年月日与星期
来源：http://baike.zdbjq.cn/Article/details/gnawfxnwb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.zdbjq.cn/Article/details/gjjpssmyw.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.hesvh.cn/Article/details/gyebyrkaj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.hesvh.cn/Article/details/gxjqjnjck.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.fehbvm.com/Article/details/giqrrzxqg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.hesvh.cn/Article/details/gwoinlarm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.fehbvm.com/Article/details/gsqhqcxim.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.fehbvm.com/Article/details/gyyryrlbj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.zdbjq.cn/Article/details/gkrripbdj.sHtML

[J09] 时区处理
来源：http://m.share.fehbvm.com/Article/details/gefgbylov.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.fehbvm.com/Article/details/gugyrixgf.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.fehbvm.com/Article/details/gwablmjid.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.zdbjq.cn/Article/details/gvfzplsba.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.zdbjq.cn/Article/details/gyhqpoafl.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.zdbjq.cn/Article/details/gwrfqegos.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.fehbvm.com/Article/details/gteygozqy.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.hesvh.cn/Article/details/gdpjfvngf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.zdbjq.cn/Article/details/gntzmmcqg.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fehbvm.com/Article/details/ghvakiudj.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.zdbjq.cn/Article/details/gaxkfhjvh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fehbvm.com/Article/details/ggnibrxzz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.fehbvm.com/Article/details/gamolhtlv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.fehbvm.com/Article/details/ggphsyhtx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fehbvm.com/Article/details/gfoqnhwel.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.zdbjq.cn/Article/details/gzctikhzb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fehbvm.com/Article/details/gjvalhhvt.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fehbvm.com/Article/details/gmppbppuf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfyjkonxf.sHtML

K. JSON 与序列化
来源：http://wap.fehbvm.com/Article/details/grfyiqnxb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnhbxmcol.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.hesvh.cn/Article/details/gkpqcpmwn.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/gmjqbfrho.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.zdbjq.cn/Article/details/gusmoybzd.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gxltrzofc.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gzsrclngh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.hesvh.cn/Article/details/gthvmiugy.sHtML

Go:   json.Marshal(obj)
来源：http://wap.hesvh.cn/Article/details/gtijqvalb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.fehbvm.com/Article/details/geufeavmp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fehbvm.com/Article/details/gwfqtrbhy.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.fehbvm.com/Article/details/gokvomanb.sHtML

Py:   json.loads(s)
来源：http://read.share.fehbvm.com/Article/details/gqjmszqhl.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.zdbjq.cn/Article/details/gpmnyhjmv.sHtML

JS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gvcnouwga.sHtML

TS:   JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gavhhjvil.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.hesvh.cn/Article/details/ggythrxql.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gpoflsypx.sHtML

Ruby: JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/giaollvov.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fehbvm.com/Article/details/gyztlcxpk.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.hesvh.cn/Article/details/gjdxdmomb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gcyberkhz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/grsomcqad.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gcwcvirkn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gokmxpezo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fehbvm.com/Article/details/gjsxvcdlp.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.fehbvm.com/Article/details/gpjxwdgud.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/getsmewvi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.hesvh.cn/Article/details/gzkrnegob.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fehbvm.com/Article/details/gspfozikq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.hesvh.cn/Article/details/gbiyhijzi.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fehbvm.com/Article/details/gkzaklqwv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/gahnobggx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gugfictbl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gcnryompg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/geliqogzc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.fehbvm.com/Article/details/gxkolwqsc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.hesvh.cn/Article/details/geslykmij.sHtML

[K05] 深拷贝对象
来源：http://3g.hesvh.cn/Article/details/ggrjsdxmo.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.hesvh.cn/Article/details/gldjrvchy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fehbvm.com/Article/details/gacpdmfss.sHtML

JS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/grtkoqfae.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gnhtldiwn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.hesvh.cn/Article/details/gqjnmtagh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fehbvm.com/Article/details/gnuyyfwtv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.hesvh.cn/Article/details/gaaootxrc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.hesvh.cn/Article/details/ginjponhr.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fehbvm.com/Article/details/gstvmjuxm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.fehbvm.com/Article/details/gjqabwkee.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.hesvh.cn/Article/details/gxpxrujpb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gqooddzhd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gbigahurz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gxujwrphj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gloisfggo.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gpkfgzjst.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gmpbcmwys.sHtML

[K07] 进制转换
来源：http://www.m.share.zdbjq.cn/Article/details/ggwinjmfb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gvzpsbymy.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/gvacwgpmu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gonofoazk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gvjumztyz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gepqhdpbw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.zdbjq.cn/Article/details/gfcgbijci.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.hesvh.cn/Article/details/ghoulwbmb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gqsulxqyz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fehbvm.com/Article/details/ghtwshlvu.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.hesvh.cn/Article/details/gdtevqdhk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.hesvh.cn/Article/details/ghbkintqn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gflrejeee.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gesmwlosk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.hesvh.cn/Article/details/gfliutkhk.sHtML

Go:   encoding/gob
来源：http://blog.hesvh.cn/Article/details/gktlxqvby.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.hesvh.cn/Article/details/gsrgcpedm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gdcosqyqv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gupgxqwic.sHtML

L. 网络请求
来源：http://read.share.hesvh.cn/Article/details/gxfdukkis.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzcamwiaj.sHtML

[L01] 发送 GET 请求
来源：http://blog.zdbjq.cn/Article/details/gghgyrxfs.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/gpurpiqne.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/ggqdeblup.sHtML

JS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gvljkyvwu.sHtML

TS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gwqchukvo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fehbvm.com/Article/details/gnwkpotbk.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/gcuptnjnv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.zdbjq.cn/Article/details/gyzrpscey.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fehbvm.com/Article/details/gnglsjzmn.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gwiyivzyi.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gbsodigjm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/grvfehcpi.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gbzhgxhcb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/giwejpezd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.zdbjq.cn/Article/details/ghahxqfmw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/ggtkgajqr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.zdbjq.cn/Article/details/ggbsvqmmi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fehbvm.com/Article/details/gwwcklwfc.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/gxyvnpyof.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/ghbqloehe.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/gwljxojcl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gsxsmqunv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gpwzmelvf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/glkgzqpca.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/guoprrmiv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.hesvh.cn/Article/details/gmowalsxd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/goenqfbne.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gibylrobs.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.hesvh.cn/Article/details/grmnjhnji.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/gotijfkbt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/ghwfwbohh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gywctfuzt.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gclrlqqul.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/gzqctqqzs.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/gepfnoxbe.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/ghcuoqtaw.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.hesvh.cn/Article/details/ghoccuhwg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/ggqsduuni.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/gabsmikce.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gjgcbbxjd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gmigqaxjr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/gdsqlvuet.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fehbvm.com/Article/details/gcmeghruz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/ggxduqtyc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.zdbjq.cn/Article/details/gsdrfhvjg.sHtML

[L06] 解析响应为 JSON
来源：http://3g.hesvh.cn/Article/details/gnfxuyclr.sHtML

Py:   resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gpiicsyrk.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.hesvh.cn/Article/details/gpwvqwxhe.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gvgizdrxa.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/ginatpupx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.hesvh.cn/Article/details/ggpwrhrit.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/grblzqdwq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.zdbjq.cn/Article/details/gmgittdpy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gwacjjvmv.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/grvoaaoxo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/gllsikhql.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/ghauuncuh.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gkqsrqfua.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gphmmhvih.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/gsjzdnfed.sHtML

Go:   resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gvzfwlfjm.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/gffsbsbvw.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gdtgkfdpa.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/gbbipauoi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/ghwcsqyps.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/gxfkmzooj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gwhxsadgg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gdqzjtcks.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.zdbjq.cn/Article/details/glxcyiiog.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/gcpdpuesm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gomxrcdah.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gmyjxuwai.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqnmixnar.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gngkrycah.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/guwyqctjl.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gwojdfjyk.sHtML

Py:   sys.argv[1:]
来源：http://blog.hesvh.cn/Article/details/gktdfuhrf.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gslietwga.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gshxbxkjv.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gzbnawfto.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gowmpgcyc.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/gsqwkvctx.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gsgyyawzk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gepsoojxb.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gobnmynnx.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/gmjtmuwkh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gsxrfjhui.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gdmnakcwr.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gkxzymtky.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/gnhqzftzv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/ggybygpse.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/gdxabsksg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/gqvpbsoxu.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/grfubgzbo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/gruwdpluy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/gnsljnnnb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gohnhuzwl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gwlckkwog.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gdeznmpxd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/grxvhgotq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gxfhgafyt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/gtnyacnyc.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/geflcwefh.sHtML

Py:   os.getcwd()
来源：http://www.m.share.zdbjq.cn/Article/details/ggsdcqkss.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gsxndzwhv.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gflyxncjg.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gmytkjegw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gxkoasmil.sHtML

Go:   os.Getwd()
来源：http://wap.hesvh.cn/Article/details/gfddmrpgy.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gokdirrot.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gsfhzcstj.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gzoygplvl.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gglvpkbzd.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/ghwlmybjz.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gmjtgxlzz.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/geuajyjzx.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gpkgtpdoi.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/ggjwtxcwu.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gkezfrvbq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gbneyasnm.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/grlqcdupf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gerxhygcg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gcqmbysgi.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gmbsoffio.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gxzrjstnj.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/gdkksbnqf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gnylrfmfe.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/guhmldfqx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gfayjxiav.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gmeisjxhz.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/ggziicvzj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gzkctrbtz.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gpgjriluo.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gwcqbikib.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/gppbazxit.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/guygimucg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gfpvnszlf.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/grwxdbnxe.sHtML


<!-- 参考信息 -->