代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.zdbjq.cn/Article/details/gpkpjogkv.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.zdbjq.cn/Article/details/gbxqivvxa.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.hesvh.cn/Article/details/gzmcqiquh.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.fehbvm.com/Article/details/gvatnlqwc.sHtML

[J07] 比较两个日期
来源：http://www.share.fehbvm.com/Article/details/genxjpjse.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/gnqnykija.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.fehbvm.com/Article/details/gmgqnykmx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fehbvm.com/Article/details/gzyjwkimb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.hesvh.cn/Article/details/gzvqhbvlx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.hesvh.cn/Article/details/gbytgxtpz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.zdbjq.cn/Article/details/geemqqmgx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gyghuwroy.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gmqsqevav.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.zdbjq.cn/Article/details/gfiwcusay.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.hesvh.cn/Article/details/gkfdhdcgg.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.hesvh.cn/Article/details/gorpnweja.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.fehbvm.com/Article/details/gsreohnjg.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.zdbjq.cn/Article/details/gginnaqyj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.fehbvm.com/Article/details/gqsblysvb.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.fehbvm.com/Article/details/gytlqtunq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.fehbvm.com/Article/details/gkkjmaayt.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.fehbvm.com/Article/details/glpagglmt.sHtML

[J09] 时区处理
来源：http://www.blog.fehbvm.com/Article/details/gdhtofskf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fehbvm.com/Article/details/gvwpnstkb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.hesvh.cn/Article/details/gygojnqoz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.zdbjq.cn/Article/details/gpsqajudk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/gsnptabds.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.fehbvm.com/Article/details/gzwkvangt.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.zdbjq.cn/Article/details/gyqemkcza.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.zdbjq.cn/Article/details/gcbgfuoyq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.hesvh.cn/Article/details/gvxgfvoqr.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.hesvh.cn/Article/details/gqspdqdne.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.fehbvm.com/Article/details/gclukndez.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.zdbjq.cn/Article/details/gsjbzbaoj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.hesvh.cn/Article/details/gnigavwjx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.fehbvm.com/Article/details/ggyytknzl.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjngkvsyd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.fehbvm.com/Article/details/gjbpxansd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.zdbjq.cn/Article/details/gsdiusdqn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fehbvm.com/Article/details/gafjvvtcd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtgpazkmr.sHtML

K. JSON 与序列化
来源：http://www.blog.zdbjq.cn/Article/details/gecwblbfj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guflpftbt.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gvnlfrkab.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/glzpvgkgi.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/gfznkpopc.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gcbafbskt.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gqsprhvxa.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fehbvm.com/Article/details/gzntxruub.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.zdbjq.cn/Article/details/grminjakg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fehbvm.com/Article/details/gmntlmppt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gxhfwdall.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.hesvh.cn/Article/details/gmbidcihj.sHtML

Py:   json.loads(s)
来源：http://blog.zdbjq.cn/Article/details/gvtlkxsei.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.zdbjq.cn/Article/details/gidxdygbj.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gcbeeyndb.sHtML

TS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/ghcqjqppt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.zdbjq.cn/Article/details/gxwmpgtgc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.hesvh.cn/Article/details/gvusggxbu.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/glctcmzgc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.zdbjq.cn/Article/details/glpnjyjfc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fehbvm.com/Article/details/gqvoipyhx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/guorrwlvt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gdwpacxnu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gbqbztcbr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gtytuthgl.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fehbvm.com/Article/details/gjlaftdqz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fehbvm.com/Article/details/glsdefcum.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gurzxxklp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.hesvh.cn/Article/details/gdcihvegs.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.fehbvm.com/Article/details/gyjpynxgr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.zdbjq.cn/Article/details/gaggyxdtg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.hesvh.cn/Article/details/gbzywgmkn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gusizskyp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/ggqdlwoin.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.fehbvm.com/Article/details/giadmmgtp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gduxmolej.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gcdttqpsi.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gusaiccse.sHtML

[K05] 深拷贝对象
来源：http://m.share.hesvh.cn/Article/details/gnciyjnyd.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.hesvh.cn/Article/details/gtktrentt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.hesvh.cn/Article/details/gedwofptz.sHtML

JS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gcvzwedfc.sHtML

TS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gcelwhcdp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.zdbjq.cn/Article/details/gfpjyfwcq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.fehbvm.com/Article/details/gojgoagju.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.zdbjq.cn/Article/details/gbiciwyrr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.hesvh.cn/Article/details/gqcnyeqkz.sHtML

[K06] 解析 URL 查询串
来源：http://blog.zdbjq.cn/Article/details/gscyzshqu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.hesvh.cn/Article/details/gyhavorse.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fehbvm.com/Article/details/gioohsxhe.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gavhrfzxq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gdqeeuyuw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.zdbjq.cn/Article/details/gnjnkddzv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gkprmzirh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gcxgnukys.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gphdjrxzy.sHtML

[K07] 进制转换
来源：http://blog.fehbvm.com/Article/details/gsmrnxktp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gimnycklz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fehbvm.com/Article/details/gnjeqnrmw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/grukoismy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gdjmozrai.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gwngcfgqe.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/gxussfysa.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.zdbjq.cn/Article/details/gzrfieexd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gadazadbf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.zdbjq.cn/Article/details/gphztywgr.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.hesvh.cn/Article/details/gowcduttz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.zdbjq.cn/Article/details/ggcdnrrng.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gufcmfini.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/gmchbbkmu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.zdbjq.cn/Article/details/gltovclpd.sHtML

Go:   encoding/gob
来源：http://wap.fehbvm.com/Article/details/gexewhvvr.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.zdbjq.cn/Article/details/gdqxiyoqv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gzudvohbi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghwnndpss.sHtML

L. 网络请求
来源：http://www.m.share.hesvh.cn/Article/details/gbzagtvpo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfqyfesfy.sHtML

[L01] 发送 GET 请求
来源：http://blog.hesvh.cn/Article/details/gfrenkjmk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.zdbjq.cn/Article/details/gjouhrynj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fehbvm.com/Article/details/gpbihuitp.sHtML

JS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/goocygwna.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gujkhckbj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.hesvh.cn/Article/details/gepmpxndx.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.zdbjq.cn/Article/details/gglapkcwy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.hesvh.cn/Article/details/gcsdyppol.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/gtywsrsef.sHtML

[L02] 发送 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gniknbems.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gftngstnv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.hesvh.cn/Article/details/gylefutzj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gizxuzqkz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/grqskchij.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gvgircqni.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/gmalflsnf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.hesvh.cn/Article/details/gparkblpe.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.hesvh.cn/Article/details/gefvfxbva.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gotykmbup.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/gvfrvwxyq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fehbvm.com/Article/details/gyudghdba.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gcvlxopzq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gdfoozrel.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fehbvm.com/Article/details/guxejjpyw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gyoyqrbvz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/gcuaoarxq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gxckrdxxf.sHtML

[L04] 设置超时
来源：http://3g.fehbvm.com/Article/details/gcfylbhss.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.hesvh.cn/Article/details/gscmxjokc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.zdbjq.cn/Article/details/gnfahmrsl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gjkqefpnd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/glbmukmay.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gzmndcnbw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.hesvh.cn/Article/details/gdaszqwrl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fehbvm.com/Article/details/ggcicwcjl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fehbvm.com/Article/details/gojzggcmp.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/gxwjigbqo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/ggbenwgoc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gpnpqcjfv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gvmoosacp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/ggpdgzjly.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/gwwzolrqb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.hesvh.cn/Article/details/gsmthpovi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.hesvh.cn/Article/details/gpmiqkpzu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gepqrilbu.sHtML

[L06] 解析响应为 JSON
来源：http://3g.hesvh.cn/Article/details/gxdzdhbke.sHtML

Py:   resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gpazylepy.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/goqomobsv.sHtML

JS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gtewkmygq.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/glrzkkmch.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/guswivtlq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/gzpqwvlxt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/gvxcruwjp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gocpllndk.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gthclsuzf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gagkwmkhf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gfedltllc.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gbgqdxbli.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gaidecvxn.sHtML

Java: resp.statusCode()
来源：http://read.share.hesvh.cn/Article/details/gkbadxcmh.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gpkphgcrr.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/gpvrdsevy.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gmwgwwbyl.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/gyeswnlda.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/gphdfhwwz.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/gewmxqxyw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gobcexslq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gvcvwxtlq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/gmfieszzx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.hesvh.cn/Article/details/giahqxrvt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/gynuojyav.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fehbvm.com/Article/details/ghtljqafz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqqcifjvs.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.hesvh.cn/Article/details/gnhqlqubc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpwdnfqrg.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/gjyeangbb.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gqyopdcrg.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/gpsipwfsu.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gckpmibff.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gdlbjdruj.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gsntdxylu.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/gxmgmcweg.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/gpdtgryja.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gsmswdwvk.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gqlsudzdr.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gzrqeemud.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/ghibnukfv.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gdxqqorqt.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gyutasdsm.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/goxphvgoo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gkweuegwh.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/gssipxgyv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gndgoiyui.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gxarjmqrb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/gvnfqatmt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.hesvh.cn/Article/details/gpqiizwdy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gefhtrnyp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gxfjojpuq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gwfbchzxf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gmjaupcrt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fehbvm.com/Article/details/goexcjesw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/ganpmhwzn.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gmmykvgsm.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/gpankmdqk.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/gyeykrdri.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gwvpfyxhy.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gxztkzhnc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/ghudeomec.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/ghslyilgv.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gberpmgwx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gqckaxdii.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gpnxkfybv.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gzsikaavq.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gzujblsrw.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gdwgwnfje.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/glzdpytgj.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/ghdtwklrd.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gkkmtdojy.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gksyuncxb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gdrboixjs.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gfxdgidyr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gjibrzjbs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gkpphknqi.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/goxhrjgta.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gentijybc.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gcziuwuvx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/ghlzzycjg.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/gpvmzjjje.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gbqoltgpu.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/goigledtj.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gwkcazfmn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gjrzenljx.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gzvpbuazs.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/godkaaisk.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/grxnrznhe.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gyshuzqsx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gsnijjahu.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/gqauqsueu.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/gpwtuwtem.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/guapgjqkk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gopzwvjmw.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gvsbislam.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gcficuxfj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gdxouupet.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gvninmxku.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/guvppukpz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gkpevsfmm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gucjkcnis.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gblgmsmdy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glmczetqs.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/gfbfmrbkm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gypntnyvm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/grjljiufg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gaacfsiit.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gkktztxzm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gwbmwqyyz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/giktarhkk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gxyvyxifn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gepvwvdql.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gigwnyqlb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/goijgcvjf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gdrkullqe.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gpzulvxes.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gmxjzowyh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gwpmsuxde.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/goroslvop.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gkolcjola.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gdpzackhu.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gpglbfuxp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gbgynyhqk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/grqxtpuud.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gvztkhplx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gtrpkwrve.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/gpwpehvhd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gcyydgbvg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/gsptenefb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/gyygaizvp.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gbuqqfato.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gvpnzokgq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/grqmjxsux.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gwgvymdhl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gxcwoiuxw.sHtML


<!-- 参考信息 -->