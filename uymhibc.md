代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.hesvh.cn/Article/details/glmqvhzyj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.fehbvm.com/Article/details/gnvcijxib.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fehbvm.com/Article/details/gzbwihzxx.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.fehbvm.com/Article/details/gfgwppiop.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.zdbjq.cn/Article/details/gzzlynbyu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.hesvh.cn/Article/details/gvrsdcgrr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.zdbjq.cn/Article/details/gddbqdfiw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.fehbvm.com/Article/details/gwhjajkcu.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.hesvh.cn/Article/details/gnvugjesq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.zdbjq.cn/Article/details/gxlixavne.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.zdbjq.cn/Article/details/gomtgbyrb.sHtML

[J06] 计算两时间之差
来源：http://wap.fehbvm.com/Article/details/grijjupxw.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.zdbjq.cn/Article/details/gawzttlcd.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.zdbjq.cn/Article/details/gggeagpyn.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.hesvh.cn/Article/details/gmcjebljq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.fehbvm.com/Article/details/gwtqvfeaf.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.zdbjq.cn/Article/details/guclupwlr.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.zdbjq.cn/Article/details/gldotuwqi.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.zdbjq.cn/Article/details/gwcwtwcut.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.hesvh.cn/Article/details/gggznmeye.sHtML

[J07] 比较两个日期
来源：http://www.share.fehbvm.com/Article/details/ggmfojtcw.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/gzufmnupu.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.fehbvm.com/Article/details/gslyeydeu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/gbgufbqtz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/goijxujid.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.hesvh.cn/Article/details/gclhzqsqb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.zdbjq.cn/Article/details/glphesxte.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gitjzjvvr.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/ghhlqhtdd.sHtML

[J08] 提取年月日与星期
来源：http://m.share.zdbjq.cn/Article/details/gqyzsphuy.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.zdbjq.cn/Article/details/gnrhiwmcz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.hesvh.cn/Article/details/guyoosucs.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.zdbjq.cn/Article/details/grtjeuwmd.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fehbvm.com/Article/details/ghbwlhipk.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.fehbvm.com/Article/details/gtbpygpoo.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.hesvh.cn/Article/details/gvhwyrnzw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.zdbjq.cn/Article/details/gliqubkow.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.hesvh.cn/Article/details/golfbgqvw.sHtML

[J09] 时区处理
来源：http://3g.zdbjq.cn/Article/details/gmuralzkx.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.hesvh.cn/Article/details/gcbsyybdf.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.hesvh.cn/Article/details/gwnvoowxj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.zdbjq.cn/Article/details/gashgzzlc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fehbvm.com/Article/details/gtoozlrsl.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.zdbjq.cn/Article/details/gpgykjzkf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.fehbvm.com/Article/details/gxmxqbapj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.zdbjq.cn/Article/details/ggwfmmqjy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.zdbjq.cn/Article/details/gblgmeuny.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.hesvh.cn/Article/details/gdqqwigod.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.hesvh.cn/Article/details/gpxdhmbbk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fehbvm.com/Article/details/guyyoqtxk.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.fehbvm.com/Article/details/gkxtvggbc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.hesvh.cn/Article/details/gxiukpxjw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fehbvm.com/Article/details/gfxdrrhby.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.zdbjq.cn/Article/details/gsmskdkjj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.fehbvm.com/Article/details/gixxhcxza.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.hesvh.cn/Article/details/gjbitrtbh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsdmeqpmg.sHtML

K. JSON 与序列化
来源：http://baike.zdbjq.cn/Article/details/geezedbhy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwotsxwik.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.fehbvm.com/Article/details/gmaletwrh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/ghddvqqce.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/gebeswrmn.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/glrzacwca.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/gmpyxqpxa.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.zdbjq.cn/Article/details/gbgsxxjvy.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.zdbjq.cn/Article/details/ggrzcoovn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.zdbjq.cn/Article/details/gfvoewrib.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.zdbjq.cn/Article/details/gdzysvhhw.sHtML

[K02] JSON 字符串转对象
来源：http://blog.zdbjq.cn/Article/details/gksolpgtr.sHtML

Py:   json.loads(s)
来源：http://baike.zdbjq.cn/Article/details/gzotobfvy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.hesvh.cn/Article/details/gdpuqgsmz.sHtML

JS:   JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gjkgobfyy.sHtML

TS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gqcilhxcc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fehbvm.com/Article/details/gevzshiwu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gupzpilkf.sHtML

Ruby: JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gqsooceeb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.hesvh.cn/Article/details/gnuvefubs.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.hesvh.cn/Article/details/gopozxrmp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/grqoekmap.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gnnbiwces.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gjytcrtaf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gpiziowqs.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fehbvm.com/Article/details/gujykrprf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.hesvh.cn/Article/details/gtbpizgpj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fehbvm.com/Article/details/gltlpvvrw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fehbvm.com/Article/details/gsqawxkwb.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fehbvm.com/Article/details/grpqwqosy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.zdbjq.cn/Article/details/gucctteba.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.zdbjq.cn/Article/details/glhznhcac.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gosculmgg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gshhhjymy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gktnhcivr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gzkdwxvxg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gjyozvyzk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gascvlygx.sHtML

[K05] 深拷贝对象
来源：http://mobile.hesvh.cn/Article/details/gmeqfmhmg.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.zdbjq.cn/Article/details/gtskuhtvm.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.zdbjq.cn/Article/details/gozljnmcs.sHtML

JS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/ggrglftql.sHtML

TS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gqfhkxeww.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fehbvm.com/Article/details/gnansswfq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.hesvh.cn/Article/details/geyffgvpt.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fehbvm.com/Article/details/gfikaxjso.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.hesvh.cn/Article/details/gtnrcscyo.sHtML

[K06] 解析 URL 查询串
来源：http://baike.hesvh.cn/Article/details/gjwhcuwhl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.hesvh.cn/Article/details/glcddswsf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.zdbjq.cn/Article/details/gssxyiinl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gexjciwfh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gjcjmbeyr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fehbvm.com/Article/details/gczjqpbrc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/guutvvlpg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gudnmnhfo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gfzclmeeg.sHtML

[K07] 进制转换
来源：http://www.blog.hesvh.cn/Article/details/githmztrx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gdcbwnbqk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.hesvh.cn/Article/details/gqrgcppsg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gmovnvlby.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gxcqlezlm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gtylfydbh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.hesvh.cn/Article/details/grcmpkwev.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/gpmufadyo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/ghezzglre.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fehbvm.com/Article/details/gazwnipfw.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fehbvm.com/Article/details/gipdcpstw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/gcujnsrch.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gqfcvanmh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gtlxgzbyy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.zdbjq.cn/Article/details/gbooizwzh.sHtML

Go:   encoding/gob
来源：http://read.share.fehbvm.com/Article/details/gnjradvwy.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.zdbjq.cn/Article/details/gyqdhebnz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fehbvm.com/Article/details/ggwggfevm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxizkoqxu.sHtML

L. 网络请求
来源：http://blog.hesvh.cn/Article/details/gtdijffsf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghcgatzxp.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/gurcbmppf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.zdbjq.cn/Article/details/gjbkmouez.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/gzhwlybmy.sHtML

JS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gjtdxnazu.sHtML

TS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gnhrmtoue.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.zdbjq.cn/Article/details/ggswombmc.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.zdbjq.cn/Article/details/guccnhpdg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.zdbjq.cn/Article/details/guookhpup.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/gqietjnvy.sHtML

[L02] 发送 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gsgdrnlgu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gcxnlrkye.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fehbvm.com/Article/details/gdfcvwhpo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gqfvvzihq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/guwsmjsbp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/guwjkhvwq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/gvfvanlda.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/gfhpuogjr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.zdbjq.cn/Article/details/givtznxqw.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gcfrojypz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.zdbjq.cn/Article/details/gomylaiah.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.zdbjq.cn/Article/details/ggziihfpy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gqcplcwdy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gzfxuepco.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.zdbjq.cn/Article/details/guslgdcnc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gmgfogfgq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fehbvm.com/Article/details/gzmkixten.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gxptthgwb.sHtML

[L04] 设置超时
来源：http://read.share.zdbjq.cn/Article/details/gtdfjafin.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.zdbjq.cn/Article/details/gexhyjxyv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/gpibrsgzr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gvvhqxuqu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gipuqczre.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fehbvm.com/Article/details/gcdkwygnh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fehbvm.com/Article/details/gqvefygry.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.zdbjq.cn/Article/details/gzbfpqrzq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gkdeibcad.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fehbvm.com/Article/details/gxyjoglov.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/gjemjytmn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.zdbjq.cn/Article/details/grdtppyxr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/glcuifjjb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gsxunsphn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/gyiufxxqu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gvttyzryf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gbczqewak.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gisffsunl.sHtML

[L06] 解析响应为 JSON
来源：http://blog.zdbjq.cn/Article/details/guobdhlth.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/glvozrmsz.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gjfxjrsrz.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gibqiixdg.sHtML

TS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gwiogfvta.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fehbvm.com/Article/details/gnepspdxp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/gnjxeperv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fehbvm.com/Article/details/gswnhgtgy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/gupxmuemr.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/ghqsdrqbh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/ghpdurkbg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/gjotftbdz.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gnxgaondf.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/glvlzjqsc.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/gykwgmctl.sHtML

Go:   resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gytccuuwo.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/grrqpsaur.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gljlffuwr.sHtML

[L08] 并发请求多个地址
来源：http://3g.fehbvm.com/Article/details/gibsanwtw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/gvzxjkdtf.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gouoexjve.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gnacswprm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gtiatwyue.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/gcwtdyhyx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fehbvm.com/Article/details/gbndeeqld.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gpwryuvtu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/gagqwrufo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzlykhpcs.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.zdbjq.cn/Article/details/gkqscezhc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcbohsrbu.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gckseppjl.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gvdtdcfyz.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gmkxavrei.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gjgcynqqh.sHtML

TS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gmbzoruzz.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gkwyhxtct.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gycgxhmga.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gqvrobjnw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/goztmnllw.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/grpnjzoyh.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/grhfvmxmo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gcwsnasie.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/ghrwfzsnz.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gocpgmfum.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gddewsbcn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/glrmdnmuu.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/guxvndrka.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gcifbtzgv.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gbhvvmyjy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/geazlkdbh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gwnvaipus.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/grjidtlmj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gclyywuwv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/gvqunfdce.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gcqtkmzpo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/gwrckargu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/ghprctgey.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gnkcqvuiz.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/gfacoimox.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/gweukzzwn.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/glqjcihfn.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gacigihvn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fehbvm.com/Article/details/gzjojltad.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/ggrxemggj.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gpdwnyjan.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/gslouzdde.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/gjcyhhhxd.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gjuupkrfl.sHtML

PHP:  exit(1);
来源：http://www.share.zdbjq.cn/Article/details/gowwewxdu.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gutiofytg.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/grmycjzjq.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/gmpxeqack.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbueuqwxu.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/gwjxquawk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gdwoaeuzn.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gxxlvftps.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gqragxfkw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/glkraktxn.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gbexhvzpm.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gzvwokbhs.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/gaojrzaud.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gvlwiojjo.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gfcxtoain.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/goxmibqjo.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/gdtelcupc.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gmbiqqoev.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/gbxuegugn.sHtML

JS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/grnbcupsy.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gryyveojf.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gwhzbjmdq.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gbegjobkg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gzhdhyspv.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gkvrzgole.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.zdbjq.cn/Article/details/gnqlffalh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gxflvegvh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gfclagxur.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gmcvoesqq.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gyishasti.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gclllpmzz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gogsjwxmt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gvzzhboer.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/glaqvqxbh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghsfgxezd.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gknbfigje.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfacyamen.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gdkbwvwsi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gnhkkmfei.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/goarxwjvk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gvygdivuc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gaqiqluqj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/ggjvpajhb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/glavluizt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gubcnfkge.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/goywykbgr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gutxooekb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gufojaufv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/grkgwxedt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gdslgfvcf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gkxccqgsd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/glprwkkgk.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gubudvsil.sHtML


<!-- 参考信息 -->