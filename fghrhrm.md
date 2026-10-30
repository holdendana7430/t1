代发 wailian999

[J03] 字符串解析为日期
来源：http://blog.fehbvm.com/Article/details/gcllsjuwu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.hesvh.cn/Article/details/gxswozprj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.hesvh.cn/Article/details/gxyhgiwrk.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gkozxtogv.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/ggppyxroc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gqncvaszy.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gkiiuuheq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/glgqubkja.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.hesvh.cn/Article/details/ggalkebzj.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fehbvm.com/Article/details/gxokimokt.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.hesvh.cn/Article/details/geynjthmc.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.zdbjq.cn/Article/details/gtmlrxsao.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.zdbjq.cn/Article/details/gcrolpqxe.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/goqkqorgd.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.zdbjq.cn/Article/details/gklendwgb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.fehbvm.com/Article/details/gaqtqnqgb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.hesvh.cn/Article/details/gvrvqdfcp.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.hesvh.cn/Article/details/gtjzfniwf.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.fehbvm.com/Article/details/gbjcijdbb.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.hesvh.cn/Article/details/gtslqetfg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.fehbvm.com/Article/details/gybaglgte.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.hesvh.cn/Article/details/gbxhrkdin.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.zdbjq.cn/Article/details/glldyymxj.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.hesvh.cn/Article/details/gghnrjkxj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.hesvh.cn/Article/details/gicfiwfrz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.hesvh.cn/Article/details/gkbzbjxzs.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.fehbvm.com/Article/details/gtmsgxjui.sHtML

[J06] 计算两时间之差
来源：http://www.blog.zdbjq.cn/Article/details/gexesgcag.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.hesvh.cn/Article/details/ghcooezcr.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.hesvh.cn/Article/details/geblgpksl.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.hesvh.cn/Article/details/gmpajusec.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.zdbjq.cn/Article/details/gychwfqor.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.fehbvm.com/Article/details/gqbmepmzs.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.hesvh.cn/Article/details/gjbuutrxj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.hesvh.cn/Article/details/gjwuavtnj.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.zdbjq.cn/Article/details/gvqbyrmny.sHtML

[J07] 比较两个日期
来源：http://mobile.fehbvm.com/Article/details/gftcnbbvq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gwihgfslb.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.zdbjq.cn/Article/details/gcbetmzms.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.zdbjq.cn/Article/details/ghifloleb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.hesvh.cn/Article/details/gncwfqiju.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.hesvh.cn/Article/details/gkespuixd.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.hesvh.cn/Article/details/ggafobuhm.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/gwtebfqvk.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/gghhprjpz.sHtML

[J08] 提取年月日与星期
来源：http://read.share.zdbjq.cn/Article/details/gfqbiqwdu.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.hesvh.cn/Article/details/gbmolkpbx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.zdbjq.cn/Article/details/gkbizkuya.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.zdbjq.cn/Article/details/gdipzczdf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.zdbjq.cn/Article/details/gxxhqswmj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.fehbvm.com/Article/details/glzrzulcv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.fehbvm.com/Article/details/glumyorde.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.zdbjq.cn/Article/details/ggxnhlojw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.hesvh.cn/Article/details/gvnbibtae.sHtML

[J09] 时区处理
来源：http://m.share.fehbvm.com/Article/details/gvcyzwmig.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.hesvh.cn/Article/details/gjqgkhwze.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.zdbjq.cn/Article/details/gdnutnnbz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/gxzmuclyo.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/gaptpxjfr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.fehbvm.com/Article/details/gazcsmqac.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.fehbvm.com/Article/details/ghbfaeaek.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.hesvh.cn/Article/details/gnlvalvzo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.zdbjq.cn/Article/details/gimxyhble.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fehbvm.com/Article/details/gscfpzogh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.fehbvm.com/Article/details/grtjzndek.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.hesvh.cn/Article/details/glngfiyic.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.hesvh.cn/Article/details/gyephxske.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.hesvh.cn/Article/details/gbybfmurj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fehbvm.com/Article/details/grzipbhfi.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.hesvh.cn/Article/details/grmwpukcp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.zdbjq.cn/Article/details/gpskbjeol.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.hesvh.cn/Article/details/gpugpcqbe.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxzezdmsa.sHtML

K. JSON 与序列化
来源：http://www.blog.fehbvm.com/Article/details/glvgvjdwf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqktvbhrc.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.zdbjq.cn/Article/details/gvwkudjbn.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/gcrverrro.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.zdbjq.cn/Article/details/gxnmedbwe.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.zdbjq.cn/Article/details/gdgylibys.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.zdbjq.cn/Article/details/guufsuiau.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.zdbjq.cn/Article/details/ggowbntzf.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.hesvh.cn/Article/details/gyiyymfac.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fehbvm.com/Article/details/gugmstajz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.fehbvm.com/Article/details/gjaupjlbs.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.fehbvm.com/Article/details/gqyrkriqj.sHtML

Py:   json.loads(s)
来源：http://3g.fehbvm.com/Article/details/gqmyuqqtz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.hesvh.cn/Article/details/gynfxduuc.sHtML

JS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gwmzjtqst.sHtML

TS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gnkaijkga.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.zdbjq.cn/Article/details/gdkrqtizj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/gqxqofcyq.sHtML

Ruby: JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gsnqdlcyq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.zdbjq.cn/Article/details/gbszjgwoc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.hesvh.cn/Article/details/ggasugowp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.hesvh.cn/Article/details/gyzfekyag.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/gsssraznc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/gmxegxute.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gxseeevfp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.hesvh.cn/Article/details/gllrjvhyl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fehbvm.com/Article/details/gjhiztloi.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.hesvh.cn/Article/details/gxdepxerd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.hesvh.cn/Article/details/girsbnoqx.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.hesvh.cn/Article/details/gzckyypbc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.hesvh.cn/Article/details/gkrososan.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fehbvm.com/Article/details/gugwkoayv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/ghgbjwkfw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gamfqeosf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.hesvh.cn/Article/details/gjfxlchfa.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gajzflzug.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gfjndxogc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/glslbvjzy.sHtML

[K05] 深拷贝对象
来源：http://mobile.zdbjq.cn/Article/details/gtvttqycr.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.fehbvm.com/Article/details/gzpnvnfzt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.fehbvm.com/Article/details/gcqeewlsz.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gjtggqsyv.sHtML

TS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gswsxpsyz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fehbvm.com/Article/details/gwrdswees.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fehbvm.com/Article/details/gdnuevvln.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.hesvh.cn/Article/details/gqtmgammw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.hesvh.cn/Article/details/gqqgbnrzo.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.hesvh.cn/Article/details/gvqzjtpbo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gqgmdxubp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.zdbjq.cn/Article/details/gfdidkkoo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gvcwyiima.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gzzyedkla.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.hesvh.cn/Article/details/gmyqvehsk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gdjwspqed.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gpwbsyczw.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gvegxyuyi.sHtML

[K07] 进制转换
来源：http://3g.fehbvm.com/Article/details/grsacsccn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gyoryeibx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.hesvh.cn/Article/details/ggnguyagk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gmurmhoqi.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gkasunnka.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gdhxqokdr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fehbvm.com/Article/details/gbzcdcjvj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.zdbjq.cn/Article/details/gksigwwvu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gwzmqcrsr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.hesvh.cn/Article/details/gyqacxreu.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/gympnbhir.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.zdbjq.cn/Article/details/gpouikefb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gacckcefr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gpwgtcvdl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.zdbjq.cn/Article/details/gkpjbfktq.sHtML

Go:   encoding/gob
来源：http://www.share.fehbvm.com/Article/details/ghhezngxs.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.zdbjq.cn/Article/details/gkvexcurs.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gozvqawil.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpxbcfsfm.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/gzizgwifl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gepksokhz.sHtML

[L01] 发送 GET 请求
来源：http://wap.fehbvm.com/Article/details/gjbahqyhp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fehbvm.com/Article/details/grtkinrpp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fehbvm.com/Article/details/gpidvdkid.sHtML

JS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gwmuhzqzu.sHtML

TS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gwjbjyqtv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/guksgebnu.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fehbvm.com/Article/details/gzlehlvwv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/gxryyputx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/gsreiwhmt.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/getujlnvm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gicyzhymr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fehbvm.com/Article/details/gqkzraidn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gmdpxvbgj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gozexychd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/gcmgmfpiu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/gpiadgumw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.hesvh.cn/Article/details/gtmrjupsg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fehbvm.com/Article/details/gomltvnek.sHtML

[L03] 设置自定义请求头
来源：http://mobile.hesvh.cn/Article/details/gzqsemsts.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fehbvm.com/Article/details/gpounubro.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.hesvh.cn/Article/details/gfdmxnltq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gxhhgwjyj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gjukdjxlw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.hesvh.cn/Article/details/glawpnayh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gxjgvntwf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/ghqhhityc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gpqxwrqiy.sHtML

[L04] 设置超时
来源：http://blog.fehbvm.com/Article/details/greiidzwj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.hesvh.cn/Article/details/gvjixefir.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/golttxiga.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gpjdtlrww.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gixluvsrv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fehbvm.com/Article/details/gqzstxosb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/gdlwoeehd.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fehbvm.com/Article/details/gacgzfgwa.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/grgcainib.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/grenxbpwz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/gpufzwdaf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.hesvh.cn/Article/details/gsswwrnfz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gyodckzux.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gljhdxqxc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.zdbjq.cn/Article/details/gkznoytaz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gulepfphn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.zdbjq.cn/Article/details/gvbtnwklj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/grmctsdud.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.zdbjq.cn/Article/details/gqajrwver.sHtML

Py:   resp.json()
来源：http://wap.fehbvm.com/Article/details/gigwbcpog.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/gevprhngo.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gsjnulokd.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gtgiatoox.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gopkhrpiv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.hesvh.cn/Article/details/ggwrkktzj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/gngpdfexe.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fehbvm.com/Article/details/gicvcxocx.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gozymvkgk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gimdyvqam.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/gllawmgqd.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gcrbrtoiy.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gpsjckbbv.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/gahfjbgsu.sHtML

Go:   resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/giadrxbrq.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.hesvh.cn/Article/details/gmvllfnsf.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gwpzwztfv.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/gvhkjmnjh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fehbvm.com/Article/details/gsoekqgfm.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/gofcdwump.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/guzokgutq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/ggnvatskr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/gytajzdkl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/glbpbvxne.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/gcriwtyvd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/glreppzvm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gannddtzl.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/gzpdpozdj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpmniaqta.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/gelkujfqs.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/gpogvtlao.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/gmrijkhmq.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/grbbovhas.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gylknfzxu.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gnztwjoqj.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gfklcktlw.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/gxfcfnhly.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/grvkmmwgs.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gqljfstdp.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gruwlthnx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/glkpppdms.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gzajietbs.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gqrycpsag.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gbidszpog.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gttxvclsz.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gboukwuyk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/gtqatdgfp.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gofxsbjuf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/grizlbwnu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/ghwjuftux.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gsasgjnro.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/grmzplueq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/givxfwrrw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gvmqepihq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/giwtfsvpd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gvjiungka.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/gfzsagjir.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/gvjikboek.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gyytckrjj.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gnxdifhdb.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gigxlwudf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/gkywexetn.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gnabqodkx.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gpecjnndu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gslkumlag.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/ggftquobi.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gefmwxmym.sHtML

PHP:  exit(1);
来源：http://www.share.zdbjq.cn/Article/details/gzchlubsx.sHtML

JS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gjenwnxqk.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gpreaalih.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gwvabdozc.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gwojgvbjb.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/giwizbedg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gtfrdptgf.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/ggevgsuls.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gwtiqigvx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/gzzfshyxc.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gppclxovl.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/grnrbigcx.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/gwctcusnm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/gustfyfrg.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gtgbcrmse.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gmdevvoxk.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/glttcevmf.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/gcfkowzmg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/ghxhhadhp.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gwflhzdjc.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gsqiwvpuk.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/gtpmmirhs.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gnzsnruzo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gkziowkbr.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gclwrfwdm.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/goegnzmsy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/gajrwvcda.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/ghwmjclmc.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gpctxvdtg.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gdhzcakwa.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gejdihcjy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gevpktdnc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/gjgdkrlbi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/gurfzuwru.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gguxyzzmu.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gwpifnblo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqrvgvsqd.sHtML


<!-- 参考信息 -->