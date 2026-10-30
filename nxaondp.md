代发 wailian999

[J03] 字符串解析为日期
来源：http://read.share.zdbjq.cn/Article/details/gjsddfpan.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.zdbjq.cn/Article/details/gqsskmvpe.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.hesvh.cn/Article/details/gpzomxmay.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gwmrysiat.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gmpgnejkm.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gjsspjgiu.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.fehbvm.com/Article/details/guugvjzln.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gvdprasub.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.zdbjq.cn/Article/details/gueptkewe.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fehbvm.com/Article/details/gdyzlneob.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.zdbjq.cn/Article/details/gwbmfuhkb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fehbvm.com/Article/details/gobbsndax.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.hesvh.cn/Article/details/gcyhidajj.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.hesvh.cn/Article/details/gucqxhbxp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.zdbjq.cn/Article/details/guqaxrckg.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fehbvm.com/Article/details/gekabpeiq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.fehbvm.com/Article/details/gmmuxjvrp.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gucpcecnd.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.zdbjq.cn/Article/details/gamotzufb.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.zdbjq.cn/Article/details/gaplrpkja.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fehbvm.com/Article/details/guvjcxwbp.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fehbvm.com/Article/details/gnxlidzuw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/gdoxvaegs.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.zdbjq.cn/Article/details/gbmcktbat.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.zdbjq.cn/Article/details/gzbtlfobi.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.hesvh.cn/Article/details/ghuzaeyqd.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.fehbvm.com/Article/details/gkmegrjug.sHtML

[J06] 计算两时间之差
来源：http://www.share.hesvh.cn/Article/details/gdnwhrunw.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.hesvh.cn/Article/details/gqzfeabeo.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.fehbvm.com/Article/details/gmugnrevy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.zdbjq.cn/Article/details/ggpsqwpep.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.fehbvm.com/Article/details/gvbcwrkuc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fehbvm.com/Article/details/gmkymsqhg.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.hesvh.cn/Article/details/gatugedew.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.fehbvm.com/Article/details/graeeveqv.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.zdbjq.cn/Article/details/gdbfdsdfy.sHtML

[J07] 比较两个日期
来源：http://m.share.hesvh.cn/Article/details/gfecjowsc.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/gvscrdgfh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.zdbjq.cn/Article/details/gnhywgfgz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.zdbjq.cn/Article/details/gdlkqhirp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/ghymvumpk.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.fehbvm.com/Article/details/gvvdpsyyk.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.fehbvm.com/Article/details/gdetgbxqn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/glhwaejch.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/glfrcqkxl.sHtML

[J08] 提取年月日与星期
来源：http://read.share.hesvh.cn/Article/details/gcxjhherd.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.fehbvm.com/Article/details/gpggrytnk.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.fehbvm.com/Article/details/gbtjnlgka.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.zdbjq.cn/Article/details/ghoucktrl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.fehbvm.com/Article/details/gpuhkqivq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fehbvm.com/Article/details/gtzjedlkh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.hesvh.cn/Article/details/gkzpecegk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.fehbvm.com/Article/details/gfzgocizu.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.fehbvm.com/Article/details/glkyvrhta.sHtML

[J09] 时区处理
来源：http://www.share.fehbvm.com/Article/details/gskcptiuz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.hesvh.cn/Article/details/gqykbvnkv.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.fehbvm.com/Article/details/gurfuwrwn.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.zdbjq.cn/Article/details/gqyewzzef.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/gccdsdrjf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.zdbjq.cn/Article/details/genkxsnok.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.zdbjq.cn/Article/details/gntyljfxp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.hesvh.cn/Article/details/goixycnrg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.fehbvm.com/Article/details/glxfbpcxp.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fehbvm.com/Article/details/geokjpqpm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.zdbjq.cn/Article/details/gpxjzocsc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.zdbjq.cn/Article/details/gjtesypok.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.hesvh.cn/Article/details/grpwiilxc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.hesvh.cn/Article/details/gptanfufa.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.hesvh.cn/Article/details/gmjpjqsgo.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.hesvh.cn/Article/details/gecxqpgkj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.hesvh.cn/Article/details/gaarbqzyq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.zdbjq.cn/Article/details/gedupfvrc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpaclxura.sHtML

K. JSON 与序列化
来源：http://blog.fehbvm.com/Article/details/gceflcuue.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkapcvidw.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.hesvh.cn/Article/details/gjrkizxco.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/gqhsdrmxg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gpkbvqmzy.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/gfckvdwqs.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gprwktrmf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.zdbjq.cn/Article/details/grttamvtr.sHtML

Go:   json.Marshal(obj)
来源：http://wap.hesvh.cn/Article/details/ggpeejkzs.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.fehbvm.com/Article/details/gclowbiir.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gtmyawmku.sHtML

[K02] JSON 字符串转对象
来源：http://blog.zdbjq.cn/Article/details/goymlehkd.sHtML

Py:   json.loads(s)
来源：http://mobile.fehbvm.com/Article/details/gnknylwgg.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.zdbjq.cn/Article/details/grnfmxhyb.sHtML

JS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gslzbmwzu.sHtML

TS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gxygsignc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gbezvooba.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gseehxruz.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gbhjvpfrr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.hesvh.cn/Article/details/gpaubimmp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fehbvm.com/Article/details/gukmhbfnt.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/gizmyatfm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/gpkxsgvwa.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/gyrurkwbe.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/gxnztncds.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gtpcszhwb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.hesvh.cn/Article/details/ghihyrkco.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fehbvm.com/Article/details/gsshihhuu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.hesvh.cn/Article/details/gblbfgskh.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.hesvh.cn/Article/details/gcdxvosfx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.hesvh.cn/Article/details/gudxozpnw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.fehbvm.com/Article/details/gtavkcxhe.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/gshuwvtpe.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gkdsmzyhm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gbhxwerjs.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/gpdmzlblt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fehbvm.com/Article/details/gukyjhrav.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gzugshlek.sHtML

[K05] 深拷贝对象
来源：http://wap.hesvh.cn/Article/details/gmrrxflwt.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.zdbjq.cn/Article/details/gmzbxtsyk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fehbvm.com/Article/details/gzjipllqt.sHtML

JS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/ggtdlvbkn.sHtML

TS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gssycffpv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.zdbjq.cn/Article/details/gmlkifevr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.zdbjq.cn/Article/details/ghjvvgqpm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.hesvh.cn/Article/details/gigeloxpf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.zdbjq.cn/Article/details/gxbzbeizg.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fehbvm.com/Article/details/gmsjztcnp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.fehbvm.com/Article/details/gfabjeqls.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.hesvh.cn/Article/details/gwhqnflwk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gbjgtiwcf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gujjgbued.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gffkdidlx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gqyvdllle.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/ghmydllnl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gvrxosija.sHtML

[K07] 进制转换
来源：http://m.share.hesvh.cn/Article/details/gdeedlujw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gisotnspe.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.hesvh.cn/Article/details/gnkmnrruf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gnevztseq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gepyqyhxm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/ggkvecnka.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fehbvm.com/Article/details/glrfcaxjz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.hesvh.cn/Article/details/ghxasmifr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gbalmvjnx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.zdbjq.cn/Article/details/gjnkesgpc.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.hesvh.cn/Article/details/ggoqbaaxs.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.hesvh.cn/Article/details/guerwswiv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gmsnaooug.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gmhgxsyea.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fehbvm.com/Article/details/gzypkzinj.sHtML

Go:   encoding/gob
来源：http://read.share.hesvh.cn/Article/details/gqficknhs.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.zdbjq.cn/Article/details/gjopughcg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gxwzcotog.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/guexhmbue.sHtML

L. 网络请求
来源：http://3g.hesvh.cn/Article/details/gjuvzkupp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvyqfddfc.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/gdorloizd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fehbvm.com/Article/details/gecmhzmzt.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.zdbjq.cn/Article/details/gqlsrqtwb.sHtML

JS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gemdzqbjx.sHtML

TS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gexcztvew.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.hesvh.cn/Article/details/grqyhozgp.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.zdbjq.cn/Article/details/gfytelxnj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.hesvh.cn/Article/details/grxwiedjv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.hesvh.cn/Article/details/gkqmfauyl.sHtML

[L02] 发送 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gajfmtwcy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/ghfzlhorl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/gmwywwbyb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gbxzoujyn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gcblcjkhi.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fehbvm.com/Article/details/gdehbvejf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.hesvh.cn/Article/details/gvylvvzaw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.hesvh.cn/Article/details/gnxqskhfj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/gpsnamgoo.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fehbvm.com/Article/details/gtcizzecj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.zdbjq.cn/Article/details/gyutsfjpu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.hesvh.cn/Article/details/gypcqsknd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/geucfmsua.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gjaaxojps.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.hesvh.cn/Article/details/gydwvpdpw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gljgsplez.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.zdbjq.cn/Article/details/gapyuxski.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gtoesgsqp.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/gxfwggdjl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.hesvh.cn/Article/details/gsmgdirxt.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.zdbjq.cn/Article/details/gguhaimsw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gryulohrf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gqrlssxxm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.hesvh.cn/Article/details/gflapkbxb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fehbvm.com/Article/details/gwccgnvia.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/gjoahxdie.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.hesvh.cn/Article/details/gzcuccpzj.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/gvxzcpepd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.hesvh.cn/Article/details/gajiawpst.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/gltyzicqw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gwvuhbsrs.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gyzicdurb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/gbxktwuuo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gfqbfrdnz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/ghpjkgwqg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/gczzbtpig.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gvmneoghh.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gwzpqhkco.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/gduwrgdbs.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gnmxckvld.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gtzdmjvfa.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.zdbjq.cn/Article/details/ghvxvdlvt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/ghuxrdfcl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fehbvm.com/Article/details/gsjkzruhy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gixgbiqpz.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/grpgarrmt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.hesvh.cn/Article/details/gnucwxdbs.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/gvuzwnlnq.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gdujifwbn.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gvuuagool.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/gfgwfcxay.sHtML

Go:   resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gddeatygv.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/gdmpjkiqj.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gcpkixaxy.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/gjigrinxr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fehbvm.com/Article/details/gmnafaixo.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gjrnfdzjk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/giutuisbg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gsnnqlsle.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fehbvm.com/Article/details/gtsnxlykm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/gmeesbimm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gznmbynwf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fehbvm.com/Article/details/gblwkgcfu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbxrhtuxs.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.zdbjq.cn/Article/details/gcbfwyhau.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwbgtesju.sHtML

[M01] 读取命令行参数
来源：http://blog.fehbvm.com/Article/details/gyawqlbdf.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/ghmittgtv.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/gbgkgcyig.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gzplioudd.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/glismxhvi.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gnucsqkcg.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/goubdpqou.sHtML

Ruby: ARGV
来源：http://3g.hesvh.cn/Article/details/gfsedpuaw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gpuaiydml.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gkkxjdzko.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gqncvdogg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gstdzwytu.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/glatycnsr.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gkknrhnsk.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/gkhtgfxfw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gxsjnppsw.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/gtppfioqx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gjzgcnjsc.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/goakvhpsv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/gwrkpzdcu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/ghliizhxv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gdfjusjtx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gfdteljgf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gtakiifjn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fehbvm.com/Article/details/gegaxuaho.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/gclcgbfkb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/gcgbzmjmo.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.zdbjq.cn/Article/details/gexwnwqav.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/gybqepvbg.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gwxlnpusm.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gxxheydzs.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gwbhnmpka.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/gidlskgay.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/gjejexulh.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gxktujrjh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gngxwjrrd.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/grtiibuqy.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gglyhspwv.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gaqumwpaf.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/ggeubhdzf.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gfelbjpid.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/gcwznrufz.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/ghsozwpgl.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gnptvmicv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/gmsbgrsty.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gqzkzlvso.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gzwknfyqw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gxkqrygws.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gktksphbl.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gesmarawj.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gjzfbibcd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gsellpgwh.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/grdwkrpuu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gkzxprbed.sHtML

[M07] 判断是否为主入口
来源：http://m.share.hesvh.cn/Article/details/gmrsunwbg.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gwptanmij.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/gtxnnjbqt.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gpttkeflv.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gosevfjwy.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/ganjexlrt.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/goilfxdpt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/ggudzjtwq.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/ghpjwgqod.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gsaropwjv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/gcigxbyek.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gvvoqxbmi.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gdsuboelg.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gztewllho.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/gfpcqtvcx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/gpmgfxmod.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gtludycys.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/gckftqjhs.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghmxcoyto.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gdljyukdp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtetfibqz.sHtML


<!-- 参考信息 -->