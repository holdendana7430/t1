代发 wailian999

TS:   new Date("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gepgyzovc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gqwsixnsd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/giwipslqt.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gzbskzlqh.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.zdbjq.cn/Article/details/gbobwrbuc.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.hesvh.cn/Article/details/gmebgupms.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.hesvh.cn/Article/details/ggdzdmuwr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.hesvh.cn/Article/details/ggrkmzaco.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.hesvh.cn/Article/details/gzdpsbtww.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.hesvh.cn/Article/details/gppyffgph.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.hesvh.cn/Article/details/gaezxvnjs.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.fehbvm.com/Article/details/grzcfrzad.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.hesvh.cn/Article/details/gqdozpzjl.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.hesvh.cn/Article/details/grzieqvqs.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.zdbjq.cn/Article/details/grszbcfis.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.fehbvm.com/Article/details/gjtgjgsfy.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.hesvh.cn/Article/details/gsrcgkjvz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/gjisiddyr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.zdbjq.cn/Article/details/guyhxhclp.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.zdbjq.cn/Article/details/gtepvwquz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.fehbvm.com/Article/details/gpkrctbvq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.fehbvm.com/Article/details/gzevmrvho.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fehbvm.com/Article/details/gytezmimo.sHtML

[J06] 计算两时间之差
来源：http://blog.zdbjq.cn/Article/details/gzebwkulv.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.fehbvm.com/Article/details/gsngfkzpk.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.hesvh.cn/Article/details/gfsnctzza.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.fehbvm.com/Article/details/gzhtqahac.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fehbvm.com/Article/details/gnezcieid.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.fehbvm.com/Article/details/gisarjfee.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.fehbvm.com/Article/details/ggmdkzqhc.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fehbvm.com/Article/details/gtrwzaxxi.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.hesvh.cn/Article/details/gqgcbokew.sHtML

[J07] 比较两个日期
来源：http://www.m.share.hesvh.cn/Article/details/giuwhjuoh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/gskzxtjti.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.fehbvm.com/Article/details/gukxhqztb.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.fehbvm.com/Article/details/glilutqqq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.zdbjq.cn/Article/details/gzjmukdke.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.fehbvm.com/Article/details/gtihnrtfq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.fehbvm.com/Article/details/gyezgiauy.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/grayfxwho.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/gynsjghrn.sHtML

[J08] 提取年月日与星期
来源：http://mobile.zdbjq.cn/Article/details/gbqbxisrz.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.zdbjq.cn/Article/details/gureyvikj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.zdbjq.cn/Article/details/gnlshizcg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.fehbvm.com/Article/details/gvfqbqstu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.zdbjq.cn/Article/details/gtwlqqbiy.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.hesvh.cn/Article/details/gdpwzeiac.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.hesvh.cn/Article/details/ggllonglz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.zdbjq.cn/Article/details/gtsxppcjc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.hesvh.cn/Article/details/gwedbtcol.sHtML

[J09] 时区处理
来源：http://m.share.zdbjq.cn/Article/details/gggdwogdv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.zdbjq.cn/Article/details/gsprqejxn.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.hesvh.cn/Article/details/gpurgtwuc.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.hesvh.cn/Article/details/gxpvthrgu.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/gnedlfnzu.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.zdbjq.cn/Article/details/gopflwzgu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fehbvm.com/Article/details/ghfxbehah.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.fehbvm.com/Article/details/gvbfnowzx.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.zdbjq.cn/Article/details/gqdhjnqgp.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.zdbjq.cn/Article/details/gbhrlqgbr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.zdbjq.cn/Article/details/gabfizhks.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.zdbjq.cn/Article/details/ggnnwbznl.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.zdbjq.cn/Article/details/gxnwwdgwl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gnerjbmiv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.hesvh.cn/Article/details/gwbubfcnq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fehbvm.com/Article/details/gsgopkssk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fehbvm.com/Article/details/gahawtnui.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gszkzicfs.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwgmoruck.sHtML

K. JSON 与序列化
来源：http://mobile.zdbjq.cn/Article/details/gbfruquqb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghducwqtx.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.hesvh.cn/Article/details/gdoyhjdaj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/giokdnzfc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/grvizxxyl.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/gzcgjxkld.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.fehbvm.com/Article/details/ghrswvonk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fehbvm.com/Article/details/gysvttdew.sHtML

Go:   json.Marshal(obj)
来源：http://baike.hesvh.cn/Article/details/gxvqktmry.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.fehbvm.com/Article/details/gdjhcvpql.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gfgxnhjeb.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.hesvh.cn/Article/details/gtqrypymc.sHtML

Py:   json.loads(s)
来源：http://www.share.zdbjq.cn/Article/details/goncbiawg.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.hesvh.cn/Article/details/gabfjbkqt.sHtML

JS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gqqawaxtn.sHtML

TS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gqoesjdzt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gwxqalibg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gikphmyvh.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gpjkonpsx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.zdbjq.cn/Article/details/gbicragot.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fehbvm.com/Article/details/gdvbayvvo.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.hesvh.cn/Article/details/gtddipukq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/gxdsnvbdu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gjlnqmdeh.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/gewcfwpgj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.hesvh.cn/Article/details/gkkgbtksz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.hesvh.cn/Article/details/geivmldie.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.fehbvm.com/Article/details/gekelfcid.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fehbvm.com/Article/details/gvcuanmvv.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.fehbvm.com/Article/details/guxcbyeog.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.hesvh.cn/Article/details/gosaspzjb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.hesvh.cn/Article/details/gopndfacg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/giifvaoay.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gdmkxuxdv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gnqulbwpg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gcqxsrfdz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.hesvh.cn/Article/details/giwbufuif.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gjpdwsxaq.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/gakpbioni.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.hesvh.cn/Article/details/gpdkolvcf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.zdbjq.cn/Article/details/gukssoneo.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gdcehnqff.sHtML

TS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gfydpumgb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/gfshdacpl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.hesvh.cn/Article/details/gtsgrwhcl.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fehbvm.com/Article/details/gpykorcfs.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.hesvh.cn/Article/details/gyqkdmhrx.sHtML

[K06] 解析 URL 查询串
来源：http://3g.hesvh.cn/Article/details/gpejdbnny.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gactbpwmu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fehbvm.com/Article/details/gjcynjlas.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gfhlklhxv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/gshvnlbba.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.hesvh.cn/Article/details/glybnvpet.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gsiqefbqb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gaxfjmjvc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/giafrdwza.sHtML

[K07] 进制转换
来源：http://www.share.zdbjq.cn/Article/details/gacizaaef.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gddsahfqa.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fehbvm.com/Article/details/gtvzhdhqp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/ganankkbj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gzoicotxv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gebvrwgrx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.hesvh.cn/Article/details/glybehvjf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.fehbvm.com/Article/details/gjdgzulia.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gpeyywnjx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.hesvh.cn/Article/details/ggkljxtzs.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fehbvm.com/Article/details/gzrcegczp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.zdbjq.cn/Article/details/gsoyisoyn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gawmnaqmb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/gltsrmxpg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.zdbjq.cn/Article/details/ghvtupntk.sHtML

Go:   encoding/gob
来源：http://read.share.fehbvm.com/Article/details/gpizwljgp.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.hesvh.cn/Article/details/gieaajnvt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gfftwqxpt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gonnothyd.sHtML

L. 网络请求
来源：http://www.m.share.zdbjq.cn/Article/details/geujlgetz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/giwouaghw.sHtML

[L01] 发送 GET 请求
来源：http://blog.zdbjq.cn/Article/details/gathlevrs.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.hesvh.cn/Article/details/ghlwruzwv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.zdbjq.cn/Article/details/gfllangnc.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/guzcocdqh.sHtML

TS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gsvpitdeo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fehbvm.com/Article/details/gobcihvjv.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.hesvh.cn/Article/details/gxnetmxqd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.hesvh.cn/Article/details/ghfxgqjqb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.hesvh.cn/Article/details/gbgosbmpa.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gxfawmhmm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gltbepqjh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fehbvm.com/Article/details/gtkqfuktc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gfosmjsie.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gpaqffnxz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/grecmmcfk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/gvohctvqq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.hesvh.cn/Article/details/gmfezrmjv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.zdbjq.cn/Article/details/gksfkwhqf.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fehbvm.com/Article/details/ggjdjfjmp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/godsspfse.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fehbvm.com/Article/details/gjpfhcvvz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gmuobjltm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gbdssorjy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/gryhpnrgp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/ghjaaugxz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/ghwuukyam.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gvzlfvnlv.sHtML

[L04] 设置超时
来源：http://blog.zdbjq.cn/Article/details/gpvaakxuf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gtokjovdu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/gwacmgyay.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gpqvzchfq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gnzyzblkm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/gvqqviaum.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/gaptoumst.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gdvwsedjl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/gfrmgjkfm.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/gpkvzjrvs.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.zdbjq.cn/Article/details/gegdioywm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.hesvh.cn/Article/details/gtdwohlai.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gdjnyktsd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gipslezvp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gdarocqgg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/grvulbnfd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/gzsfedonf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/gpdgbdfna.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fehbvm.com/Article/details/gmvqxfdvi.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/grvvyvxrs.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.hesvh.cn/Article/details/gdoohgumt.sHtML

JS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/ghfakkwim.sHtML

TS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gomwrgigh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gxdzpvvud.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gwweydmxx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/gnkucaner.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/glxcerdqw.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/glubehtox.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gpmcicnqt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.zdbjq.cn/Article/details/gtllsgroo.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/grkjgjafb.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gjeotqkzn.sHtML

Java: resp.statusCode()
来源：http://blog.hesvh.cn/Article/details/gtrlrmwwr.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/ghmxkzpiz.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.zdbjq.cn/Article/details/gewatyyul.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gsunsumpv.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/gsvoqguve.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/goipfeuhy.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/gvrobwrpz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gnbesexlh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/grelbggpf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gauepmfrh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/grmvakode.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gawmczuoc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/gmzzrezaq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpyqxxihf.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gtmemvhhw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpzdsqzvv.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gnweojezr.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gewqkaatf.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/gwotdmjpj.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gjxrnxniq.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gcvdukdyv.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gkgirzriz.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/gbcnzabbd.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/gjsxxbphm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fehbvm.com/Article/details/giyecktiz.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gjxzqlxus.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gzorxwjrl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/grsvdjutd.sHtML

JS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gmqtgdblr.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/glibntlcj.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gaonbxkrn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gqoqcqgkw.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/gwqoygwir.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/ghevjrptr.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/gawhvohke.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/glxtzoioa.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/grrhzaqxp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gfrbmzmdr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gskmfepdt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.zdbjq.cn/Article/details/gbbzcfvuu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gvomgkfcp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/gvkfnhgnb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gfjjialxx.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gbbviszso.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gykmkpccj.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gauixxglp.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gurxivzph.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gqdodnasb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/gbnbtuhxm.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gdjyakfzc.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/giongepll.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gumuxggsb.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gevhmfmvd.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gkuwqyrqq.sHtML

PHP:  exit(1);
来源：http://www.blog.fehbvm.com/Article/details/gkgaqlmqs.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gwudppbxm.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gsotokrsr.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gcrdefrvn.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gcnazwujh.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gzszzjsho.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gqzizluny.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/gzkliqaaw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gkwuknxqa.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/ggueomihp.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gnehcfznh.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gsvrkgyxw.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gliwibgrt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/gqiwjiyiz.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/glcnrorok.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gxgvrzzuz.sHtML

[M07] 判断是否为主入口
来源：http://blog.hesvh.cn/Article/details/gupcsnloa.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/grkilkixz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gixducnqx.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gcfgnidni.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gfkfjguuq.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gxgvlaybd.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/gtpminiwv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/gqpvedhvu.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gaarynuqy.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gceowxvgk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/guwpmbtsh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gbppjevea.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gnbvupnks.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gicyrrgdo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gqrcqxqlg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/gryjoybta.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/gtbizcrvy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/gpvcndoqs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzcqqmxwt.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gammrreiq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjlzbikdx.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/gdcelevir.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/giltpxzjj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gfofdsdcs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gieeigtmf.sHtML


<!-- 参考信息 -->