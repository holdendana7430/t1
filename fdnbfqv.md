代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkgxaxxo.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.fanxiaobao.xyz/Article/details/gezbsrwvy.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkuymrcr.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.fanxiaobao.xyz/Article/details/gpfaepzzt.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.fanxiaobao.xyz/Article/details/gnezobieq.sHtML

[J08] 提取年月日与星期
来源：http://blog.fanxiaobao.xyz/Article/details/gxrlsyvtv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtseagrhj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxfiibds.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fanxiaobao.xyz/Article/details/gnoibzhro.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.fanxiaobao.xyz/Article/details/glkqszsnf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyzvqhut.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.fanxiaobao.xyz/Article/details/grhvlezap.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.fanxiaobao.xyz/Article/details/gmebhhtpz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggokyqyfa.sHtML

[J09] 时区处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnlfgmgo.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfprixave.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geynchpzj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fanxiaobao.xyz/Article/details/gmljreyur.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fanxiaobao.xyz/Article/details/giwtossxu.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.fanxiaobao.xyz/Article/details/grhfheijx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbfxdwwv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgyoknkv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.fanxiaobao.xyz/Article/details/gkezboznn.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwshupde.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fanxiaobao.xyz/Article/details/gwnqdetgw.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fanxiaobao.xyz/Article/details/gyiuplzom.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gycqgmwfg.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxtfnepe.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzeztvckp.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkygdlst.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.fanxiaobao.xyz/Article/details/glqjzhyij.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsuyyvxb.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzaynlvli.sHtML

K. JSON 与序列化
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbmksagm.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gytbysoao.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gwqhsoped.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fanxiaobao.xyz/Article/details/gmkowhhou.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgrbksve.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsktgwxt.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/ghbckkbld.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuikljkh.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelcsqjpa.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjbhveuw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkmncsjr.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gdevqhpca.sHtML

Py:   json.loads(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gmkvpnees.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fanxiaobao.xyz/Article/details/gsowvhrln.sHtML

JS:   JSON.parse(s)
来源：http://wap.fanxiaobao.xyz/Article/details/giegkzgow.sHtML

TS:   JSON.parse(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gicofvjom.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fanxiaobao.xyz/Article/details/gtnadenbo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlqdcrui.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwdsonyd.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuuylojz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fanxiaobao.xyz/Article/details/glkjuxoqy.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrkspdgm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtwhbpql.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcratslov.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gomaoggqt.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/ghbykhkga.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.fanxiaobao.xyz/Article/details/gqazgsqbt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/grqsbznqm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fanxiaobao.xyz/Article/details/gmugyyfjc.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcojfwgrc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gdblccjlz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fanxiaobao.xyz/Article/details/gimtaefan.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fanxiaobao.xyz/Article/details/gypmjcddw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsujpsosi.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gordaapfb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgusekhm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fanxiaobao.xyz/Article/details/ggaqpvqwu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkbkmumx.sHtML

[K05] 深拷贝对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gghqiwnrp.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyhwyvkv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fanxiaobao.xyz/Article/details/gbeqyysjc.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwutcysa.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcondvnqu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fanxiaobao.xyz/Article/details/gcmpfpnxk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fanxiaobao.xyz/Article/details/gnseqtsif.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzerkncs.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.fanxiaobao.xyz/Article/details/glcvvapti.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.fanxiaobao.xyz/Article/details/grsnupjzx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fanxiaobao.xyz/Article/details/gfftoqymw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvslbgwx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fanxiaobao.xyz/Article/details/gttfmkblq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsixkpznw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihiaietz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnexcugdu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbiroxazo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.fanxiaobao.xyz/Article/details/gujiddhrz.sHtML

[K07] 进制转换
来源：http://3g.fanxiaobao.xyz/Article/details/gwokhgull.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gongfmggl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwphpjskf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgmzmybr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhzefuyf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/grerraxec.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fanxiaobao.xyz/Article/details/gdbkmaaft.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqjugave.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrfbuobm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fanxiaobao.xyz/Article/details/glnqgupuq.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gesboubcn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/guhrgtyjd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fanxiaobao.xyz/Article/details/gjrtnsrkm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fanxiaobao.xyz/Article/details/gguyheqgs.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fanxiaobao.xyz/Article/details/grntcjgot.sHtML

Go:   encoding/gob
来源：http://wap.fanxiaobao.xyz/Article/details/gsftdwcrl.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gsnkouczi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlhlzagd.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gmjskjesc.sHtML

L. 网络请求
来源：http://blog.fanxiaobao.xyz/Article/details/gvwpilvdt.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxfhgrrl.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfptrjggy.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxefoyeim.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fanxiaobao.xyz/Article/details/gecuxsgnp.sHtML

JS:   await fetch(url)
来源：http://baike.fanxiaobao.xyz/Article/details/gefglsdeo.sHtML

TS:   await fetch(url)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrdivpsc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fanxiaobao.xyz/Article/details/gbpgktlvq.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxonfwkn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbqwjrks.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fanxiaobao.xyz/Article/details/gljbjfkzk.sHtML

[L02] 发送 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gftmfbudc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fanxiaobao.xyz/Article/details/gchojifib.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyhbqekq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbolugzy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gjndkakrc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fanxiaobao.xyz/Article/details/gyumafkgm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdsiqlvg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfrdzcxl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fanxiaobao.xyz/Article/details/gbnieqvqt.sHtML

[L03] 设置自定义请求头
来源：http://wap.fanxiaobao.xyz/Article/details/ginifogoy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvailmlg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gynoprhxn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fanxiaobao.xyz/Article/details/gtskqyzbu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fanxiaobao.xyz/Article/details/gikvuciko.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fanxiaobao.xyz/Article/details/gytyuxakj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fanxiaobao.xyz/Article/details/gmiguxlya.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fanxiaobao.xyz/Article/details/gdnhtftap.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpfieadu.sHtML

[L04] 设置超时
来源：http://blog.fanxiaobao.xyz/Article/details/gekygrwuh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fanxiaobao.xyz/Article/details/gywvlrokg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjjtjang.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrorjzbg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbtpmhbq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fanxiaobao.xyz/Article/details/gzpjwtoga.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fanxiaobao.xyz/Article/details/gepiwtqjo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fanxiaobao.xyz/Article/details/gaqkfclol.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gdeigbscp.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fanxiaobao.xyz/Article/details/gxmpohgog.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fanxiaobao.xyz/Article/details/gunmdopzp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfwjinse.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxlkovsh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fanxiaobao.xyz/Article/details/gvwzmgqem.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fanxiaobao.xyz/Article/details/gggjeofkm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewtzutoi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fanxiaobao.xyz/Article/details/gyngchyth.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjivngfpu.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavdfjcye.sHtML

Py:   resp.json()
来源：http://mobile.fanxiaobao.xyz/Article/details/gthuvnxjm.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gammlbizo.sHtML

JS:   await resp.json()
来源：http://m.share.fanxiaobao.xyz/Article/details/groqiiipv.sHtML

TS:   await resp.json()
来源：http://wap.fanxiaobao.xyz/Article/details/gjnzcqtar.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fanxiaobao.xyz/Article/details/gtuldqlxs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grymtmbyh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzdieaig.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fanxiaobao.xyz/Article/details/gunzytenw.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gmpeoksab.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtcrwzfa.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fanxiaobao.xyz/Article/details/gedctaapu.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fanxiaobao.xyz/Article/details/geynhaquh.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fanxiaobao.xyz/Article/details/gmltkvouz.sHtML

Java: resp.statusCode()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcjdpzps.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjabcixjc.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxjxqrlx.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyktlefnm.sHtML

[L08] 并发请求多个地址
来源：http://blog.fanxiaobao.xyz/Article/details/glusggzuz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fanxiaobao.xyz/Article/details/glfgopcvf.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glksijphh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gaynfjuqt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gjipnfslo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.fanxiaobao.xyz/Article/details/gntxeidwl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fanxiaobao.xyz/Article/details/glnvcfcrc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzxaxngd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjuqmagh.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/givnkpmrp.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fanxiaobao.xyz/Article/details/gnazhxlat.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqiafnjb.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyoqpwgv.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdufupjsg.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsshjwplx.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fanxiaobao.xyz/Article/details/gvntrjmfm.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gioxooowj.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxrjrcly.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/greiuxqzx.sHtML

Ruby: ARGV
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpowedqt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkoqdlrj.sHtML

[M02] 读取环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvlfrsdy.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtmwoilc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtrfaxxs.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugpzqnfp.sHtML

TS:   process.env.HOME
来源：http://wap.fanxiaobao.xyz/Article/details/gbuoygecv.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fanxiaobao.xyz/Article/details/gudpuujil.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnexudan.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjimeyuuz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxofdixs.sHtML

[M03] 执行外部命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gewgddvbj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlxrpqsc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fanxiaobao.xyz/Article/details/goukukfza.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fanxiaobao.xyz/Article/details/gdbhixvuk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fanxiaobao.xyz/Article/details/gerbimgqh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fanxiaobao.xyz/Article/details/gurbqykgr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fanxiaobao.xyz/Article/details/gtejlvplw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqcslcba.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fanxiaobao.xyz/Article/details/ganazerau.sHtML

[M04] 获取当前工作目录
来源：http://wap.fanxiaobao.xyz/Article/details/gawkoxqat.sHtML

Py:   os.getcwd()
来源：http://wap.fanxiaobao.xyz/Article/details/gtgpsfnnt.sHtML

PHP:  getcwd();
来源：http://baike.fanxiaobao.xyz/Article/details/gztapqncf.sHtML

JS:   process.cwd()
来源：http://www.share.fanxiaobao.xyz/Article/details/gphhsgzys.sHtML

TS:   process.cwd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpgqcjhs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqfigukl.sHtML

Go:   os.Getwd()
来源：http://3g.fanxiaobao.xyz/Article/details/gscbkbssw.sHtML

Ruby: Dir.pwd
来源：http://wap.fanxiaobao.xyz/Article/details/gpsdmyfxb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvoenhgai.sHtML

[M05] 设置退出码
来源：http://wap.fanxiaobao.xyz/Article/details/gprggqstp.sHtML

Py:   sys.exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gekrkmjwh.sHtML

PHP:  exit(1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvotpozcs.sHtML

JS:   process.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gjqlqodyr.sHtML

TS:   process.exit(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbmyfbgz.sHtML

Java: System.exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gxtomgiau.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngpptdbt.sHtML

Ruby: exit 1
来源：http://baike.fanxiaobao.xyz/Article/details/gpqhxahza.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fanxiaobao.xyz/Article/details/gltoqbxet.sHtML

[M06] 向标准错误输出
来源：http://wap.fanxiaobao.xyz/Article/details/giufkohcz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggiopsmzw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbynrblf.sHtML

JS:   console.error("err")
来源：http://read.share.fanxiaobao.xyz/Article/details/glmjsbcvp.sHtML

TS:   console.error("err")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbddsfzam.sHtML

Java: System.err.println("err")
来源：http://read.share.fanxiaobao.xyz/Article/details/gowbrivee.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fanxiaobao.xyz/Article/details/gqayvmdfs.sHtML

Ruby: warn "err"
来源：http://blog.fanxiaobao.xyz/Article/details/ghhhbkuez.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fanxiaobao.xyz/Article/details/gxrsdmkbz.sHtML

[M07] 判断是否为主入口
来源：http://blog.fanxiaobao.xyz/Article/details/gmzyenjio.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fanxiaobao.xyz/Article/details/gtknzaozo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhdjoxpe.sHtML

JS:   require.main === module
来源：http://baike.fanxiaobao.xyz/Article/details/gonuwuhti.sHtML

TS:   require.main === module
来源：http://baike.fanxiaobao.xyz/Article/details/giktflhsu.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnmmohgq.sHtML

Go:   func main()
来源：http://wap.fanxiaobao.xyz/Article/details/gdtdaysug.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fanxiaobao.xyz/Article/details/gciakmbqp.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fanxiaobao.xyz/Article/details/gkmzvgfhv.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fanxiaobao.xyz/Article/details/gzsyvbhfq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyozikpg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fanxiaobao.xyz/Article/details/gqznsvrpk.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fanxiaobao.xyz/Article/details/gynjxodnj.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fanxiaobao.xyz/Article/details/gennqoyil.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawffwchj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fanxiaobao.xyz/Article/details/gaymhzmmw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fanxiaobao.xyz/Article/details/gepnvaohg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fanxiaobao.xyz/Article/details/gnwvzymeg.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ggwizyelc.sHtML

N. 数据结构与算法
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfrfuwbn.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gwxeobzis.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fanxiaobao.xyz/Article/details/gkuwqiuut.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfxqnjvx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyoxseko.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwowrviax.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fanxiaobao.xyz/Article/details/greepdywz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gnzjwvyhz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/goahxuzym.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fanxiaobao.xyz/Article/details/gqmbcchnp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaomzfipz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fanxiaobao.xyz/Article/details/gipggfjky.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fanxiaobao.xyz/Article/details/gxiqidpbh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gvwepqmep.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gsyyballm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/guchyielj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsayclmhf.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gcnmfztpd.sHtML

Ruby: arr.sort
来源：http://wap.fanxiaobao.xyz/Article/details/gwtwuaskf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fanxiaobao.xyz/Article/details/gklsdfvxl.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fanxiaobao.xyz/Article/details/gbswkztpk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fanxiaobao.xyz/Article/details/gopjucmon.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexoddwjr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fanxiaobao.xyz/Article/details/gfhhpotno.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fanxiaobao.xyz/Article/details/girkkefic.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fanxiaobao.xyz/Article/details/gvahcdeqk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fanxiaobao.xyz/Article/details/gtkbmoizp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptponnwb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqqcyxvv.sHtML

[N04] 斐波那契数列
来源：http://mobile.fanxiaobao.xyz/Article/details/ginacjxxo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gsmsrlvuo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqkyuhto.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsxqfuhp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpahjqats.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrhypxaz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzyfdlug.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpuulbxw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvymhfbvb.sHtML

[N05] 最大公约数
来源：http://3g.fanxiaobao.xyz/Article/details/glkoovreg.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fanxiaobao.xyz/Article/details/gkgqdleis.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fanxiaobao.xyz/Article/details/gezebkccb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gybdmznxs.sHtML


<!-- 参考信息 -->