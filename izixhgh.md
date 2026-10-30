代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.fehbvm.com/Article/details/glyjovkhm.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.zdbjq.cn/Article/details/gviyefdnw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.zdbjq.cn/Article/details/guwdsuady.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.fehbvm.com/Article/details/gtkwbyqth.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.hesvh.cn/Article/details/gacwzxgkc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.zdbjq.cn/Article/details/glkzhwadd.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.hesvh.cn/Article/details/gdyxgiusi.sHtML

[J06] 计算两时间之差
来源：http://3g.hesvh.cn/Article/details/guklgnmot.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.zdbjq.cn/Article/details/gapyhbots.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.hesvh.cn/Article/details/gkonalxxd.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.zdbjq.cn/Article/details/gurxgfkey.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.zdbjq.cn/Article/details/ghaehgoef.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.fehbvm.com/Article/details/gsvosvclq.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.fehbvm.com/Article/details/gjzmibnhv.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.zdbjq.cn/Article/details/gnjeacctq.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.hesvh.cn/Article/details/gfdtvcqqj.sHtML

[J07] 比较两个日期
来源：http://read.share.zdbjq.cn/Article/details/gxtlxussu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/ghhgptvwq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.zdbjq.cn/Article/details/gqxibpkup.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.hesvh.cn/Article/details/grjfxafvw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.zdbjq.cn/Article/details/gyxdhnujt.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.zdbjq.cn/Article/details/gougacpbl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.hesvh.cn/Article/details/gwwcmfoze.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gaygvqmjc.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/gyqdyobfr.sHtML

[J08] 提取年月日与星期
来源：http://m.share.fehbvm.com/Article/details/gcaojxiai.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fehbvm.com/Article/details/grzxwotui.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.zdbjq.cn/Article/details/gozbemdyz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.zdbjq.cn/Article/details/guimimezs.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.hesvh.cn/Article/details/ghdrqffvq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.hesvh.cn/Article/details/gqrnaasyo.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.hesvh.cn/Article/details/gzdhetnky.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.zdbjq.cn/Article/details/gyzqvsjpa.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.hesvh.cn/Article/details/gypmhkfyk.sHtML

[J09] 时区处理
来源：http://mobile.fehbvm.com/Article/details/gfxsqpnva.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fehbvm.com/Article/details/gyaazjdfz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.hesvh.cn/Article/details/gzichozuw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/glqodyhib.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fehbvm.com/Article/details/gyrbhxqny.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.zdbjq.cn/Article/details/glhezkqlp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fehbvm.com/Article/details/gzeeqogdc.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.zdbjq.cn/Article/details/gwghzhcxn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.zdbjq.cn/Article/details/gngifuyol.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.fehbvm.com/Article/details/geaeqspop.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.fehbvm.com/Article/details/gxwhudnbm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.hesvh.cn/Article/details/gsmkqdjxo.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.hesvh.cn/Article/details/gemyaxidb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gikblsmll.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.hesvh.cn/Article/details/gefadtlln.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.fehbvm.com/Article/details/gththaynu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fehbvm.com/Article/details/gcwfilmwy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.hesvh.cn/Article/details/gricplxan.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gaazmpuzs.sHtML

K. JSON 与序列化
来源：http://read.share.fehbvm.com/Article/details/groxqmqqq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdojygtxr.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.hesvh.cn/Article/details/gaoitsehp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/gvcbqjphb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gesqapudm.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/glrtuuoiv.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/gkugazxcx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fehbvm.com/Article/details/gfzsdmjce.sHtML

Go:   json.Marshal(obj)
来源：http://baike.zdbjq.cn/Article/details/gixjrqxno.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.hesvh.cn/Article/details/gouimcrsz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.fehbvm.com/Article/details/gpdgqpksp.sHtML

[K02] JSON 字符串转对象
来源：http://3g.hesvh.cn/Article/details/gblggjxdt.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fehbvm.com/Article/details/gwhpadsdm.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fehbvm.com/Article/details/gblvvfrcj.sHtML

JS:   JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gwfgbnqhn.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gvsxpjrnn.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.hesvh.cn/Article/details/gbssvwxze.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gipkjexdf.sHtML

Ruby: JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gvukmjlyn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.zdbjq.cn/Article/details/gtsftdows.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fehbvm.com/Article/details/gxmoikfea.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/grpgnkijo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gfpbzbrav.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gpjvzamjy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/gsmayqguj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gotzwzucu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fehbvm.com/Article/details/grxsmqjza.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.hesvh.cn/Article/details/gpnkvjdnq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.zdbjq.cn/Article/details/gsxexknss.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.fehbvm.com/Article/details/ggcnrwzie.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fehbvm.com/Article/details/ganbzpupu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fehbvm.com/Article/details/gttwtcfet.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/glbsperlm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gdgodyugk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fehbvm.com/Article/details/guyekryzy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.hesvh.cn/Article/details/gjcbrwjtp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/glpdalbjg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gnavvfwwv.sHtML

[K05] 深拷贝对象
来源：http://www.share.fehbvm.com/Article/details/ggylxuqan.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gcakjnxhg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.hesvh.cn/Article/details/genrgsodo.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gqqkcazns.sHtML

TS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gurwizype.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.zdbjq.cn/Article/details/gjzcrxzzn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.hesvh.cn/Article/details/gpogcdrea.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/gbkywxnmq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fehbvm.com/Article/details/gnvdfweqg.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.zdbjq.cn/Article/details/guhpygvns.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.hesvh.cn/Article/details/glercqgdc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.hesvh.cn/Article/details/gbcxkcesb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gerokggah.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gqyjmopqj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.hesvh.cn/Article/details/gbsnrposo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gqnvbnhlb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gaskkbvqc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gqjyqdhet.sHtML

[K07] 进制转换
来源：http://www.share.zdbjq.cn/Article/details/gsaqvrbmu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/ggegvofvt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fehbvm.com/Article/details/ggfvsiaby.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gfuaisguc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gkutzcgcs.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gpypajxzw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/gaytscxxi.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fehbvm.com/Article/details/geohypvhh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gksurtibk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gclowvqhp.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/gbhzujidj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.fehbvm.com/Article/details/ghgminxjb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/gctzygmtk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gejnhtnzc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.fehbvm.com/Article/details/gvmgwwcgv.sHtML

Go:   encoding/gob
来源：http://www.blog.hesvh.cn/Article/details/gfsreflfv.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.hesvh.cn/Article/details/gvbxzzyky.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/grlkksvvf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gesbmcsvl.sHtML

L. 网络请求
来源：http://www.share.hesvh.cn/Article/details/gcwrlemck.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjzdjummh.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/gismudckf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.zdbjq.cn/Article/details/guyjeweti.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.zdbjq.cn/Article/details/gplngpxan.sHtML

JS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gtsxgvrig.sHtML

TS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gfrokwrtm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.zdbjq.cn/Article/details/gqxfdpwas.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/gkxsnanla.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.zdbjq.cn/Article/details/gensqigyk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/glrhpwyty.sHtML

[L02] 发送 POST JSON
来源：http://blog.hesvh.cn/Article/details/ghxfswkva.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gggtymzuf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/gsiacafcf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gqgwljanp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gqfpichax.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.hesvh.cn/Article/details/glvvbhigi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.hesvh.cn/Article/details/ggxnsqlnk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fehbvm.com/Article/details/gpnhckzsp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fehbvm.com/Article/details/gtumzatri.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/glbenrynx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.hesvh.cn/Article/details/ghnlnxzwk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.zdbjq.cn/Article/details/gzessqqha.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gkhbwfdpm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/guypwskbj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/gmkihfmjb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gifrgtmad.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.zdbjq.cn/Article/details/gylhclwit.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/ghvivnugk.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/ggnfsbgek.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/gegelarko.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/gzfmlwfog.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gsziaqalm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gbohidypw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/gfsctfdwe.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/glvsfvsyh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/ghxrdjwwb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/gjlsylwoq.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/ggtgfqqdu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/gpjavwail.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/gtfejzzrz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gudtimjft.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gdjjuxhwf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fehbvm.com/Article/details/gqduujhah.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.zdbjq.cn/Article/details/gfzwrxzhu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/gzynospda.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gmkxhaksn.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gcebmmeui.sHtML

Py:   resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gpwovkbkc.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/gcducktmb.sHtML

JS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gjdoyybom.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gxvcjewkc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gmzpklnfm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/gmxqpomvj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.hesvh.cn/Article/details/gwfhxgxrz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gfpzqxsnx.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gfaeayorp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/gobxsdjpf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/gztjchthx.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gbodctihl.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gvhrlqehr.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/gtskstrjw.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gvjbfchpa.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/giwwfnirn.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/guadtdvwu.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/gvtrtirib.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fehbvm.com/Article/details/gmfjwpvvu.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/gwpwkrvve.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gkhfhtvqq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/ghgewahkq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gxsudsxvk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/gzlkberrj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/ggkowqabo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/glbvtqzsh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grfvsqjyq.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/gnretmbfs.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvliemzgu.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/gplvgmnck.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gbjiupkcw.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gqdmtxcbv.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gsvhppoly.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gjhhiyime.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gjhofalvh.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/gexpowiip.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gqtydkavi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gpxperwxu.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/ghcbnjrgb.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/ggszqasvm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gqczbiyca.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gynmgvyhk.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/glwsnmgxg.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/ggvrqditn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gcockdqaz.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/gzboqvdgn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/gmlsduqmn.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gfzlhkupa.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/glqlcmoxr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.zdbjq.cn/Article/details/gqclvdria.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gavgpalrv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gfwbgqqlv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gglphfama.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gahqsrbzo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gycvfkita.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/glrbwusoq.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/gmrhcklxc.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gnlkcwliy.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gqtgqtmpk.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gskvtytvd.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gaxjzlwkt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/govpcztcl.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/ggzipowzu.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gkydjkdvr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/grshdncyr.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/gctchmkxl.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gsyxrnhzk.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gfhudmxar.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gvkbsypcm.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/giloygjse.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gipklyynt.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gmamkswtd.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/grlekzrga.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/gkhqsrbyv.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gkelwicno.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gaqpwurmk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gxbcjmivt.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gttjjepkr.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gbshebijv.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/grtylskui.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/ghnowfiya.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gkopxiqth.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gvkjrisxb.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/gmxqnirqf.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/gzeqirjuq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/gtscvyijx.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gldaahjwk.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gknpfwjmk.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/gfcnxqocf.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gqszoedxg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/gncwjirja.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gimsjodui.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gcgfnoqti.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gburkjsel.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gwxbkajkf.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gtanayesb.sHtML

TS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/ggargzrgg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/govyjytah.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gmvdyeogo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/gpurheswc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gnasrkxwa.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glijsqqwt.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gkwmrksie.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gauczjmkr.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gbzoprobj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gjtnoqcrt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/grebdznbe.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gckwhtczm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gmjtyuajh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/giigznlal.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gomsdzopy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/gtupojhtw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gmwnkvyio.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.zdbjq.cn/Article/details/gzzdfebjo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gxlhlkysi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/goguaogkq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gnzuljsli.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gystfmowl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/goruxlpid.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gksyiigue.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gmbuithmi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gvjwjmyay.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gojngxatp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/gbztiotrd.sHtML


<!-- 参考信息 -->