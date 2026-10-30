代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fehbvm.com/Article/details/gxvzjmyjx.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fehbvm.com/Article/details/gqoyzpulg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.fehbvm.com/Article/details/gkggvlyie.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.hesvh.cn/Article/details/gpcpyxaha.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.fehbvm.com/Article/details/gbveeytvv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fehbvm.com/Article/details/gznbaxuza.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.hesvh.cn/Article/details/goeaaxggn.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/ghynjwqui.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.fehbvm.com/Article/details/grhemnmff.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.hesvh.cn/Article/details/gwkxbhpnx.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fehbvm.com/Article/details/gfljopbcf.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.fehbvm.com/Article/details/geiuzdapw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fehbvm.com/Article/details/gqykwqltv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.zdbjq.cn/Article/details/gkrxzktjb.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/gqijduiux.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.fehbvm.com/Article/details/guvrwrcml.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.fehbvm.com/Article/details/gcpvsvuya.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.hesvh.cn/Article/details/gxothgtah.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.fehbvm.com/Article/details/gagqvgcte.sHtML

[J06] 计算两时间之差
来源：http://wap.hesvh.cn/Article/details/gekivpckc.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.hesvh.cn/Article/details/gwcxycqrq.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.zdbjq.cn/Article/details/gtnsqjaah.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.fehbvm.com/Article/details/gguxywbbx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.zdbjq.cn/Article/details/ganqzqacs.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fehbvm.com/Article/details/gicepcjzu.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.hesvh.cn/Article/details/gubjmvibh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.hesvh.cn/Article/details/gzhtjtdbk.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.zdbjq.cn/Article/details/giihstspn.sHtML

[J07] 比较两个日期
来源：http://wap.hesvh.cn/Article/details/gdpvoxwjz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/goapfwagl.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.fehbvm.com/Article/details/ghbizhmoq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.fehbvm.com/Article/details/gymfpsmek.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/gbmzogiuc.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.zdbjq.cn/Article/details/gyehackkt.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.hesvh.cn/Article/details/gbiibbxrd.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gzaugldrr.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/ganzbjmcb.sHtML

[J08] 提取年月日与星期
来源：http://blog.zdbjq.cn/Article/details/gpdfiscji.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fehbvm.com/Article/details/gludjgvnh.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.zdbjq.cn/Article/details/gutvnarzt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.fehbvm.com/Article/details/gvuvuthqp.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.fehbvm.com/Article/details/gxotxzkbj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.zdbjq.cn/Article/details/grvycxjmv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.fehbvm.com/Article/details/ghuwndywb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.fehbvm.com/Article/details/gimabarjk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.fehbvm.com/Article/details/gjxbifotq.sHtML

[J09] 时区处理
来源：http://www.m.share.zdbjq.cn/Article/details/gdvezehre.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.zdbjq.cn/Article/details/gjelmljfq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.zdbjq.cn/Article/details/glnzfepvo.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fehbvm.com/Article/details/gdycpgkxq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fehbvm.com/Article/details/gvrhmaobz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.hesvh.cn/Article/details/gsgixhkbf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fehbvm.com/Article/details/gfakftahr.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.hesvh.cn/Article/details/giemnymji.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.fehbvm.com/Article/details/gluwbkddy.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.hesvh.cn/Article/details/gsexpepro.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.fehbvm.com/Article/details/gvuquyadl.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fehbvm.com/Article/details/gxzgnfeye.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.fehbvm.com/Article/details/gowzuxbtc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.hesvh.cn/Article/details/getesqmsd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.zdbjq.cn/Article/details/garmifhzw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.hesvh.cn/Article/details/gayivsjxg.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.hesvh.cn/Article/details/ghvwwsmzk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.hesvh.cn/Article/details/gokocxitn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsxksmabf.sHtML

K. JSON 与序列化
来源：http://baike.fehbvm.com/Article/details/gjqzexbhv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gipflqhhz.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.hesvh.cn/Article/details/grkcjkqgx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/gcbnjzkma.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gdescbfhn.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gydbgrovl.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/gktvyzuka.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.hesvh.cn/Article/details/glffkoyqg.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.zdbjq.cn/Article/details/gwdwobazt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.hesvh.cn/Article/details/grxxmtviz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.zdbjq.cn/Article/details/gkryfffab.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.hesvh.cn/Article/details/gvygbnqjr.sHtML

Py:   json.loads(s)
来源：http://blog.fehbvm.com/Article/details/ghogxdnkw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fehbvm.com/Article/details/ggpzttspb.sHtML

JS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gjtruyyqe.sHtML

TS:   JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gbpamswta.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.fehbvm.com/Article/details/geruhzicr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gdhvijhlx.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gtidcccvn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.hesvh.cn/Article/details/gsxzhpcdf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fehbvm.com/Article/details/gvlpeebaq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/gqtscrfpm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.zdbjq.cn/Article/details/gkpdceqll.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gqcrvrxul.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gzsyskazk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gxfkuwszu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.zdbjq.cn/Article/details/ghwwkcxzv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.zdbjq.cn/Article/details/gzjuvuvnq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.fehbvm.com/Article/details/gdzqhnchk.sHtML

[K04] 读取 JSON 文件
来源：http://blog.hesvh.cn/Article/details/glgwaphbe.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gsvkxekdi.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.zdbjq.cn/Article/details/gwusdjfkl.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gguelbkkb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gztlfbxcg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gwermlccz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gnhjtpjpc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gydbpjnpy.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gijafshsg.sHtML

[K05] 深拷贝对象
来源：http://mobile.hesvh.cn/Article/details/gtqlstjvd.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.hesvh.cn/Article/details/gewsycgpg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fehbvm.com/Article/details/gmfekwdbq.sHtML

JS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gwqbvapmz.sHtML

TS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gdwoxqtyz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.hesvh.cn/Article/details/gpkxevkgs.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.hesvh.cn/Article/details/gudpldnqp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.zdbjq.cn/Article/details/gvcxqtkdp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.zdbjq.cn/Article/details/gaxodttpb.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.hesvh.cn/Article/details/ggmyvjmad.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.hesvh.cn/Article/details/gwkcrgfhm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.hesvh.cn/Article/details/gvzhofvfb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gqooktryt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gpuvbjbeb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.hesvh.cn/Article/details/gwjxssyqz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gmcagpqyg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gpqmhwnon.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gbkudttyg.sHtML

[K07] 进制转换
来源：http://read.share.hesvh.cn/Article/details/ggbxanfjo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gbdentozz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fehbvm.com/Article/details/gnnebdfyb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gxblxotgg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gjgnweebv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/grjsjorwk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fehbvm.com/Article/details/gomttxwuz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.hesvh.cn/Article/details/grqrfwixv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gpgyccpbl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/gmxmjsfbj.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.hesvh.cn/Article/details/gjqbufgsq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.hesvh.cn/Article/details/gcqteayav.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gekvnlkct.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gvtcdjvtw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.zdbjq.cn/Article/details/gymnxmody.sHtML

Go:   encoding/gob
来源：http://wap.hesvh.cn/Article/details/gknokrdnt.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gegyfuqxi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/ghupbsylq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggozzmkdf.sHtML

L. 网络请求
来源：http://read.share.zdbjq.cn/Article/details/gqjepzbcb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsoyfyqkd.sHtML

[L01] 发送 GET 请求
来源：http://wap.hesvh.cn/Article/details/gkoqebofi.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fehbvm.com/Article/details/gpjqdvwpc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.zdbjq.cn/Article/details/getzmlwbo.sHtML

JS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gauwvmyup.sHtML

TS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gvykdmymy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fehbvm.com/Article/details/gggrieswm.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/goxkwzczw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fehbvm.com/Article/details/gufpjzskw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.hesvh.cn/Article/details/gbuyddycw.sHtML

[L02] 发送 POST JSON
来源：http://wap.fehbvm.com/Article/details/glkojikir.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gaixlrali.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/gfbdxpclg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gqjeqqcgz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gdiadfdwk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fehbvm.com/Article/details/ggaguuwha.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/gzumipfbs.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fehbvm.com/Article/details/gptdyacra.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/giahbjuwy.sHtML

[L03] 设置自定义请求头
来源：http://3g.zdbjq.cn/Article/details/gfudyavts.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.zdbjq.cn/Article/details/gjuwjilau.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fehbvm.com/Article/details/gmvkdvwev.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gatmrqwpz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/ggxmydggf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.zdbjq.cn/Article/details/ggqvokski.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gbkilkeor.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.hesvh.cn/Article/details/gumbqlinh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gdqvdhenz.sHtML

[L04] 设置超时
来源：http://www.m.share.zdbjq.cn/Article/details/givvredll.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fehbvm.com/Article/details/gomhvgzrz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.zdbjq.cn/Article/details/glgxieodd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gqldeelew.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gftuymqdf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/gcvtxrebp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.zdbjq.cn/Article/details/gktfpfeap.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.zdbjq.cn/Article/details/grgtyqzpr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.hesvh.cn/Article/details/gypcylmim.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.zdbjq.cn/Article/details/gdtnqflwp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fehbvm.com/Article/details/ghzkmkbfv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.hesvh.cn/Article/details/gbsglivpp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gnswghfau.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gdbodqxgs.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/gtgzwpbis.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gkhpdwfpg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/gsjoilakc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/gigastabx.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/giatyofhz.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gixrnoomt.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/gpktbbjbc.sHtML

JS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/ghjnpbkga.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gxlvnxtjb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/ghoindhfi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/gvyrbxeam.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.zdbjq.cn/Article/details/grpdscszw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/gulcknftg.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gplnintyr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/gmusywjyc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.zdbjq.cn/Article/details/gqouqziyo.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gnbowykjf.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gfpgxsmgb.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/gahoormmr.sHtML

Go:   resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gtcmvnvxr.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/gufbdxnej.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/ggreczlmb.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gbrhbdxma.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/gstyseqrk.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/gplrcxdge.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gyacbboic.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gkyfsjlvb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/gwohrvlml.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gbeqyjkot.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/ggofrjmxb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gcqjttefo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxvlavaez.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/gtsvvmwis.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcgauuaxw.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gvtxwipxz.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gxzzwgzxq.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/gbiyrmcuw.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gzxunbbbq.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gpdcnbvgr.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gfvbfriqm.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/gczcmmaip.sHtML

Ruby: ARGV
来源：http://3g.hesvh.cn/Article/details/gqnjmsirt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gfhgzxajd.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gosxopgkp.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gsfktdbvz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gfaxwwmdi.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/giaadzppl.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/ghlodmszj.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/gbwexngqa.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gmzxecqqd.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gggepssri.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gqmflvoyr.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gcfbzdbzm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gawugyybh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/gciluqroi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gwydfkipl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gtjllgovi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gtcacqfwd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gpklpywdv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gfllmgbxw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gpyvunzof.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/gizwehhog.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/gqynumhag.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/gxcjknnuj.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gxepndemz.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gajxzlxnb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/gxoqshccu.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gtonqomub.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/ghdjuespa.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gfavninry.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/grpdivdua.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/gydmubqed.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/ghnbbrctu.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gtdgnmxqz.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gdvvdacgu.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gyjhtafhc.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gkoleillc.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gwwhdmibi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gmvxgytnk.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gxodvtmfb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gaszlqihy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/glaulkmpl.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gwiezbbch.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gtblhugmx.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/gkfxyvryx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/giwsbkiaj.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gwfslpgcl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gtoeigefo.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gvcautadn.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gthonmklo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gpbcikpcq.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gvheyqiis.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gppzkenew.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gcuubqpju.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/grplfqtod.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gvgrvjnev.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gvzvypquj.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gefyezuyx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gkvocibeh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gvrcviuyc.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/ghpnkqivl.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gwddgrqef.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/gcukettzd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gtpvmhmij.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gfgcprbmv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/ghdsoxztn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvcgvkvjj.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gmabwsety.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfgvyqocf.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/gxduraook.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gimgqjxyq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gjtnmgqvl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gmepycjos.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gxfipwzow.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gprhmwjsl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/goacdtbli.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/ghndwntoq.sHtML


<!-- 参考信息 -->