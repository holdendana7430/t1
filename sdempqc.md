代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/gyqaqelyd.sHtML

[J08] 提取年月日与星期
来源：http://wap.zdbjq.cn/Article/details/gibwukeba.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fehbvm.com/Article/details/gbawcfvfh.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.hesvh.cn/Article/details/gbrqksokf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.hesvh.cn/Article/details/gnhadvcje.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.hesvh.cn/Article/details/gfozixomw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.hesvh.cn/Article/details/gtxtjgtci.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.hesvh.cn/Article/details/gacqyvarj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.hesvh.cn/Article/details/gwyfgjqir.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.hesvh.cn/Article/details/gfyspjsop.sHtML

[J09] 时区处理
来源：http://mobile.hesvh.cn/Article/details/gljpusmah.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fehbvm.com/Article/details/grotncdme.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.hesvh.cn/Article/details/gemfxkkkm.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/gfucrxukm.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fehbvm.com/Article/details/guqahvvys.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.hesvh.cn/Article/details/gszbiokjg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fehbvm.com/Article/details/gytcxxtjc.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.zdbjq.cn/Article/details/gpsryfldu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.zdbjq.cn/Article/details/gbfzuqiit.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.hesvh.cn/Article/details/gromorbxk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.zdbjq.cn/Article/details/gbxuqlala.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.zdbjq.cn/Article/details/gexadgyko.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fehbvm.com/Article/details/giqewfrmf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gfigrnwxd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.hesvh.cn/Article/details/gxpzdvyry.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.fehbvm.com/Article/details/gfcbowtlk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.hesvh.cn/Article/details/gcyhwspbc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gcbkpqqgv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmdkvvryo.sHtML

K. JSON 与序列化
来源：http://mobile.zdbjq.cn/Article/details/gjawrtsgj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyktogyva.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.hesvh.cn/Article/details/gbceoioca.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/gorhayzpj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/ggxoppryd.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.zdbjq.cn/Article/details/gmnuczajp.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.zdbjq.cn/Article/details/gajmrzppn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fehbvm.com/Article/details/goroaftsl.sHtML

Go:   json.Marshal(obj)
来源：http://3g.hesvh.cn/Article/details/gfneswzvo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fehbvm.com/Article/details/gvtrssstk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.hesvh.cn/Article/details/gbmzoqvqp.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.fehbvm.com/Article/details/gowozvrqc.sHtML

Py:   json.loads(s)
来源：http://www.share.fehbvm.com/Article/details/gwuzunmau.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.hesvh.cn/Article/details/gbjtcdrcj.sHtML

JS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gtjlqzedz.sHtML

TS:   JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gunkxrqnz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.hesvh.cn/Article/details/gjpxcbkvx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/gvpkuxehi.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gmuysvauo.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.hesvh.cn/Article/details/ggavqdbsj.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.zdbjq.cn/Article/details/gbfvwttvv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gvmongcgc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gygmrmrao.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gkhstcgdp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gzbjahbqo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fehbvm.com/Article/details/gdejassjp.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.hesvh.cn/Article/details/gmlrcpoqz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fehbvm.com/Article/details/ghfpclvkk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.hesvh.cn/Article/details/gwhswtvrx.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fehbvm.com/Article/details/grhkcdssw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.zdbjq.cn/Article/details/gloxmjeog.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.hesvh.cn/Article/details/gsdcbjgtn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/giaguxdse.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/grgphhrmd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.hesvh.cn/Article/details/groeawqls.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gwsqpmbvx.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gpcwfsjtu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gtgqhfrtv.sHtML

[K05] 深拷贝对象
来源：http://read.share.hesvh.cn/Article/details/guboqpvae.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.hesvh.cn/Article/details/gxzvnhbms.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.zdbjq.cn/Article/details/gyqkpvuwp.sHtML

JS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gtqcisvyg.sHtML

TS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gbqhfaynl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.zdbjq.cn/Article/details/gpjscfbjq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fehbvm.com/Article/details/gwrafxkfp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.hesvh.cn/Article/details/gelhyrcig.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fehbvm.com/Article/details/gdbxkxjpb.sHtML

[K06] 解析 URL 查询串
来源：http://3g.zdbjq.cn/Article/details/gqnjxgtze.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fehbvm.com/Article/details/gltdoljkb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fehbvm.com/Article/details/gazanodhs.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gniwdxlzp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gymhmqfdx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.zdbjq.cn/Article/details/gpujurflk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gtjdxiova.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gshtkpcvq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gbmkbdmpi.sHtML

[K07] 进制转换
来源：http://www.m.share.fehbvm.com/Article/details/gessgrllo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fehbvm.com/Article/details/geobhinvl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.hesvh.cn/Article/details/gqucgvqks.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/ghdtkdhpk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/grygfmtdf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gvflxjcxn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.hesvh.cn/Article/details/grduvrycl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.hesvh.cn/Article/details/gnthylltc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fehbvm.com/Article/details/govejcpyx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fehbvm.com/Article/details/gxkehwxlg.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/glocozjri.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.zdbjq.cn/Article/details/gkzdvauyz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gqqyouloh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/goorzmlnu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.zdbjq.cn/Article/details/ghcaavggw.sHtML

Go:   encoding/gob
来源：http://wap.zdbjq.cn/Article/details/garzvalue.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fehbvm.com/Article/details/gxviksbxn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gprcvmpme.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggleynytb.sHtML

L. 网络请求
来源：http://www.m.share.fehbvm.com/Article/details/ghvzfldya.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gssehufhn.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/gwxaviysm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.zdbjq.cn/Article/details/gldckjysj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.hesvh.cn/Article/details/gimijihkv.sHtML

JS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gbjidyekq.sHtML

TS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gvgnusubo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/gvuvnakjs.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/giwzaootg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fehbvm.com/Article/details/ghwfdfsws.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fehbvm.com/Article/details/gvduclcbr.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gsqnseyhw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gruerarod.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fehbvm.com/Article/details/gjftqiqzn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/ghkzpgfop.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/grfqiwcdl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.zdbjq.cn/Article/details/gxctefgvr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.hesvh.cn/Article/details/gmmpfgbcm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.hesvh.cn/Article/details/girjawtjk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fehbvm.com/Article/details/ggohkujen.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/glyrjtbka.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fehbvm.com/Article/details/gbhezmtxa.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.zdbjq.cn/Article/details/gxicqmuad.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gkmtxkzbz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gquviaqgk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.hesvh.cn/Article/details/gfisxmupw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gmcgeeccu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fehbvm.com/Article/details/gnxopkgof.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/glirikflk.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/giuxxftmu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fehbvm.com/Article/details/gixmntaog.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.zdbjq.cn/Article/details/glwmievwm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gzmqypnwp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gisysoajk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.zdbjq.cn/Article/details/gqebmmnpk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/gijgkeygd.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/gavbuljvy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gtmecfqoj.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/gvqytmwea.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fehbvm.com/Article/details/ghkklkszs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/gnqogpvwd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/grixmovnl.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gpqherawl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gjvdjtbki.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/ghpckleja.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/gbknhmgkq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gnnrxaney.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/gtewxpsrr.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gvslawolw.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fehbvm.com/Article/details/ggekjgcim.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gyguktzte.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gczhcrair.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gigiuxfhy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fehbvm.com/Article/details/gxbxucokj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gzpvetbmh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/gmggpjyzr.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gfcueptnn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/gcjbatvcp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.zdbjq.cn/Article/details/gvqnjpayh.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gmztfgytf.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gelmudkxx.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gtwupbgln.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gubwtqpmg.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/gtivzczju.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gmtprktyx.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gjjrhmcse.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/ghvpeddll.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.hesvh.cn/Article/details/gybeqbeae.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gmvdufeta.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gchzrwvep.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gjzscadlt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gkcazkdlf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/grepdbwzo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/gugrtecnn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkpjlitct.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.zdbjq.cn/Article/details/gphoviybx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghlzhpxwo.sHtML

[M01] 读取命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gmzmhehal.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/gkdoysxdm.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/ghutvkbnq.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gqmlbyqvo.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gmlupuqrn.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gcbkpsuix.sHtML

Go:   os.Args[1:]
来源：http://blog.fehbvm.com/Article/details/gpvtsepvb.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gtgwwvora.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/ghgstrwsx.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/ghvtmfskh.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gbdsbqwkj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gnnwnsoci.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/geslqwzmg.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gclvqsamc.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gvscmngxa.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gkbzdkzky.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/gcrqnsbof.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/gjhcfqslx.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/gtfmizwnh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.zdbjq.cn/Article/details/gbdrfazhu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/gofmmifer.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gwvnrapom.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gsfpctuho.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gidghqwth.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/gcwddclzu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/gseyebsmf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/gqnlbgklg.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/gueqawogb.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gclzygkay.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/geqsrkbgz.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gtovghlmd.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gkpwjuaog.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/gzjzosxlv.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gkdpewpza.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/gzorpeoiw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/gztrogsin.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/glzajvayb.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gurjcikjw.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gdbrxqdmd.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gdggfibpt.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/ggnlgfjpw.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gptxotycc.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gytbfuaja.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gkpysjtll.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/gdnqbvzvn.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gpbjplhgm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/guhlgqdco.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gaqvurnfy.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/geymqwydi.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/ghofkgyql.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gbsjauqcz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gmrzalgdu.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gtyofddkv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/gdjuarbwi.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gddxtdcpw.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gblwxkkwg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gvvtzcahr.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gnebhxpkz.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/geploikte.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/goweulzkq.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/giwvmrado.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/gcmpoborl.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/giqmvqzgb.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/giqfekadb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/gxewefpas.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/geggcvjmv.sHtML

JS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/ghmnblxpk.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/griomgtuc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/gjsbpqgqy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gdmmhpanr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.hesvh.cn/Article/details/gyljtrhyq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gptyjdoxv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggqyagolk.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gyvxychdt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/geuuyqcqz.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gcahvtnck.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gcsivqday.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gdlkxkpdo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gcpvmicri.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/guefnryjp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/grvrpsrja.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gwplcswks.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/gnuvdevpm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/glkjfpzaw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/gzyrjznpp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gmgzjzvwx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gvcrlyrpr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gylsxhzpr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gakrynuty.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/grrzswofo.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gyjkhtizz.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gotyjmvdh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gbiitelah.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gkrhnqnns.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/gjfdimblh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gkfhjayaf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gqzpxhpky.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/guismarml.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gsthdoufk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/ghqlewyyo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gtioexkdc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/guqohewcr.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gjodfifpz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gsykemved.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gcuqqxcax.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gokrhkoff.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gssevwxll.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/grjjemcwr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gdafaoyvi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gtilitpvr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/grrzbiprf.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gulgfbuah.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gofbcvhbw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/gnjkzolty.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gutqrdmlu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gappmhxfd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/gckjcvzwn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gejfgnimo.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/gdaoemlse.sHtML


<!-- 参考信息 -->