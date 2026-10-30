代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvblmdrf.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbunoxfhs.sHtML

[J09] 时区处理
来源：http://blog.fanxiaobao.xyz/Article/details/gqvwbwmts.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvygtmdpk.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.fanxiaobao.xyz/Article/details/glssouawb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fanxiaobao.xyz/Article/details/gloivwsfk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fanxiaobao.xyz/Article/details/gxuwhfyaz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfffsuhd.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqahswuk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzauhvccg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.fanxiaobao.xyz/Article/details/gciaphefn.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkufyndr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.fanxiaobao.xyz/Article/details/glgrrkokh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlrmjbtu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glacxjbxm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhrejzmj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxnsrmdi.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjuhaljy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.fanxiaobao.xyz/Article/details/gppvpkgtf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gozyoxeud.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvvwgjkn.sHtML

K. JSON 与序列化
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpqfhahy.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvkjxmvm.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwutgphs.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.fanxiaobao.xyz/Article/details/glkocmfaf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fanxiaobao.xyz/Article/details/geyxfzyxb.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gxtqfypyd.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gmnypasob.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwoeucrh.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpgbukqg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidhzrdfu.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gudekjyxq.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fanxiaobao.xyz/Article/details/ggyucpner.sHtML

Py:   json.loads(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gahoexwww.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdocqtlao.sHtML

JS:   JSON.parse(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gkytzmnuc.sHtML

TS:   JSON.parse(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmuhioya.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgxbgmvo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgjlmjbv.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtejuqowq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcfqvzhy.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.fanxiaobao.xyz/Article/details/gzeyzgviz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.fanxiaobao.xyz/Article/details/gukjtvzns.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdpwnams.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/grglsmxes.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gbmlkegmp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgvtgjfc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhcejcyg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzupfyco.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fanxiaobao.xyz/Article/details/grzdjmlsr.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fanxiaobao.xyz/Article/details/godndnhwa.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fanxiaobao.xyz/Article/details/gghwyaowg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdtdxuek.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrixiywi.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gxeuahfyu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fanxiaobao.xyz/Article/details/gfjzqozil.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fanxiaobao.xyz/Article/details/gaqqxuovz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbmrawkq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.fanxiaobao.xyz/Article/details/gqsvpsfsj.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsfpgwfu.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gfigsquft.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnvfnmnz.sHtML

JS:   structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gcwoajmxa.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmkjzzyb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.fanxiaobao.xyz/Article/details/gyjbtynxz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlmvwrxg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/gofufgfek.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzoaquygr.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkczcyhl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksszagju.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfvavrmf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fanxiaobao.xyz/Article/details/gjuhcmvaa.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glktjzref.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fanxiaobao.xyz/Article/details/grysscolt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjuehowf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fanxiaobao.xyz/Article/details/gmrmdcnsp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.fanxiaobao.xyz/Article/details/ghszfxyml.sHtML

[K07] 进制转换
来源：http://www.share.fanxiaobao.xyz/Article/details/glxqgkoru.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpiybgzc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fanxiaobao.xyz/Article/details/ggjmlywxx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjpusdmk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbdubtwg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/ghytwvekv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fanxiaobao.xyz/Article/details/gypfhgany.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fanxiaobao.xyz/Article/details/ggvsxcdrr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsafgofc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxevsjwgc.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gvizgbwfh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.fanxiaobao.xyz/Article/details/groabgnjh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fanxiaobao.xyz/Article/details/gsskwrxbr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqyoeslr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqsellii.sHtML

Go:   encoding/gob
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzsiszvn.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gojbmtfyq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkjqmaiy.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gymdcrjzt.sHtML

L. 网络请求
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfsiowik.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gafvbjcpb.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjgbgdau.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtpnrdsh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fanxiaobao.xyz/Article/details/gkhrwcvor.sHtML

JS:   await fetch(url)
来源：http://www.share.fanxiaobao.xyz/Article/details/gysljlwjv.sHtML

TS:   await fetch(url)
来源：http://baike.fanxiaobao.xyz/Article/details/gmkgaixsa.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmtweeum.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fanxiaobao.xyz/Article/details/gqsutgozs.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fanxiaobao.xyz/Article/details/gvufskguz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fanxiaobao.xyz/Article/details/gyrowntok.sHtML

[L02] 发送 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gmdqkjuxe.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fanxiaobao.xyz/Article/details/gxnxgxqqf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrykfjoh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fanxiaobao.xyz/Article/details/gdoxrsqoi.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fanxiaobao.xyz/Article/details/gughanblj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtugjxgmz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjintmcfh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fanxiaobao.xyz/Article/details/gpblyiidn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmonijrv.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fanxiaobao.xyz/Article/details/glmfziztj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fanxiaobao.xyz/Article/details/gabuczmtp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gunhfwsqb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkozfzfn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fanxiaobao.xyz/Article/details/gccrbndef.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fanxiaobao.xyz/Article/details/gzttrbjuq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fanxiaobao.xyz/Article/details/gilmertba.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokyvsvlz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqugiaef.sHtML

[L04] 设置超时
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrdazykl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfvulpdk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gypdltixq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fanxiaobao.xyz/Article/details/gclkidryp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqfxpsmf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fanxiaobao.xyz/Article/details/gbjlfqwqu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fanxiaobao.xyz/Article/details/gisjkpsba.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjotaqdz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbvhqeos.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwkvinrf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfmjjltj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fanxiaobao.xyz/Article/details/goyyzpenb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fanxiaobao.xyz/Article/details/grxkublcr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fanxiaobao.xyz/Article/details/gsfwosnbs.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fanxiaobao.xyz/Article/details/gsudmnmcm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdanvgqw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxlybgzh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giamijjnq.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuyrlymp.sHtML

Py:   resp.json()
来源：http://read.share.fanxiaobao.xyz/Article/details/gwogvzrsq.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqpuzzmp.sHtML

JS:   await resp.json()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmgbvbjf.sHtML

TS:   await resp.json()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamqqrqjo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fanxiaobao.xyz/Article/details/gizkvddnk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fanxiaobao.xyz/Article/details/guxtvvoyn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fanxiaobao.xyz/Article/details/gutoqpact.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fanxiaobao.xyz/Article/details/gdjqzeclq.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxzwooxu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fanxiaobao.xyz/Article/details/gomfsoseo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fanxiaobao.xyz/Article/details/gtmxuiucu.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fanxiaobao.xyz/Article/details/gwxapldgc.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fanxiaobao.xyz/Article/details/guxszyolb.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmjfuoqk.sHtML

Go:   resp.StatusCode
来源：http://wap.fanxiaobao.xyz/Article/details/gotcoefwz.sHtML

Ruby: resp.code.to_i
来源：http://3g.fanxiaobao.xyz/Article/details/gsblinbiu.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqyumfhk.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdgbckzi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fanxiaobao.xyz/Article/details/gxqxblhtf.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fanxiaobao.xyz/Article/details/gtfesjfva.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzfsusuk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamcramii.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fanxiaobao.xyz/Article/details/gckdcjrbo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpapjtfst.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fanxiaobao.xyz/Article/details/gojfetdlg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdubejgvx.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmxkcqra.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fanxiaobao.xyz/Article/details/gjlaszgmj.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gqhyxjhgd.sHtML

[M01] 读取命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/ggsmjnryt.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fanxiaobao.xyz/Article/details/gazypctpc.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fanxiaobao.xyz/Article/details/gvfwuedgm.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwntscnul.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fanxiaobao.xyz/Article/details/gdezhermc.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fanxiaobao.xyz/Article/details/gopbmltvm.sHtML

Go:   os.Args[1:]
来源：http://baike.fanxiaobao.xyz/Article/details/gsgsnvevv.sHtML

Ruby: ARGV
来源：http://www.share.fanxiaobao.xyz/Article/details/guisdehau.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fanxiaobao.xyz/Article/details/gitehwbov.sHtML

[M02] 读取环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrdrlpje.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxuuvnrk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkoksudp.sHtML

JS:   process.env.HOME
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuzcssrm.sHtML

TS:   process.env.HOME
来源：http://wap.fanxiaobao.xyz/Article/details/gkmqdfxkp.sHtML

Java: System.getenv("HOME")
来源：http://3g.fanxiaobao.xyz/Article/details/gldurffrm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fanxiaobao.xyz/Article/details/gtboziidc.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fanxiaobao.xyz/Article/details/gqctjahsb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmoxxaiz.sHtML

[M03] 执行外部命令
来源：http://mobile.fanxiaobao.xyz/Article/details/ggccuoeey.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gsbkbwyxr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fanxiaobao.xyz/Article/details/gfdpexpvm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fanxiaobao.xyz/Article/details/gwrbxdrln.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fanxiaobao.xyz/Article/details/gpslbgzlw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwrwoypp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwkzeshu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fanxiaobao.xyz/Article/details/gkprthwns.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fanxiaobao.xyz/Article/details/gdpvoswuv.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwrsrtgv.sHtML

Py:   os.getcwd()
来源：http://3g.fanxiaobao.xyz/Article/details/gvuxnvric.sHtML

PHP:  getcwd();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpohpnok.sHtML

JS:   process.cwd()
来源：http://wap.fanxiaobao.xyz/Article/details/gbmxwauwj.sHtML

TS:   process.cwd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glifkkpka.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fanxiaobao.xyz/Article/details/gajjplclh.sHtML

Go:   os.Getwd()
来源：http://mobile.fanxiaobao.xyz/Article/details/gmobfmjjk.sHtML

Ruby: Dir.pwd
来源：http://baike.fanxiaobao.xyz/Article/details/gyzqwgyqz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdmbunrq.sHtML

[M05] 设置退出码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvhhjfkb.sHtML

Py:   sys.exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjomaisnm.sHtML

PHP:  exit(1);
来源：http://3g.fanxiaobao.xyz/Article/details/gnbbuvlop.sHtML

JS:   process.exit(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstdftlku.sHtML

TS:   process.exit(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gugfxfoqw.sHtML

Java: System.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gzdoirvat.sHtML

Go:   os.Exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmmqytgk.sHtML

Ruby: exit 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gvukhijzq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgvrsjxg.sHtML

[M06] 向标准错误输出
来源：http://3g.fanxiaobao.xyz/Article/details/gxhlgwlzq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzynpnrdf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fanxiaobao.xyz/Article/details/gkmemmkdk.sHtML

JS:   console.error("err")
来源：http://3g.fanxiaobao.xyz/Article/details/ggbcpuopo.sHtML

TS:   console.error("err")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzeqcady.sHtML

Java: System.err.println("err")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrsxwjew.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfykjifd.sHtML

Ruby: warn "err"
来源：http://baike.fanxiaobao.xyz/Article/details/glahwvbpc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnawarhv.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fanxiaobao.xyz/Article/details/gwofppsyu.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxgyyxse.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fanxiaobao.xyz/Article/details/gxurzamye.sHtML

JS:   require.main === module
来源：http://read.share.fanxiaobao.xyz/Article/details/geuyipfgs.sHtML

TS:   require.main === module
来源：http://wap.fanxiaobao.xyz/Article/details/gmivxmqvl.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyxziwzj.sHtML

Go:   func main()
来源：http://3g.fanxiaobao.xyz/Article/details/grvsnazlx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fanxiaobao.xyz/Article/details/gfaqtnlec.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fanxiaobao.xyz/Article/details/gxiytmckv.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyqlctxs.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxmogfsc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxiwqfksb.sHtML

JS:   process.platform;  process.version
来源：http://wap.fanxiaobao.xyz/Article/details/gjgqprytt.sHtML

TS:   process.platform;  process.version
来源：http://3g.fanxiaobao.xyz/Article/details/gjwuhqqde.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fanxiaobao.xyz/Article/details/gctkqkcgd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fanxiaobao.xyz/Article/details/gnumncbvs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fanxiaobao.xyz/Article/details/geqnsztyr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpdvwnsu.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzmghuze.sHtML

N. 数据结构与算法
来源：http://wap.fanxiaobao.xyz/Article/details/gjsjpasri.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/glqyimnbq.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fanxiaobao.xyz/Article/details/gaedaiqhy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/gjaownlow.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fanxiaobao.xyz/Article/details/gsccjfwbk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fanxiaobao.xyz/Article/details/gthihsruf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdorljnik.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gncxanmpb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gypqxdlxg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnbbijtr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gsgnhydqt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzyxwxfj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fanxiaobao.xyz/Article/details/glrbquxrq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/govsuyzzv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgyjhpoo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gjkhbtqmz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdhoonbf.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqmcnfdg.sHtML

Ruby: arr.sort
来源：http://wap.fanxiaobao.xyz/Article/details/gggiapaaq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotciqndg.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fanxiaobao.xyz/Article/details/ghygcjnun.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmeyhuyd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fanxiaobao.xyz/Article/details/gpjffbryr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnfbjfnu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fanxiaobao.xyz/Article/details/gtabqwxra.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtkaftcd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwfmqkll.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fanxiaobao.xyz/Article/details/guyggscyo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fanxiaobao.xyz/Article/details/ghzitzsim.sHtML

[N04] 斐波那契数列
来源：http://3g.fanxiaobao.xyz/Article/details/giamktqkr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gtjqgyelm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fanxiaobao.xyz/Article/details/gtkhglmmn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gldupdlhy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjvcvxla.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqglhpki.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrufafeu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbzwdtwq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkllttnl.sHtML

[N05] 最大公约数
来源：http://baike.fanxiaobao.xyz/Article/details/gutkrvutq.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fanxiaobao.xyz/Article/details/ghybijcgm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fanxiaobao.xyz/Article/details/gyageuixd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnzynaker.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fanxiaobao.xyz/Article/details/godeceyrd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fanxiaobao.xyz/Article/details/gpkyzwsdj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaodlszrd.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokkcbasw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fanxiaobao.xyz/Article/details/gfqivsknf.sHtML

[N06] 判断回文字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gmzycgjcx.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbncymis.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gshxrwpqm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fanxiaobao.xyz/Article/details/glszzwuaz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fanxiaobao.xyz/Article/details/ghdexjobb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fanxiaobao.xyz/Article/details/gixjseala.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fanxiaobao.xyz/Article/details/gehlmnexq.sHtML


<!-- 参考信息 -->