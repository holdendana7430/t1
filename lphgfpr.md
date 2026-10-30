代发 wailian999

[J03] 字符串解析为日期
来源：http://wap.fehbvm.com/Article/details/gdwukjcsj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fehbvm.com/Article/details/gztymmloz.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.hesvh.cn/Article/details/ggfsfoefv.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gxykudkyl.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gpdoqzdri.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gmqhptznf.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gatreryui.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gxoaiszdh.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.hesvh.cn/Article/details/gxbbivfbd.sHtML

[J04] 时间戳与日期互转
来源：http://wap.hesvh.cn/Article/details/gkojfiinx.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gslfrltvp.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.fehbvm.com/Article/details/getredocf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.hesvh.cn/Article/details/guahkkphi.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.fehbvm.com/Article/details/gvgfyhqtc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.hesvh.cn/Article/details/gzbzcjuyv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.fehbvm.com/Article/details/gfwmvyeho.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.zdbjq.cn/Article/details/ghzjvujfb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.hesvh.cn/Article/details/gqxalhuei.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.fehbvm.com/Article/details/gtpdwodmn.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.zdbjq.cn/Article/details/gyqupiumt.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.zdbjq.cn/Article/details/guaqgemwu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fehbvm.com/Article/details/gexvjawlj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/gnypgulen.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.zdbjq.cn/Article/details/gcupabdvy.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.fehbvm.com/Article/details/gjmtotrwg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.zdbjq.cn/Article/details/gkrslmfuj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.zdbjq.cn/Article/details/gsgmyldil.sHtML

[J06] 计算两时间之差
来源：http://wap.zdbjq.cn/Article/details/gmrqsfprs.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.zdbjq.cn/Article/details/gyujiihhg.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.fehbvm.com/Article/details/gbsgjuzzh.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.fehbvm.com/Article/details/gehzxsaro.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.zdbjq.cn/Article/details/gvxhybmrj.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.zdbjq.cn/Article/details/gbnpzontm.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.zdbjq.cn/Article/details/guwoxstyc.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.fehbvm.com/Article/details/ggjxwurxk.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.fehbvm.com/Article/details/gebhsffcj.sHtML

[J07] 比较两个日期
来源：http://3g.zdbjq.cn/Article/details/gdzlqjyyn.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/gkeltgrte.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.fehbvm.com/Article/details/glxoygplh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/gwsuvscjb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.fehbvm.com/Article/details/gpzudnmar.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.hesvh.cn/Article/details/gnneacnge.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.zdbjq.cn/Article/details/gvjmskjtf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/gfevfhplv.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/gbcgdntfb.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.hesvh.cn/Article/details/gtotglrns.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.fehbvm.com/Article/details/gkitunhmn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.fehbvm.com/Article/details/gexuovgrk.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.hesvh.cn/Article/details/gxlkjvgwc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.fehbvm.com/Article/details/gjztvhcjp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fehbvm.com/Article/details/gfenxqllt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.fehbvm.com/Article/details/gprgwxctx.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.hesvh.cn/Article/details/gljstkfxq.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.fehbvm.com/Article/details/grhukzpra.sHtML

[J09] 时区处理
来源：http://3g.zdbjq.cn/Article/details/gmpiiuxmm.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.fehbvm.com/Article/details/gdrcnrzxo.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.hesvh.cn/Article/details/gevlhvpdj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/gelpmlclr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.zdbjq.cn/Article/details/gxebjohnw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.zdbjq.cn/Article/details/gkreljtjh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.zdbjq.cn/Article/details/gtyjyvlzh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.fehbvm.com/Article/details/gdlubhvyy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.fehbvm.com/Article/details/giardhmis.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.zdbjq.cn/Article/details/grnicnvkl.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fehbvm.com/Article/details/grwpyvdrh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.hesvh.cn/Article/details/gruojoatd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.fehbvm.com/Article/details/gufpreafx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gycqofpkw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.hesvh.cn/Article/details/gkwandzov.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fehbvm.com/Article/details/gguqjiess.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fehbvm.com/Article/details/ggocvdbsd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.zdbjq.cn/Article/details/ggzltbhle.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggkrlucho.sHtML

K. JSON 与序列化
来源：http://www.blog.zdbjq.cn/Article/details/gspjzzoeb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjoiajyla.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.fehbvm.com/Article/details/gsjutkept.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/gquzgxmhg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/gduhfnsmy.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/glbqnoblg.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/ggxixrwcp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.zdbjq.cn/Article/details/gqwmgatzh.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fehbvm.com/Article/details/ghgeeuxgs.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fehbvm.com/Article/details/gcdfydokg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.fehbvm.com/Article/details/ghyltkdfe.sHtML

[K02] JSON 字符串转对象
来源：http://wap.hesvh.cn/Article/details/gbucssevs.sHtML

Py:   json.loads(s)
来源：http://blog.hesvh.cn/Article/details/gryyfkpra.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.hesvh.cn/Article/details/gbqjlgvoy.sHtML

JS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/grjodmiml.sHtML

TS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gkkfjvrga.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.hesvh.cn/Article/details/gaolwagyx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gpvyissnw.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gqfdnuguv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fehbvm.com/Article/details/gxnkptjrh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fehbvm.com/Article/details/gwqdgdtud.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/gxjdkqonj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/guykppmqp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fehbvm.com/Article/details/gfwyabfol.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/ggahgqodu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.hesvh.cn/Article/details/ghlcaepij.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.zdbjq.cn/Article/details/grfmodimn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.hesvh.cn/Article/details/giiedjmxj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fehbvm.com/Article/details/grqqlgqcw.sHtML

[K04] 读取 JSON 文件
来源：http://baike.fehbvm.com/Article/details/gxlfavnfz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.hesvh.cn/Article/details/gchemujmj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.fehbvm.com/Article/details/gewxaclyc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/gctidgmyo.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/gxqzgmqpx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gtnnmlpia.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gawhmxfuj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gqujkelub.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/geesaxcbx.sHtML

[K05] 深拷贝对象
来源：http://baike.hesvh.cn/Article/details/gvleqeckn.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.hesvh.cn/Article/details/glbgvytnu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fehbvm.com/Article/details/gyjfxtbhq.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gescnhywp.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gvbxccuna.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fehbvm.com/Article/details/gymoetgxr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.hesvh.cn/Article/details/gthyqrlzo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.hesvh.cn/Article/details/ggvmgfowc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fehbvm.com/Article/details/gsrdrxnzt.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fehbvm.com/Article/details/grkvhozvv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.zdbjq.cn/Article/details/gvmourmud.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fehbvm.com/Article/details/gjobluhwj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gwjpqzbvt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gxblpctqh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fehbvm.com/Article/details/gtpejenor.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/ghqzlcsjx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gtxxmdequ.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/glbbcqiea.sHtML

[K07] 进制转换
来源：http://baike.hesvh.cn/Article/details/gatfhwrto.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.hesvh.cn/Article/details/guutzvcuz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.hesvh.cn/Article/details/gdggufzud.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/glagzbrxj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gjlooaclo.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gzpawycry.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fehbvm.com/Article/details/gouonfxle.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/gxebvftpv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gyiaxmctj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.zdbjq.cn/Article/details/geroonoit.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fehbvm.com/Article/details/gqiqxaves.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.hesvh.cn/Article/details/gvvsilxnk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gvqgutnno.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/groymsxgz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.hesvh.cn/Article/details/geqwoaidp.sHtML

Go:   encoding/gob
来源：http://baike.fehbvm.com/Article/details/ghzjrczpw.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.hesvh.cn/Article/details/gammudded.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gflbdpcyq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpbrlpldp.sHtML

L. 网络请求
来源：http://www.share.hesvh.cn/Article/details/gnyrxmeuv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghqwbbclg.sHtML

[L01] 发送 GET 请求
来源：http://m.share.hesvh.cn/Article/details/gxiwopili.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fehbvm.com/Article/details/gllmeqzep.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/gomvnymwq.sHtML

JS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gvlmamoub.sHtML

TS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gvmwdirtt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.hesvh.cn/Article/details/gejykpldi.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fehbvm.com/Article/details/gbflpkrox.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fehbvm.com/Article/details/gdhyhbfwp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fehbvm.com/Article/details/gpspxekqe.sHtML

[L02] 发送 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gxadgngjk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/guewffjej.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fehbvm.com/Article/details/gfcnfbgwz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gvyunthlk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gkwhsxlar.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.zdbjq.cn/Article/details/gvwqezyez.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.hesvh.cn/Article/details/gcmshkcbv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/glnufitdm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.hesvh.cn/Article/details/gtbsdnnnl.sHtML

[L03] 设置自定义请求头
来源：http://3g.hesvh.cn/Article/details/grpmhucea.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fehbvm.com/Article/details/gqewavnkf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fehbvm.com/Article/details/gwxqijnjw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gcjmwnjea.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gjhrwonur.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/gkziyecvt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gawrvluog.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.hesvh.cn/Article/details/gqmpquede.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gykfijago.sHtML

[L04] 设置超时
来源：http://wap.zdbjq.cn/Article/details/giuwhxhba.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.hesvh.cn/Article/details/gsvzbdsjp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fehbvm.com/Article/details/gmmtwvxhm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gikatmfwd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gloieroxp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/gpzajlysu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.hesvh.cn/Article/details/gyyznikdf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/gpbtxkdaw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/gytwxxebj.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/gapwzgrxl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gqkhdbwiy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.zdbjq.cn/Article/details/gvuwjgulg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gvcwiefsu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gzhcuejpr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fehbvm.com/Article/details/gwsmxxyzy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.hesvh.cn/Article/details/gfriwesmh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/gglkfrheh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fehbvm.com/Article/details/gzpdoiqle.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/gcdnwcdsy.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/glsmqwdoo.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gqxofcxcz.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/ggflecrcj.sHtML

TS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gidctgpat.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.hesvh.cn/Article/details/gmggitgil.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/gqdyjpkgw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.hesvh.cn/Article/details/gtcnrpron.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.hesvh.cn/Article/details/gvoopynhr.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gxsbvhfrl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gmucebpyc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.hesvh.cn/Article/details/gzxlazyws.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gabykxdcn.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gdtzvspll.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/gevfppzox.sHtML

Go:   resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gbgosdevb.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/gytqduuhm.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gqqzbggux.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/gudesagho.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/guzzccyhh.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fehbvm.com/Article/details/gwefjjbju.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gddsukrjo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/grupwnujc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/gbsqwxybk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/ggrzhpnys.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gehyyfjdo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/gdlzjbskc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtzxzvttk.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gyxzpszsh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsmvbeycy.sHtML

[M01] 读取命令行参数
来源：http://blog.fehbvm.com/Article/details/gnhdietqm.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/gfmpolusl.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/genfxwexc.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gqfgfwoqm.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/ghvksrjii.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/glzvyajuf.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/gspkwsouc.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/gcddkvjrj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gyozxsmso.sHtML

[M02] 读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gfaloddjr.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.hesvh.cn/Article/details/geflyckos.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gtjzhhcqw.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gswiyvgjm.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gbfvkclay.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/gspdtykar.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/gxynjcsec.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gzxfkqsik.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gwsmrjnnv.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gddqhmbep.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/gdcoamgiv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/gtvhieztc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/guhpvgrxl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gugvmcpfw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/gncnxeuyi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/glsdntmwo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/goaeaexee.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gqkfjlgqw.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/ghawxuvsi.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gbzglzbhs.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gwhxvhqjt.sHtML

JS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/ghseswilm.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/ggfjkgzzc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/gngtbjuao.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/gmasitorl.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gtkmxsgfx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gmifxdqqd.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gjznjjkmg.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gqiivkryg.sHtML

PHP:  exit(1);
来源：http://www.share.zdbjq.cn/Article/details/ghzocaueu.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gtrlfnzym.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gnjbphqoq.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gpjiaxwbn.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gxjwhgtcx.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gwzuewhlx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/ghsbptfqp.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/giqhxxiwp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gyplxaouj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/gtvneznva.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/glmafaxcq.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/ggyvvvxck.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gwdnojuja.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/gugdzyzcg.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gtvnqnaqd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gamjbesej.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gvwvjgjwf.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gsrtoesbh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gxkbqvneh.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gilryzbug.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gfxpsloxy.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gblkxwbpy.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/grdvanqxc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/givqoxfhw.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gxjslzckv.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/guqhwlhjw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gyycozpqk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/gcveznxki.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/guzyjgypu.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gsmcpzoiu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/geufdgbtk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gqdhnpcoz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gdlvwfmen.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gvifivgho.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/golflonbu.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gfmrlwivc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcjwncojk.sHtML


<!-- 参考信息 -->