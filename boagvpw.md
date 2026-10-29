代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.zdbjq.cn/Article/details/gwrpnvbqo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/gyxzruupj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fehbvm.com/Article/details/gojgsbepo.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.hesvh.cn/Article/details/gdltqhtsb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.zdbjq.cn/Article/details/gkmnurxyz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.zdbjq.cn/Article/details/gkmzqatvd.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.zdbjq.cn/Article/details/gvupaggik.sHtML

[J06] 计算两时间之差
来源：http://m.share.hesvh.cn/Article/details/gkzyxyqsn.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.hesvh.cn/Article/details/gfqmdtgey.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.zdbjq.cn/Article/details/ghfbbbuse.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.hesvh.cn/Article/details/gbscjxtnd.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fehbvm.com/Article/details/gzfpilesi.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.zdbjq.cn/Article/details/gwzpxozqr.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.zdbjq.cn/Article/details/gcubkaobf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.zdbjq.cn/Article/details/gucdcjhee.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.zdbjq.cn/Article/details/gkkoemtla.sHtML

[J07] 比较两个日期
来源：http://mobile.zdbjq.cn/Article/details/gnyuagule.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gqofyttfo.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.fehbvm.com/Article/details/gzjdneoox.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.fehbvm.com/Article/details/gkwpwrzhu.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.zdbjq.cn/Article/details/gzzahchhk.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.hesvh.cn/Article/details/gqxrminak.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.fehbvm.com/Article/details/gjbbxiwtn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/gwfbbzoex.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/guicfhwwq.sHtML

[J08] 提取年月日与星期
来源：http://3g.zdbjq.cn/Article/details/gmlhnojat.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fehbvm.com/Article/details/gfosltmys.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.hesvh.cn/Article/details/gidefzrfd.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.fehbvm.com/Article/details/glsapddwn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.fehbvm.com/Article/details/grmcafsqe.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.fehbvm.com/Article/details/gtktnxbdl.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.zdbjq.cn/Article/details/ggqmbddyv.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.zdbjq.cn/Article/details/gldhkveyh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.fehbvm.com/Article/details/gqkcyjdpq.sHtML

[J09] 时区处理
来源：http://mobile.zdbjq.cn/Article/details/gxuczmttt.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.zdbjq.cn/Article/details/gxrmhlscq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fehbvm.com/Article/details/gbyoszhlk.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/gffppsjts.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.hesvh.cn/Article/details/gpmktieeg.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.hesvh.cn/Article/details/gwiyiecsx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.zdbjq.cn/Article/details/gwgwduuxp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fehbvm.com/Article/details/gqodxplbl.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.zdbjq.cn/Article/details/gnvylmtqq.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fehbvm.com/Article/details/gnfurbmkz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.hesvh.cn/Article/details/gixpajbhk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.hesvh.cn/Article/details/ggtafstek.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.hesvh.cn/Article/details/gjalikehv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.zdbjq.cn/Article/details/ghrpdexrp.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.fehbvm.com/Article/details/gqztkhmsc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.hesvh.cn/Article/details/gmcjsyzbm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.hesvh.cn/Article/details/ghkskgayo.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fehbvm.com/Article/details/gqvctffbv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdnlptpcw.sHtML

K. JSON 与序列化
来源：http://www.m.share.hesvh.cn/Article/details/gcgybbukl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gddiiiojm.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.zdbjq.cn/Article/details/gzbbgjpip.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.hesvh.cn/Article/details/gpeowpkee.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/grrgfmyuq.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.hesvh.cn/Article/details/gjmjackef.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gwkqotjet.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.zdbjq.cn/Article/details/grjsfrhgf.sHtML

Go:   json.Marshal(obj)
来源：http://wap.zdbjq.cn/Article/details/gbfceqmkz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.zdbjq.cn/Article/details/gmsfwsqzv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.zdbjq.cn/Article/details/gnmtohhsy.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.zdbjq.cn/Article/details/grdtwpxnv.sHtML

Py:   json.loads(s)
来源：http://wap.zdbjq.cn/Article/details/ggbnqjlcd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.zdbjq.cn/Article/details/gfjosvkno.sHtML

JS:   JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/guaimhziz.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/guacelopw.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.fehbvm.com/Article/details/glkcaziap.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/gybxxitjr.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gqadcceio.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.zdbjq.cn/Article/details/guhmpoclr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.zdbjq.cn/Article/details/gzggmqbbu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gazcaycjx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/gcexqqmzr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/gxuerddid.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gkmbxbcim.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fehbvm.com/Article/details/gpjwsuqru.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fehbvm.com/Article/details/gwobxudny.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fehbvm.com/Article/details/gqsfyreej.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fehbvm.com/Article/details/gzajqfzhn.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fehbvm.com/Article/details/ggglxtwlu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.hesvh.cn/Article/details/gcbrstfiu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fehbvm.com/Article/details/ghvdwwisk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/gqunxsfse.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gnsfeoedo.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fehbvm.com/Article/details/glgzcygaz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gbpyunoyr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gvtlgqzfy.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.hesvh.cn/Article/details/gqewjnezf.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.hesvh.cn/Article/details/ggmsqthpz.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gxvtplhhw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.zdbjq.cn/Article/details/guroaezap.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gqrpoejmn.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gjjygeejk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.zdbjq.cn/Article/details/goiovzbnc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.fehbvm.com/Article/details/gsjtsriey.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.hesvh.cn/Article/details/gnhdlyciu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fehbvm.com/Article/details/ghcqtnpil.sHtML

[K06] 解析 URL 查询串
来源：http://blog.zdbjq.cn/Article/details/gldcgslsv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.hesvh.cn/Article/details/gtzvjprtv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fehbvm.com/Article/details/gfpcardql.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gobjluzxo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/gkagzbumt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.zdbjq.cn/Article/details/gzemtakll.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/ghrzivkgb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gogjppfnn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gxjbniigl.sHtML

[K07] 进制转换
来源：http://blog.zdbjq.cn/Article/details/grhrcwbrs.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gjizehikd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.zdbjq.cn/Article/details/gcrhhyrpo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gmgyuefkd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gaewbvhul.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gxcyqmedt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.zdbjq.cn/Article/details/gsonadjon.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.zdbjq.cn/Article/details/gvbrlwmwc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gebiyvrxu.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fehbvm.com/Article/details/gvaqnjphp.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.hesvh.cn/Article/details/gcsfqipvy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.hesvh.cn/Article/details/gbtdbfztk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gvhuezqjl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gicubkmxi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fehbvm.com/Article/details/gifiscwfo.sHtML

Go:   encoding/gob
来源：http://www.m.share.zdbjq.cn/Article/details/gxtogdvpl.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.zdbjq.cn/Article/details/gtwtrbnmj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gctgkexkr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grxowecgw.sHtML

L. 网络请求
来源：http://baike.zdbjq.cn/Article/details/gjpoisiqu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkxztvcqe.sHtML

[L01] 发送 GET 请求
来源：http://3g.hesvh.cn/Article/details/ghrdevopo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.fehbvm.com/Article/details/gzetrcign.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/gqbbtrvbk.sHtML

JS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gytohobsz.sHtML

TS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gwtkkbmgg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/gzyfpujwx.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.hesvh.cn/Article/details/gnsbtzmhu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fehbvm.com/Article/details/ghkdfeock.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fehbvm.com/Article/details/gvzuslrjm.sHtML

[L02] 发送 POST JSON
来源：http://read.share.hesvh.cn/Article/details/ggnvtsqoa.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.hesvh.cn/Article/details/gvpezheif.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/ghoisansx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gtgklzkkq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gcgyesmig.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.hesvh.cn/Article/details/gafwipeul.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.hesvh.cn/Article/details/gmjsxqvcy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/gxsdeyxfr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.hesvh.cn/Article/details/gtmecuugs.sHtML

[L03] 设置自定义请求头
来源：http://wap.zdbjq.cn/Article/details/gxfpjnjqw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/gyvstclqq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fehbvm.com/Article/details/gylshkfbm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gsmahxkof.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gnljmfdwq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.hesvh.cn/Article/details/gvzrbzknr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gfkvivudi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fehbvm.com/Article/details/gfzugypby.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/glfzmtike.sHtML

[L04] 设置超时
来源：http://baike.fehbvm.com/Article/details/gilfptsal.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.zdbjq.cn/Article/details/godftbzqi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fehbvm.com/Article/details/gbuqqktyn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/givjxifad.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gvzvieumq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/gnyujqgne.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/gevowihzm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/gsyimjqou.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.zdbjq.cn/Article/details/gwdopvoet.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/gvuvwbqjn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.hesvh.cn/Article/details/gvedxavsp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/gsasrdrmq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gywpnxbgs.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gbcllbdwm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.zdbjq.cn/Article/details/grbazuqmi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fehbvm.com/Article/details/glhiiydzs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/gicvyzevs.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gsmabeiqu.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/gsagcyrpw.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/gnhtrcwrg.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/gbbjnxmrd.sHtML

JS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gcxjmbmuo.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gpedpopfe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gqopissxk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fehbvm.com/Article/details/ghcmpekzx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fehbvm.com/Article/details/gojgttinb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/gpgltgcdw.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gzbwarztg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/ggssqsmqz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/gegqpgbdh.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gtaqjvngd.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gcrjlgjkw.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/gtbjcbyvz.sHtML

Go:   resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gwbmgfado.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/gahsacngy.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gfeqhgewz.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fehbvm.com/Article/details/gpcjfhyse.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/ghlvquiav.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/gbyvzixef.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/glwlmtoss.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gscaihhsx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.hesvh.cn/Article/details/gzpgrtbxl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.zdbjq.cn/Article/details/gxhpvflpt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gqdwqzgjb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/gvifklcea.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/goupauwju.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.zdbjq.cn/Article/details/gewexyslu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gazqkqwjp.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/ghpkjjtvf.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/gxykdbblc.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/gqvqfrcuk.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gablaskqf.sHtML

TS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gfiajkjvt.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gkztgbqen.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gjqwibsrf.sHtML

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/gdkdilihh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gqufnnmut.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/gxsjkgeyr.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/gvheayuyc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gxflstpbb.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gdqulcyft.sHtML

TS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gytwlmdbq.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gwvngvcck.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/ggkecehnw.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gqkrrrzvu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/gpgdgsets.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gekittgas.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gxjlmkisn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gczqxwyem.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gkggsiztv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gzjamrvwk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/ggioosfxj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gsdapxiyf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.hesvh.cn/Article/details/gwyijvxbl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/gfyycqldg.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/gasopstwm.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gemnqqkdb.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/gupzhudlk.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gblhapyer.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gjsgfpfhv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/gcivreaez.sHtML

Go:   os.Getwd()
来源：http://wap.hesvh.cn/Article/details/gcwcyknjb.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gkyphfnic.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gtohoyaor.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/gwjuhghwf.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/ganrzxmet.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/ghhbtnkci.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gycbaktog.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gijkcaotr.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gzcxefvzt.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/grobwdxhu.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/gupfjlzle.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gxxtputht.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/gpzzoazgu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/grdeyvjju.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/geafirtwg.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gagyvmbfz.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gafjmtath.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gykttwipe.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/gvrgdmmnm.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gnijvrqez.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/govmgsfih.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/gknvuyqkl.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/gqhwyddks.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gqpnwmhvy.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/ggtamzppc.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/goskddzek.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/gsvytthoj.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gjewohapj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/gutekusou.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/gpwxgtnly.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/giakvrvvk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gutwljaiw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gopzxnkaj.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/geyausjze.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gxatufnih.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gjgriasrt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gvapjhmdz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/gmkutpyts.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gmhqtchfn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpzkxniqp.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/gjarjsemc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjyugnsnv.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gwsborung.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fehbvm.com/Article/details/gfqrlezwu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gbmwahndz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gmzpoxind.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gugqtnblw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gdzavszxn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gihsntszv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gayydbycq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gyptlklex.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gbglpxjoo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gfrazfmya.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gmedkgptb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gxzbsodbr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gnipdnulz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/ggwyxnqjx.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gcaifnwof.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gbenevuhm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/grseeoftp.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/geghsdlme.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/glrfcjfoj.sHtML


<!-- 参考信息 -->