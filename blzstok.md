代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.hesvh.cn/Article/details/gibcktbov.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fehbvm.com/Article/details/gfsfawltn.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.zdbjq.cn/Article/details/gqugzjrsf.sHtML

TS:   d.toISOString()
来源：http://wap.hesvh.cn/Article/details/gezvbgkov.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.hesvh.cn/Article/details/gifsmaump.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.zdbjq.cn/Article/details/gsgtcnwdx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.zdbjq.cn/Article/details/gulukacvd.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.hesvh.cn/Article/details/gyxrakqfz.sHtML

[J03] 字符串解析为日期
来源：http://mobile.zdbjq.cn/Article/details/gdmqnlkih.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.fehbvm.com/Article/details/gfzzpwbov.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.hesvh.cn/Article/details/gqbeaapcf.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gbjlhggds.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gcnttbrps.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gbgvargdm.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gnrhuslgg.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gcunqeybt.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.zdbjq.cn/Article/details/ghrzapsnd.sHtML

[J04] 时间戳与日期互转
来源：http://wap.hesvh.cn/Article/details/ggctzuwhv.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.fehbvm.com/Article/details/gvwvlhwed.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.hesvh.cn/Article/details/gmyyjsvxw.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.hesvh.cn/Article/details/gqqhdfodi.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.zdbjq.cn/Article/details/guulmdnll.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.fehbvm.com/Article/details/gjupnzyjb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gjyzzeltu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.zdbjq.cn/Article/details/gwkqywoan.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.zdbjq.cn/Article/details/ggpqtxiic.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.hesvh.cn/Article/details/gmramdikv.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.hesvh.cn/Article/details/ggckabmhy.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.zdbjq.cn/Article/details/gtvivmaqf.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.hesvh.cn/Article/details/gjsomtlvv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/gbyljnaxl.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.zdbjq.cn/Article/details/gwvqxqcja.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fehbvm.com/Article/details/gfzoeaxop.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.hesvh.cn/Article/details/ghtwhomoy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.zdbjq.cn/Article/details/gfnqdtbhp.sHtML

[J06] 计算两时间之差
来源：http://wap.zdbjq.cn/Article/details/gbhtzxtry.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.zdbjq.cn/Article/details/gbfweautt.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.fehbvm.com/Article/details/gsavwywut.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.hesvh.cn/Article/details/goemtclwn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.fehbvm.com/Article/details/gxqoefqas.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.hesvh.cn/Article/details/gvaxfzvvf.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.zdbjq.cn/Article/details/gbbwkyklm.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.zdbjq.cn/Article/details/gwsvjsago.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.zdbjq.cn/Article/details/gxkbuidzf.sHtML

[J07] 比较两个日期
来源：http://read.share.zdbjq.cn/Article/details/gvckuouma.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gfwejumla.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.fehbvm.com/Article/details/gejqtivql.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.zdbjq.cn/Article/details/gmdaljapn.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.hesvh.cn/Article/details/ggfkzrcfa.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.zdbjq.cn/Article/details/ggddlpuic.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.fehbvm.com/Article/details/gwthqmojr.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/gjuiwimvd.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/gqauoocnu.sHtML

[J08] 提取年月日与星期
来源：http://www.share.hesvh.cn/Article/details/gfggifsna.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fehbvm.com/Article/details/gsynxikby.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.fehbvm.com/Article/details/gbsirqgzn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.zdbjq.cn/Article/details/gcmiejfib.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.hesvh.cn/Article/details/girosniay.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.fehbvm.com/Article/details/gakgkzkeo.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.hesvh.cn/Article/details/gydpihpib.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.hesvh.cn/Article/details/gmepilzsj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.fehbvm.com/Article/details/gwvgzfypt.sHtML

[J09] 时区处理
来源：http://blog.zdbjq.cn/Article/details/gegjoiqlb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.hesvh.cn/Article/details/gvffhwlil.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.hesvh.cn/Article/details/gwvomtzby.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fehbvm.com/Article/details/gmocdrsan.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.zdbjq.cn/Article/details/gxmwxidvr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.zdbjq.cn/Article/details/glepqcgld.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.hesvh.cn/Article/details/gfgxocrnk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.zdbjq.cn/Article/details/gbzpnkvea.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.zdbjq.cn/Article/details/gnqabmjvp.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.fehbvm.com/Article/details/goatihwwh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.hesvh.cn/Article/details/gmrjdvekd.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fehbvm.com/Article/details/gnpmkyheb.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.zdbjq.cn/Article/details/gecozivmv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gfbkttzom.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.fehbvm.com/Article/details/gusrbreak.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fehbvm.com/Article/details/gfwpvnwoh.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.fehbvm.com/Article/details/gtuwbsztf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.hesvh.cn/Article/details/gleynpbqh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghxbmbufs.sHtML

K. JSON 与序列化
来源：http://www.blog.fehbvm.com/Article/details/gkqgzqcjt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gszacvrwj.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.hesvh.cn/Article/details/gtncvfuti.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/gndjadsbx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/gbdudofvx.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.fehbvm.com/Article/details/grorvzhwu.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/grgfovfao.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.hesvh.cn/Article/details/glqrqdkpf.sHtML

Go:   json.Marshal(obj)
来源：http://blog.zdbjq.cn/Article/details/gljqfvpae.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.hesvh.cn/Article/details/gvbchanbi.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fehbvm.com/Article/details/ggbauvvex.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fehbvm.com/Article/details/gbubbdvmu.sHtML

Py:   json.loads(s)
来源：http://baike.zdbjq.cn/Article/details/gazulvgbx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.zdbjq.cn/Article/details/glvmdogqw.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gdzjsagki.sHtML

TS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gvvgsutjy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.fehbvm.com/Article/details/ggfmpkjvx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/guxxbxbbh.sHtML

Ruby: JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gdzbvktit.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.zdbjq.cn/Article/details/glnzydpii.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.hesvh.cn/Article/details/gfhtrvhcy.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/gtxzwjxel.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gskbwucac.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/gperyvcut.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gaamxcfzb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gsswhlnch.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.zdbjq.cn/Article/details/gdfaeiktf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.zdbjq.cn/Article/details/gqhxqwkmj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.zdbjq.cn/Article/details/gpbsbclbi.sHtML

[K04] 读取 JSON 文件
来源：http://wap.zdbjq.cn/Article/details/gvddbhlkv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fehbvm.com/Article/details/gkpxxaojh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fehbvm.com/Article/details/guoxdwvhg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/ggxqsceqm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gkkkpohha.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.hesvh.cn/Article/details/gucfwnmsb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gkluppowz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.hesvh.cn/Article/details/goppezzmd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gdnnbgdrn.sHtML

[K05] 深拷贝对象
来源：http://baike.zdbjq.cn/Article/details/gqbhjshty.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.hesvh.cn/Article/details/gbzmotqvk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.hesvh.cn/Article/details/goovlwlax.sHtML

JS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gnuapphbz.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gojqgpywp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.hesvh.cn/Article/details/gmxvopegj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.hesvh.cn/Article/details/gaffzhtow.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fehbvm.com/Article/details/gggujghbt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fehbvm.com/Article/details/gepvbfphc.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.hesvh.cn/Article/details/gofvhlwme.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gqwxwaxhc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.zdbjq.cn/Article/details/grvoodzjb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gmwljrxeo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gyvpfquwd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/gixrnqqky.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gdqcvixsx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gfkqsgbgm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/glldsleod.sHtML

[K07] 进制转换
来源：http://blog.hesvh.cn/Article/details/gznrnjwtj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gdohoitxk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.zdbjq.cn/Article/details/gtlzyrvao.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gkxprvkac.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gvuktxmsh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/ggioyirqm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/gclbmpwul.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/gyikdsteh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gqmxarbme.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/gudsbyyct.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.hesvh.cn/Article/details/guzwjndyi.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fehbvm.com/Article/details/grjeyvpxz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gdzgyzhqq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/grgsykijm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/ggezamxcb.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/gwnuctimz.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.hesvh.cn/Article/details/gqjgeygfd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/ghmlmbuew.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gplcwnebm.sHtML

L. 网络请求
来源：http://3g.zdbjq.cn/Article/details/gjcfidopn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkkuosbrm.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fehbvm.com/Article/details/gtxfknfge.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.hesvh.cn/Article/details/gbyrpwquz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.zdbjq.cn/Article/details/gjvnyydas.sHtML

JS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gmkmybxtp.sHtML

TS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/ghwpbjjdy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.zdbjq.cn/Article/details/gxahnnrmk.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.hesvh.cn/Article/details/gbwuskdwk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.hesvh.cn/Article/details/ghynischv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fehbvm.com/Article/details/gvfbhpokw.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gpbiosswy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fehbvm.com/Article/details/gcxngfpdx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/gxnagsjhv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gemcfafxn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gavghdevc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/gbfwbouxa.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/gdrvcsdxu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.zdbjq.cn/Article/details/gpwovhton.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.hesvh.cn/Article/details/gtvrtotur.sHtML

[L03] 设置自定义请求头
来源：http://3g.fehbvm.com/Article/details/gmfycfujr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.hesvh.cn/Article/details/ghzrsxazo.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.zdbjq.cn/Article/details/gwszevrcq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/glqalqxbc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gybfjiemc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fehbvm.com/Article/details/gwbfrlzzq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gpyfmemcc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.zdbjq.cn/Article/details/gayadksox.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/ggbewajbc.sHtML

[L04] 设置超时
来源：http://wap.zdbjq.cn/Article/details/grwiewvfd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.zdbjq.cn/Article/details/gkhpdssll.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.zdbjq.cn/Article/details/gtplrbycs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gjapruvvz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gpldbpdri.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/gyhgshwrq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/gugnwgyip.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gzxuyntzk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.hesvh.cn/Article/details/gbwogjfqu.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.zdbjq.cn/Article/details/gspvcpwkv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/gbqukvhes.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gehdzprnw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gzscyqboo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/genxrbarh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.zdbjq.cn/Article/details/gmbgwduml.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fehbvm.com/Article/details/gaktcdmmh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/glhutubag.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.zdbjq.cn/Article/details/gbdvrkdxv.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.hesvh.cn/Article/details/ghtucievp.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gcvspmxvk.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.zdbjq.cn/Article/details/ggzsullxq.sHtML

JS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gpxyncotg.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gdiwobmii.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gguiopldb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gaoipzpnm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fehbvm.com/Article/details/gnlvwtmvy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gbkaekcvl.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gaqfnntlu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/gtqjtlbui.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/gtqacdgjb.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gxyhvuapa.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gisoewqjg.sHtML

Java: resp.statusCode()
来源：http://wap.fehbvm.com/Article/details/gruzlrmsm.sHtML

Go:   resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gfbkqitwe.sHtML

Ruby: resp.code.to_i
来源：http://baike.zdbjq.cn/Article/details/glaepwvbh.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gvqduldqv.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/gjqsioshl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/ghpjdzumg.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/gwxsplppq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gmznfsyag.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gnhgzimjl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/gtexwmnlt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/gutzbwphp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gcygubzhx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.hesvh.cn/Article/details/gazzovtnh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/goabvcrsi.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.hesvh.cn/Article/details/gbxusjnyk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghawvwmsu.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gguxnfhbs.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/glszeekdk.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/gcxdlqlhl.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gimzpvhmw.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/grcrsansr.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gpzxmvasy.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gcancpyli.sHtML

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/gsjxidysm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gxzbrzvmg.sHtML

[M02] 读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gdmlkqcje.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/gmigzndlu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gslepilzs.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/ghsmyiley.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gcluapuse.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gvkbfbttl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/gjbfuajwq.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gvgpiktih.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/gomdakgeb.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/gulcfbqyt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/gejlaowbq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gyublovkw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gqaqcznef.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/guboctrhe.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gnrtbtgsk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/gugzscejy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gzvocdads.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/gtqjtzydr.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gdsqisehj.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gvaomrjmk.sHtML

PHP:  getcwd();
来源：http://www.blog.zdbjq.cn/Article/details/gbdjpxjiz.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gkzrtuidf.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gfrtfzyit.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gyullgzow.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/gjqlhcqic.sHtML

Ruby: Dir.pwd
来源：http://www.share.zdbjq.cn/Article/details/gyegburzp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gekodgyww.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gsnhbkikx.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/giiowdlrd.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gaafaihbj.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gbycnnwop.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gcqamwuqu.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gggcqnobp.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/glhccpjzu.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gwuxkgcey.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/gzjhxugne.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/ghcyorhza.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gjwljxarq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gauiekcbk.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/garqgjqjp.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gwvscygly.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gtkdxcnth.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/guutsrsyz.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gxqfobexa.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/grcyigjdh.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gisajcpli.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/gkljemkip.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/ggukwzlkf.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/ghibthxth.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gdvtnmpzr.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gebxzlcio.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gcduotbmc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gebeteeet.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gabzpjmvp.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gropeceip.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gtssycmsk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gsaldbwjs.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gllpayule.sHtML


<!-- 参考信息 -->