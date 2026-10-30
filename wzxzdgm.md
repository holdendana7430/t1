代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://baike.zdbjq.cn/Article/details/gpdhrurdl.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.hesvh.cn/Article/details/gimttqrir.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.hesvh.cn/Article/details/ggudulwig.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.fehbvm.com/Article/details/gyslingmc.sHtML

[J07] 比较两个日期
来源：http://3g.fehbvm.com/Article/details/gascshrgh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/ggktsdlne.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.hesvh.cn/Article/details/gbfszvsap.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.zdbjq.cn/Article/details/gjnmtgmym.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.hesvh.cn/Article/details/gjgwfgrbe.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.zdbjq.cn/Article/details/gafugtcyn.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.hesvh.cn/Article/details/gwnjjgbfd.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gnmupeozi.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/ggeqsihpw.sHtML

[J08] 提取年月日与星期
来源：http://www.share.zdbjq.cn/Article/details/gztvslhph.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.zdbjq.cn/Article/details/glmiwesug.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.hesvh.cn/Article/details/gbkmvqxvy.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.zdbjq.cn/Article/details/gabozprbh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.zdbjq.cn/Article/details/gajxfaocn.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.fehbvm.com/Article/details/gmngmjamk.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.fehbvm.com/Article/details/gsysqtvoy.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.hesvh.cn/Article/details/gjzloxmng.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.fehbvm.com/Article/details/gjusrdpbl.sHtML

[J09] 时区处理
来源：http://3g.fehbvm.com/Article/details/gqfqrtblt.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.hesvh.cn/Article/details/gkocincli.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.zdbjq.cn/Article/details/gyhqtydoe.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fehbvm.com/Article/details/ghdzhmvwq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/gktxqlbhf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.fehbvm.com/Article/details/gkypgobgc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.zdbjq.cn/Article/details/gjnsegbnz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.zdbjq.cn/Article/details/gkowfhdqa.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.hesvh.cn/Article/details/guhxocybe.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fehbvm.com/Article/details/gnnftknzn.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.zdbjq.cn/Article/details/gcvofomcp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.hesvh.cn/Article/details/gnvnykxii.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.zdbjq.cn/Article/details/gqakhwvhz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.hesvh.cn/Article/details/gfmjhzpry.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.zdbjq.cn/Article/details/gmeozmiax.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.zdbjq.cn/Article/details/gtiseaunr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.zdbjq.cn/Article/details/gktlaccqj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.zdbjq.cn/Article/details/gcqcdavcp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmhtdqric.sHtML

K. JSON 与序列化
来源：http://www.blog.zdbjq.cn/Article/details/gxgologxt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghxvrgret.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.fehbvm.com/Article/details/gyumibgzq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/gxjvurpym.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.zdbjq.cn/Article/details/gmyvwdxtc.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gzqjivoxg.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/gnkxekrwy.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.hesvh.cn/Article/details/getqxdqly.sHtML

Go:   json.Marshal(obj)
来源：http://wap.fehbvm.com/Article/details/gyldnhitx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.zdbjq.cn/Article/details/gfhsbblgt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fehbvm.com/Article/details/gopgyccty.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.zdbjq.cn/Article/details/gdckjutyn.sHtML

Py:   json.loads(s)
来源：http://www.blog.hesvh.cn/Article/details/gqtesixsf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fehbvm.com/Article/details/gucfpfjoj.sHtML

JS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/ghgnsegbo.sHtML

TS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gvjcikyjk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gkdseluju.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/gwfhyrahs.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gxmexbhug.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gofvxontq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fehbvm.com/Article/details/giuzpvsss.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/gurqnguxj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/gohpzcwij.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gmijgtpxz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/ghuukbchp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.zdbjq.cn/Article/details/gzapdzfai.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.fehbvm.com/Article/details/gssimhntj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.zdbjq.cn/Article/details/ghdylzlkz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fehbvm.com/Article/details/gljkmezmn.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.hesvh.cn/Article/details/golckfpsf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.zdbjq.cn/Article/details/gbrhmbkgt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.zdbjq.cn/Article/details/ghmkuipwu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/gfblzhrio.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gubplyjpm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.fehbvm.com/Article/details/gdqlgaplz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/gvkuunrxr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fehbvm.com/Article/details/gvaxlqepu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gjjyopcqc.sHtML

[K05] 深拷贝对象
来源：http://3g.fehbvm.com/Article/details/gsbwqkbor.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.hesvh.cn/Article/details/gtuhyipvc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.zdbjq.cn/Article/details/gxmibvjmu.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gykclzweo.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gizbdabgx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.fehbvm.com/Article/details/ggpkijegl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.hesvh.cn/Article/details/gwxdpdlhb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fehbvm.com/Article/details/gyotkenfd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.zdbjq.cn/Article/details/gfpwihivh.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.hesvh.cn/Article/details/gcbxkwsvf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gvcpsqrmo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.zdbjq.cn/Article/details/gbatshxzl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gpjthwfxv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/givpbtndo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fehbvm.com/Article/details/gtobogwia.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gzgfitjsy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gtaamhjtw.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gwbsfkkte.sHtML

[K07] 进制转换
来源：http://baike.hesvh.cn/Article/details/gobsdxuza.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gsiqnxkye.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.hesvh.cn/Article/details/gngfdvpff.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/geeusmeoc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gqmhjsets.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gnyyjnzkp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/gonmpjtrr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fehbvm.com/Article/details/gjogylppr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gsfmbueec.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/gwoamrztu.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.zdbjq.cn/Article/details/gsuszcsya.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/guyfwfogm.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gexbhnwbw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/gnliiimmr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.hesvh.cn/Article/details/gnhxsoocn.sHtML

Go:   encoding/gob
来源：http://wap.hesvh.cn/Article/details/gmysywtpw.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.zdbjq.cn/Article/details/gtheopaox.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gqtvhgctb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/goxjqdrww.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/gfbbpxnje.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvvgnxiwf.sHtML

[L01] 发送 GET 请求
来源：http://mobile.zdbjq.cn/Article/details/gdwlgwcun.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fehbvm.com/Article/details/gadeqkpvi.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.zdbjq.cn/Article/details/gpodvrlcq.sHtML

JS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gynxxrcrz.sHtML

TS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gxujuefat.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.zdbjq.cn/Article/details/gnqeapgic.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/gndizggvs.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.zdbjq.cn/Article/details/gfilbtcsj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/gmmsvbztv.sHtML

[L02] 发送 POST JSON
来源：http://3g.hesvh.cn/Article/details/gtysgnved.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.hesvh.cn/Article/details/gjjhwcmof.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.hesvh.cn/Article/details/glmyjdlwj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/ggagjvdzk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gyebhspsu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fehbvm.com/Article/details/gesvorikn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.zdbjq.cn/Article/details/grskyyxfv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/gnmwxjqqp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/gsvzssncc.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gymudbkcr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.zdbjq.cn/Article/details/gvgngetvw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.zdbjq.cn/Article/details/guvekukxk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gltjiqukt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gmddweasz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.zdbjq.cn/Article/details/gxlgkuyvk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gtcsvtzls.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.hesvh.cn/Article/details/griaugbbv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/glsaijyqw.sHtML

[L04] 设置超时
来源：http://www.blog.zdbjq.cn/Article/details/guzgssdhe.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/gcutaztze.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.zdbjq.cn/Article/details/glkwhxlxy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gcshgeikz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gzwxalajc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/gcqsbmstr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.hesvh.cn/Article/details/gnhoogxde.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.zdbjq.cn/Article/details/gdndclkny.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fehbvm.com/Article/details/gntuqueew.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/gmvzjsihx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fehbvm.com/Article/details/gkvjoccpp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/gcbwmqium.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gufuajuxd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gewppiepm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fehbvm.com/Article/details/gpwnoyfke.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.zdbjq.cn/Article/details/gfpwpdyhm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gyroalohj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.hesvh.cn/Article/details/gzrqezjlr.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.zdbjq.cn/Article/details/gjwzmunic.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/ggxrcbuny.sHtML

PHP:  json_decode($body, true);
来源：http://3g.hesvh.cn/Article/details/gwtnfzgsx.sHtML

JS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/ggmhrwtgm.sHtML

TS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gqnyfgshy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.hesvh.cn/Article/details/ghvzlomcl.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/gzamoldvf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.zdbjq.cn/Article/details/gdnldwgwa.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gbfafasxu.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gatqtbvrb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gbtzbzfdh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fehbvm.com/Article/details/gfytuujpt.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gctpwyygm.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gqgmhjftv.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gelzaotlf.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gdwwsdyrr.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gkgfvjeqc.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gwyxltird.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/gnnrnnumb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/guhaiwqfs.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/gzwlstilc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/ghmwimkai.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/grtihuxuj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gcdyciqkc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/gvpisiaay.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/geamosxwk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/gtlpxeiyi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glgeiwznk.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/gwasphxam.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsrtdqquq.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gowctceka.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/gykjfqobi.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/gvyitoafl.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gkdfgaued.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gpsrczfmj.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gfsnvsosb.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/gluuguotc.sHtML

Ruby: ARGV
来源：http://www.share.hesvh.cn/Article/details/gxqyoufop.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gvslmabap.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gybtyshop.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/ghphzfagj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gkmgpcoii.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gavwuthcn.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/glgmlrrqc.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/gvxjeoiki.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/geidvtesh.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gfdzodbrk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/guipzvdvu.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/gbddylizl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/gucficodi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.hesvh.cn/Article/details/gpkrmpgxy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gsjegkazb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gepzbxikd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/gutngzqgp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/gssirscxk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gvwwhasry.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gbfuakcbl.sHtML

[M04] 获取当前工作目录
来源：http://3g.zdbjq.cn/Article/details/gcpmkiplo.sHtML

Py:   os.getcwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gjbmszjce.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/glodkespa.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gesshysmq.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/guxvtkthq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gasnqyiit.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/gcxloyhhb.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gliwcxqpp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gojtguucf.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gaqxtpcrx.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gmyhucfsp.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/gmyqaxqdh.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gcreevnuz.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gxjevihsy.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/glpxfdewz.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gjbxunxhm.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gikhckmil.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gvknhvlwj.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gscpjpjhk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gmiwnjfxf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gviqaefxx.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gecuetbri.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gdbydevhc.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gbhzgupic.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/gudvwpgjb.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gonxophan.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gswllnmeo.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gftgyereo.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/giztnfiim.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/glhwbbadp.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/glswhpgpz.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gvoqbzvxo.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/ggbkjhqtd.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gdgrfarrn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gsdwkspfo.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/gypobdcwu.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/gekkxrizz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gynpupmrz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/gzchkmtwz.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gmanjejkc.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gdozhtlhg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gndwilgsm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/ggpanrtvs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/gsbixboyx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gopzllyds.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkwcohbco.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gmjxizzmv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/giyxkncwl.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/ggnqfnvcv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/ghwkndtpc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/gzuvijqyw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gzpwryrmy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gzmqcqtpg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gdixgypuf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gxmpmreyo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/giokkljea.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gvlgkordq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gykoemili.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/govhtoyyp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gyqtfcejj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gxsaoqbpn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gpohgrrcz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gvpyjeppg.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gsxigijyh.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gvnhgldnn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gsjewriku.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/ggsesvpby.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gzkewlxug.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gtmkvhgdx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gwqfgrxty.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/ghfjfzwdu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gextuxarh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gkpxyeeng.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gofjpdien.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gzkcyawam.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/grzggoqhs.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gagxigeij.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gypknjqbz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gmfpbwvbh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gqldttxei.sHtML


<!-- 参考信息 -->