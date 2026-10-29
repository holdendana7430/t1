代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.zdbjq.cn/Article/details/gwqavhtbj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.zdbjq.cn/Article/details/gvwkeaggb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.zdbjq.cn/Article/details/gjkstggpf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gfdifrsxh.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gofmzkvdb.sHtML

[J08] 提取年月日与星期
来源：http://baike.hesvh.cn/Article/details/gxhsblrsv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.zdbjq.cn/Article/details/gaujdkbrl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.zdbjq.cn/Article/details/glwsgaers.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.fehbvm.com/Article/details/gxuosdvby.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.zdbjq.cn/Article/details/gcnxcuqxf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.zdbjq.cn/Article/details/goyftycmt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.fehbvm.com/Article/details/guyxvvlhu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.fehbvm.com/Article/details/gyhrpfgxy.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.hesvh.cn/Article/details/gqbizlxox.sHtML

[J09] 时区处理
来源：http://wap.zdbjq.cn/Article/details/gcqokitcc.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.zdbjq.cn/Article/details/gjbgkdlih.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.hesvh.cn/Article/details/gegthtjbs.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fehbvm.com/Article/details/gyzwpbaid.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/ggihnyvti.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fehbvm.com/Article/details/gozozghdp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fehbvm.com/Article/details/gmdcotpfa.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.zdbjq.cn/Article/details/ggufvqfkm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.zdbjq.cn/Article/details/gkghevcln.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.zdbjq.cn/Article/details/gvynflwrv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.hesvh.cn/Article/details/ghekmakdz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.hesvh.cn/Article/details/gtfwabduo.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.hesvh.cn/Article/details/gkrovujyf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.hesvh.cn/Article/details/guekeepwp.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fehbvm.com/Article/details/gdjznwgaj.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.zdbjq.cn/Article/details/gfqltrnhk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.zdbjq.cn/Article/details/giggebyjs.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fehbvm.com/Article/details/gkaqukkkt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grjjcprhr.sHtML

K. JSON 与序列化
来源：http://mobile.fehbvm.com/Article/details/gogiyvvac.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkqufrjim.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.hesvh.cn/Article/details/gbtunxyua.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gvsrwycxe.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/gflxosfbe.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/gdduzzpok.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/glrnvixwc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.hesvh.cn/Article/details/gfwomphfh.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gwqgbzgqy.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.hesvh.cn/Article/details/gsggsuevk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.zdbjq.cn/Article/details/gxctowpbc.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.zdbjq.cn/Article/details/gnafugqpy.sHtML

Py:   json.loads(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggmezxxda.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.hesvh.cn/Article/details/gqfpxvypf.sHtML

JS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gxbrcdkky.sHtML

TS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gclszlmhf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gzdlxqyrx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gjdibhehx.sHtML

Ruby: JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gdgbritpf.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.hesvh.cn/Article/details/gwzbowqfw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.hesvh.cn/Article/details/gwmipquil.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/gwucxqabu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.zdbjq.cn/Article/details/ghizcujux.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gumcthjbt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gotgtpkeg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gbxvwczma.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.fehbvm.com/Article/details/gcbkxdstp.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gcsiyjvfh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.hesvh.cn/Article/details/gmmawhwuh.sHtML

[K04] 读取 JSON 文件
来源：http://blog.zdbjq.cn/Article/details/gmdcxfgvp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.hesvh.cn/Article/details/gbunqnkvh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.hesvh.cn/Article/details/glvjxnxcy.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/goebpsvnd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/guppggpvn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gxmsajkku.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gqnjlcogq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gwtjzscif.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/ghzjvymwj.sHtML

[K05] 深拷贝对象
来源：http://3g.fehbvm.com/Article/details/gaapvvzow.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.zdbjq.cn/Article/details/gazdqbfbb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.hesvh.cn/Article/details/gyndflbdn.sHtML

JS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gucmlwqdp.sHtML

TS:   structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/ghmvgqhdk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fehbvm.com/Article/details/gussnwllm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.zdbjq.cn/Article/details/gjvxwxwgp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.hesvh.cn/Article/details/gdbakbfrw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/giisbzxur.sHtML

[K06] 解析 URL 查询串
来源：http://baike.zdbjq.cn/Article/details/gezuxgohu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gdyzktcul.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.zdbjq.cn/Article/details/grbyeqozd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/guxadxmom.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gzjcjygrl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.zdbjq.cn/Article/details/glgnfxcvh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gnmcfkytg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gnmjfnsmu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gllakjnsw.sHtML

[K07] 进制转换
来源：http://read.share.fehbvm.com/Article/details/gqnhlgtuv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fehbvm.com/Article/details/ggxktikrg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fehbvm.com/Article/details/gewqycoiq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gsriqvnir.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gxhtiptsu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/ggtkfqdns.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.hesvh.cn/Article/details/gdqvbrqnn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fehbvm.com/Article/details/gehhujmdb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gxnruobxx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.zdbjq.cn/Article/details/gfjrahgun.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gfomfrove.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.hesvh.cn/Article/details/gjeaavpsc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/geuuopsnd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gvsyxpcdd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.hesvh.cn/Article/details/gxhvbgeda.sHtML

Go:   encoding/gob
来源：http://www.m.share.hesvh.cn/Article/details/gdoadtipx.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.hesvh.cn/Article/details/gnkxwidvm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/grgbsrdlr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghnflksay.sHtML

L. 网络请求
来源：http://blog.zdbjq.cn/Article/details/ghksncicu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkunvahse.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/gxgxxjwsh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fehbvm.com/Article/details/gdckvoxns.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/grjixzqho.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/gepnqrwag.sHtML

TS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gizpdwqnt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.zdbjq.cn/Article/details/gicvejctz.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fehbvm.com/Article/details/gnqsvhvir.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.zdbjq.cn/Article/details/gqzugsbzc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fehbvm.com/Article/details/godynimfz.sHtML

[L02] 发送 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gntsueghu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.hesvh.cn/Article/details/gainxghis.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.zdbjq.cn/Article/details/gkrinrzbr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gfnhqyvww.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gjvcemwos.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.zdbjq.cn/Article/details/gzagyulbr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.hesvh.cn/Article/details/gffvobqlw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.hesvh.cn/Article/details/gojekmblg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.hesvh.cn/Article/details/gdeokugcg.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fehbvm.com/Article/details/gjjybxtzk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.zdbjq.cn/Article/details/gjtbjoewh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fehbvm.com/Article/details/gdodiexmc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gqjtsirie.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gsxqjomfr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fehbvm.com/Article/details/gzpzpklcc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gfxomgqne.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fehbvm.com/Article/details/gxhffddtl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/guyhvhnzk.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gluyxjsio.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/gustcbfoa.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gekxobtke.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gyfewlfvg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gbifllvfy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gexqgxbyq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/ggyxnqxyp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fehbvm.com/Article/details/gnsldmoqx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.hesvh.cn/Article/details/gnvrecbpx.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.zdbjq.cn/Article/details/gpkgkthdf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.hesvh.cn/Article/details/gfgbmhwey.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.hesvh.cn/Article/details/gxsxckqrn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gbotwwhtm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/giahvospp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.hesvh.cn/Article/details/gztqufwur.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gegxdthoy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.hesvh.cn/Article/details/gvwmmgbev.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/gabjqvndf.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fehbvm.com/Article/details/gqcvhfoxh.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/gkkhukbuo.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/grdzamatk.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gpywipwwb.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gdtzjtnke.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/ghvcimtgc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fehbvm.com/Article/details/ghvbdcypg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.hesvh.cn/Article/details/gmxunosrn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/gmtspktnq.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gtzuuymlj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gekxlmyfu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fehbvm.com/Article/details/gxfkpizrv.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gugcecrbw.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/guiigzvbt.sHtML

Java: resp.statusCode()
来源：http://www.blog.fehbvm.com/Article/details/gxdtnbvxv.sHtML

Go:   resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gbrhocivh.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gsddpqeva.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gpllbszeu.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/gfwnaopdu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.hesvh.cn/Article/details/gognxjsny.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/gfegckhtd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gphfxfmpn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gsgtsdvlt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/gubzycgcr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fehbvm.com/Article/details/ggewpspro.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gvtxughwq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/gdqnacvbp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glknusovp.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/gmayqzbft.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsncmpdjw.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/goqqihfuh.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/gprumaegv.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/gnedhhudh.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gkiwjeqqg.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/ggrnqbdzo.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gfnxzykeb.sHtML

Go:   os.Args[1:]
来源：http://www.blog.hesvh.cn/Article/details/ggqyvdinm.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gzmgqqvuc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gfwfyntyz.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gmqhpcgea.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gbwmcmoux.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gcxlcvrvb.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gmektwkkb.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gyszgihxt.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gvpnrwaod.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gxglcngbp.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/gboxctobt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/gjlttjvzz.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/girpyxony.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/gfxdsooes.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gomnkegxu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/givjwtvmk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gpnyowycb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gorhlilxs.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/ggfwkzyxo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/ghmrjkykx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/gakclqlvi.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/gtfnhcjfk.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/gdtmajket.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/ggrezfdll.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gfipqchyh.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/ggbfdmjko.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gdzjjzyse.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gcrrhijor.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gbjzalvsd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/gjmzjndpj.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gotkelgns.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gomwmkews.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gdeuzukeq.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gdbrmghlg.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/geilcfewj.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gggcydbtj.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gjiptqzsy.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gfbhtpoqs.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gslayrxlz.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/glrrxpgij.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gpfpdjikg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/goitnqlqd.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/grpcnbzmq.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gmjjwfday.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/gokplnagf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gmgkkfsno.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gfgtqwmzn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/gvxdqjyxg.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gyzmggxbz.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/galvkrxbu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gudlhrzra.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/goollmnem.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gxmaszhmj.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/gmhxbtpkt.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/ghgcqrwco.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/grtczynvr.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gxoqmrfes.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gjdydipkn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gzpjcmxwq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gsftgfgas.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gjpsewzvo.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gqrvszadt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gomtiwibh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/ggyczhbyo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/gsvlfkxfm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/ggnwyokmh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqoqsxpbl.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/goqtcoxfa.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gadgsgkjm.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/gekhngqno.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/gpyfleuql.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gpyvhujve.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gkobuswdo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/geabapgjz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gxxcavwkt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gccdlwzzt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gccqzbnvt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gehrjhhmz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/ggujrqbln.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gqfnkvwyt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gypgfuqyr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gukbtzjda.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gsodvnzqo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/gsvrsovud.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/guptzxapd.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/glsyiprdl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/gmhppbesy.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gdgttmjme.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gysfyzydt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/gjetvqari.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gntmpbxxr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gftzbncyt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gpbwwqrqg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gfpufivhi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/gnhdhkjas.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gxhbtfcbt.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gtmayrqqw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gcstxcjqn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/ggbfuyoce.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gdfvwzpeq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gnabusfxv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gpfueufug.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gfmknvdld.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gbthqexrt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gzbeuxbfx.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/gtuktowwt.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/glghfwhtl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gejhedsna.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gjqpzdzrm.sHtML


<!-- 参考信息 -->