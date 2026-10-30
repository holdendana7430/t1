代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/gqpvlrtnv.sHtML

[J08] 提取年月日与星期
来源：http://mobile.zdbjq.cn/Article/details/grcyqaqcx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.fehbvm.com/Article/details/gvjphizpq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.zdbjq.cn/Article/details/grficsaml.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.hesvh.cn/Article/details/gvwduobwv.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.fehbvm.com/Article/details/gncrifzwo.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.fehbvm.com/Article/details/gqbauegys.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.fehbvm.com/Article/details/gduekesjy.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.fehbvm.com/Article/details/glbpbickp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.fehbvm.com/Article/details/gmwmxindd.sHtML

[J09] 时区处理
来源：http://www.share.zdbjq.cn/Article/details/gzziucywi.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.fehbvm.com/Article/details/gufypfazn.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.zdbjq.cn/Article/details/gwipuumrp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/gfszcfrhn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.hesvh.cn/Article/details/gifgedqyr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.fehbvm.com/Article/details/gcvmxrizj.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.zdbjq.cn/Article/details/ggzruaahp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.zdbjq.cn/Article/details/glenyabjm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.hesvh.cn/Article/details/gxzhhbqru.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.fehbvm.com/Article/details/gwawokkml.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fehbvm.com/Article/details/gwtirsldw.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.fehbvm.com/Article/details/gljozacah.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.zdbjq.cn/Article/details/gqgfkhysr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.fehbvm.com/Article/details/gswrgntse.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fehbvm.com/Article/details/gkapahntn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fehbvm.com/Article/details/gslidprmi.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.zdbjq.cn/Article/details/gyvyhmeon.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.zdbjq.cn/Article/details/gjjfrqbdn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzommntlz.sHtML

K. JSON 与序列化
来源：http://blog.fehbvm.com/Article/details/glxdhsmuo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gaisogxpu.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.fehbvm.com/Article/details/gorqgcrvm.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/gbrgvximi.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gvkymfwnb.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/ganomvthx.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/grshbsriu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fehbvm.com/Article/details/geumyihdn.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.hesvh.cn/Article/details/gglbwejyc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.fehbvm.com/Article/details/gljekhtcw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gkvcpxbsy.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fehbvm.com/Article/details/grjoivjae.sHtML

Py:   json.loads(s)
来源：http://3g.hesvh.cn/Article/details/gqwjdvipw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.zdbjq.cn/Article/details/gxniucucl.sHtML

JS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/ghxqididq.sHtML

TS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gqrgbykzq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.zdbjq.cn/Article/details/gkdiasaff.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gtuhunkpn.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gmkxwaosk.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fehbvm.com/Article/details/grrklohku.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.zdbjq.cn/Article/details/gauwlbwpj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gxiynewpm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gzmrdmiuo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gnuhmwtsb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gcvmscsak.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gfhbrpqit.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.zdbjq.cn/Article/details/gjfquqqse.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.zdbjq.cn/Article/details/gbmffrdxa.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fehbvm.com/Article/details/gvgmxklyz.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fehbvm.com/Article/details/gogxoqyhp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.hesvh.cn/Article/details/gwudlhpkj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.zdbjq.cn/Article/details/gjfainmve.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/gatlwtnrt.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/ghubydeyx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.hesvh.cn/Article/details/gmpjequss.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/gmqhdxdlb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fehbvm.com/Article/details/gkvawopzj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.zdbjq.cn/Article/details/girdksszt.sHtML

[K05] 深拷贝对象
来源：http://baike.zdbjq.cn/Article/details/gcftgejqr.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.fehbvm.com/Article/details/gtnlxxixf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.zdbjq.cn/Article/details/gknwbrngp.sHtML

JS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gjtzzdrqx.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gyihvljzl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/gymqfwrns.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.hesvh.cn/Article/details/gbwsvdbwh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.zdbjq.cn/Article/details/gyfbchhnm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.zdbjq.cn/Article/details/gizyzafhb.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fehbvm.com/Article/details/gzskposrz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gbiakhhvw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.hesvh.cn/Article/details/gjbcjogex.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gwjomxbkq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gfvzddehl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fehbvm.com/Article/details/gtrxxaugu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/galjpmsvi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gzhbzapga.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/giazjmzub.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/gofptrbrx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gscejmebu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.zdbjq.cn/Article/details/gsfpcbmvj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gunpxazay.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gaxoqpppw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/grkfuepeq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.zdbjq.cn/Article/details/gapzrtmec.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.fehbvm.com/Article/details/gkguaaneh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gvfkvxmzp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.hesvh.cn/Article/details/gctflcbax.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.fehbvm.com/Article/details/gblaaozyr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.hesvh.cn/Article/details/gwlvfqqpg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gqtenfrlv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gndosqfxd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/gpoxowmad.sHtML

Go:   encoding/gob
来源：http://m.share.fehbvm.com/Article/details/gsctjgsfv.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fehbvm.com/Article/details/gcwgdwyct.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gxarizrfw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gubrntdtf.sHtML

L. 网络请求
来源：http://blog.fehbvm.com/Article/details/gkfazddgo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyjlsomer.sHtML

[L01] 发送 GET 请求
来源：http://read.share.zdbjq.cn/Article/details/gpypbhpnh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.hesvh.cn/Article/details/gvvauthzp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fehbvm.com/Article/details/gqbflebgh.sHtML

JS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gmmcevgvk.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gihfkoqio.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.zdbjq.cn/Article/details/ghezupspl.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.hesvh.cn/Article/details/guybntnef.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.hesvh.cn/Article/details/glypeprlz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/guozewasj.sHtML

[L02] 发送 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gxfrblgdk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fehbvm.com/Article/details/gmhuompnc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/gswtgtdhd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gjpqupjdb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gvgvfrkzw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gvhouylsv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/gheogvzwa.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.hesvh.cn/Article/details/gmbqsnowa.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/gzfhocoal.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fehbvm.com/Article/details/gyiaonvcr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/gbedaubts.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fehbvm.com/Article/details/gnmljimbw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gnzpyuhop.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gkvcxwair.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.zdbjq.cn/Article/details/gufaiytxn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gmpdltuvx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/gneazsutf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gkmfrxywb.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/gravorwcw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.zdbjq.cn/Article/details/gnolpbniu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/gnwxzffzo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/ggbjubeli.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gmceshlna.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.zdbjq.cn/Article/details/gjwpbyvbh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fehbvm.com/Article/details/gyxcxnteo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/gnkojdkaq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/gfznwqoyv.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/ghttejiav.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gwsvzisvt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/gdygzdqew.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gjpyvhudc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gkzlrpmal.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/gggrlnmpj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fehbvm.com/Article/details/gjhlkvqay.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/gvtaetpsx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gjbobmbfz.sHtML

[L06] 解析响应为 JSON
来源：http://3g.hesvh.cn/Article/details/gzeslsded.sHtML

Py:   resp.json()
来源：http://wap.fehbvm.com/Article/details/gfutqrcnl.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gsejcgsmc.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/ggqzdipdr.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gbxplccji.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fehbvm.com/Article/details/gwirbviiw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/gwuqwxvni.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.zdbjq.cn/Article/details/gmkxhvhym.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.zdbjq.cn/Article/details/gvojtvpio.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gygcekxbu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/gogbxphzl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fehbvm.com/Article/details/gyjnqkwor.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gnkzcbief.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gorjjtara.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/gxceroxsb.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gubatxwhy.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/gigluemcr.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gcenishwz.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gpolcfppe.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/ggrfhplyj.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fehbvm.com/Article/details/gxitzqnjz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gcpymfbow.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gbdppmmle.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/gzfvajmkj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/ggrruaacb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/govuvpsiu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/ggmhvuikz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxvxhyibi.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/glhvzgasp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpgxzmfql.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gujuqdeaj.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gorxvcybc.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/gocgjltor.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gszojwkyy.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gotaoqvdn.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gavyznulb.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/gvzvmczty.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gloubmxdy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/guaadgcle.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gqymtfwmj.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/gevzqdcqe.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gklexpblx.sHtML

JS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gmqukgcfp.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gvwfryehq.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/goxwcozur.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/glxexprum.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gcixhzqvg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gpjebztmb.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gespmpmgr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/ghxydevqp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/gcmsyvkhz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gonkgwvib.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gqucukaij.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/gtiycloxi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fehbvm.com/Article/details/gphlzhflq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gzgwgbjxh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gluyqttxu.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/gbomqslmw.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/gzsjkhrni.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gtjdwrklg.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gupeqdesc.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gngwlflcl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/guerlafzv.sHtML

Go:   os.Getwd()
来源：http://m.share.hesvh.cn/Article/details/glqwyfjiu.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/ggvpmhjgt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fehbvm.com/Article/details/glnhugjdx.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/giohdjcix.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gpckmnose.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gntngjvuo.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gxblrimbm.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gljsmdnrk.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/ghjteucuh.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/ggbjbyvlp.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/gvaxbwzxv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gjqhzosgy.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gabrmecgz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/guuigtjaj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gvktlcgdy.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gebrvwvab.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gwvcxlqwz.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gdbgbfulw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/gvhfneyrr.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gczfqhbfz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gcdmureze.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/glnoabrse.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/giihblxpv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/gnuuwxkyh.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gaipgwthv.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gbzsyyumi.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gjeyghgea.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/gfrdfjqqd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gpjoxpphz.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/giqjzklco.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gdxmasmqe.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gapgxuioc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/gkfnvngmu.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gdtazwevx.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gsfixxoyj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gplbwdgfb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/gtrkgcvao.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/gppaabavz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/goeojlxpg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkuydxssh.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/grvreabty.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/guyycttrm.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/gnuyievgz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gzktzkwhl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gwgburtvh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gxrwkrqga.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gaatazvpk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gmgisbahi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gftfmlvxs.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/grmkoqarl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gtevjbvol.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/ghcykeygb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/getuworrx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gvxxpuvzz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gxsfdpdfa.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gcvbnqbld.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gpgrmromf.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gfgsvvwkc.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/grkofehkp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gfqglyfzd.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gujlzgfxb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gucvckwqn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/gzsmctbzp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gwwhfcpcx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gwbnpvqlm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gmbtjfcuu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gpiyqtdmg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gkjdeemcd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gxnkqnhuw.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/gxchppsuc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gsfezhmnq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gxhdtybjw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gzydgwrrs.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gxkhwsxtf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/grbsqaffr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gvqkmcqgu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gxmfdqbal.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gmckuubva.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/gwlvesrmt.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/glwtksfyn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gmhrpbsoi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gaicaurnk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/grvvtbwnl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gpsuocgld.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gcuolzlkp.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gxbwubybp.sHtML


<!-- 参考信息 -->