代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gtsopwqzp.sHtML

[J08] 提取年月日与星期
来源：http://wap.hesvh.cn/Article/details/gluljnvvs.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fehbvm.com/Article/details/gatjxztnc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.zdbjq.cn/Article/details/gzglztkpq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.fehbvm.com/Article/details/gemxsvnsk.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.zdbjq.cn/Article/details/gqamnfexb.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.hesvh.cn/Article/details/glctwznne.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.fehbvm.com/Article/details/gllsviunt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.hesvh.cn/Article/details/gaebqosyu.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.fehbvm.com/Article/details/grvqimmsr.sHtML

[J09] 时区处理
来源：http://3g.hesvh.cn/Article/details/gewyirjnb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fehbvm.com/Article/details/gojvjwmls.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fehbvm.com/Article/details/geafnrwtm.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fehbvm.com/Article/details/gcvhaeyqz.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gsrkpdgyy.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.hesvh.cn/Article/details/gcnbayizy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.zdbjq.cn/Article/details/gifcyosbv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.zdbjq.cn/Article/details/gfkdpiipu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.fehbvm.com/Article/details/gkogbokdc.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.fehbvm.com/Article/details/gmeehovmf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.zdbjq.cn/Article/details/gnatmrcps.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fehbvm.com/Article/details/glfqpfmee.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fehbvm.com/Article/details/glgyyjwbi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.zdbjq.cn/Article/details/gnkwdnalh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fehbvm.com/Article/details/gwpnyhrrp.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.zdbjq.cn/Article/details/gpploordb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.zdbjq.cn/Article/details/gyuwwozhu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fehbvm.com/Article/details/gcdpmlsct.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gldfszmnq.sHtML

K. JSON 与序列化
来源：http://mobile.hesvh.cn/Article/details/gjcniycei.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gohnsioyi.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.zdbjq.cn/Article/details/gaaysszpt.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/gimmhnubt.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/gykcdktgd.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/glksapwbd.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gswgbvtnn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.hesvh.cn/Article/details/gltvuiyqn.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fehbvm.com/Article/details/ggdmcrozk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.hesvh.cn/Article/details/gbprjvcwc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.hesvh.cn/Article/details/gjxtomhru.sHtML

[K02] JSON 字符串转对象
来源：http://blog.fehbvm.com/Article/details/gkocnapop.sHtML

Py:   json.loads(s)
来源：http://m.share.fehbvm.com/Article/details/gvvopzlvn.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.hesvh.cn/Article/details/gtjlqepqs.sHtML

JS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gwvxmegdf.sHtML

TS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gbbofveds.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.fehbvm.com/Article/details/gddlxeeqo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/girdukeip.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gruzlwruq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.zdbjq.cn/Article/details/gqgriqgiz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.zdbjq.cn/Article/details/gxhhkayea.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/gtsecljca.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gnvfxipzu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/gcioohqpi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gihtcvoya.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.zdbjq.cn/Article/details/gvlvicxod.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fehbvm.com/Article/details/gkcvhggbn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fehbvm.com/Article/details/gjgpgwyjt.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.hesvh.cn/Article/details/getfqlqax.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.zdbjq.cn/Article/details/gjfpzzcwx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.zdbjq.cn/Article/details/gcttfjojk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.zdbjq.cn/Article/details/gxbddzhyt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gefvlyssv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/gulhjujay.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fehbvm.com/Article/details/ggmonzngq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.hesvh.cn/Article/details/gzpxiuvty.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.hesvh.cn/Article/details/gosgujhct.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fehbvm.com/Article/details/grsyqqoby.sHtML

[K05] 深拷贝对象
来源：http://mobile.zdbjq.cn/Article/details/gdqqdjxnl.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.zdbjq.cn/Article/details/gccfvpcbd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fehbvm.com/Article/details/gknnhoyeq.sHtML

JS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/ggfmlohbs.sHtML

TS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/grjsfvavo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fehbvm.com/Article/details/gbdvtwxim.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.hesvh.cn/Article/details/gbfdbotmh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.hesvh.cn/Article/details/ghpcybydp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.fehbvm.com/Article/details/gryhniadk.sHtML

[K06] 解析 URL 查询串
来源：http://blog.zdbjq.cn/Article/details/gzxsjvcbt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/glgfjbewp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fehbvm.com/Article/details/glktqdujq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gndtbfexf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/gjzjstklz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.zdbjq.cn/Article/details/gzztkbrsv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gccomdfid.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/grgzxilqr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gnhgvjcuc.sHtML

[K07] 进制转换
来源：http://blog.hesvh.cn/Article/details/gjoduumwe.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gjxbyqdjz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.hesvh.cn/Article/details/gvahnjrqs.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gixrenelm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gchdebswx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/ggkjjqbdh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fehbvm.com/Article/details/ghuoessmc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/garoigqcs.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gzjlpehmd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.hesvh.cn/Article/details/gmgexyzmi.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fehbvm.com/Article/details/gmloaxvgt.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.zdbjq.cn/Article/details/gaduxzyus.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gjgoazbon.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/ggriylhci.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.zdbjq.cn/Article/details/gtxmzoltc.sHtML

Go:   encoding/gob
来源：http://www.share.fehbvm.com/Article/details/gykspezlm.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.zdbjq.cn/Article/details/gyslcsaer.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gdqambvbn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gakuoqhqf.sHtML

L. 网络请求
来源：http://www.m.share.zdbjq.cn/Article/details/gehrttkpl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gundrnerz.sHtML

[L01] 发送 GET 请求
来源：http://m.share.hesvh.cn/Article/details/gejddpywt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.zdbjq.cn/Article/details/gceibcobt.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/ghuhlkjuz.sHtML

JS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gzexdokif.sHtML

TS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gpxlydgks.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/gmfjzuywv.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/gukarmncd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fehbvm.com/Article/details/gautigybz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fehbvm.com/Article/details/gqrcjhwch.sHtML

[L02] 发送 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gepeepeoz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fehbvm.com/Article/details/grxymwbbe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.hesvh.cn/Article/details/gurmuobwj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gskolswgt.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gzwgvarom.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.hesvh.cn/Article/details/ggyxddjcm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/gwpabepvo.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fehbvm.com/Article/details/gakpkrpcr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.hesvh.cn/Article/details/gtjwquvcm.sHtML

[L03] 设置自定义请求头
来源：http://3g.fehbvm.com/Article/details/gddfldzvn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.zdbjq.cn/Article/details/gzeadradd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.hesvh.cn/Article/details/gvgolilxq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/ghmozajdk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gqjaqehyh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.zdbjq.cn/Article/details/gvsiohkjc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gejtvwexi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.zdbjq.cn/Article/details/gmgcciiir.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/guewpxydw.sHtML

[L04] 设置超时
来源：http://www.blog.zdbjq.cn/Article/details/gmwiwowhv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/gglcbfnog.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gmaynivzc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gnflvujzs.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gjfgruoud.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fehbvm.com/Article/details/gitecjijf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/guqauboyu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/gvrmlsqul.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.hesvh.cn/Article/details/gkcbsmvhz.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/ghhxvdrbi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.hesvh.cn/Article/details/gcgbanzyf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/giylshrtv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/glgwiomcw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gjoxxepqm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.zdbjq.cn/Article/details/gflqvocjh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/gdiilsxpo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/geownzxzc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gofqcgtgy.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/gzaeefure.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gpyrajoep.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/givqpmkmc.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gimtbsrir.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/ggdjbbigg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/grxondcrz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/gtgqhgzhv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fehbvm.com/Article/details/ghtapwqha.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gjysqbopa.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gwshpeamf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/gcqgyykco.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.zdbjq.cn/Article/details/gjawzsjhr.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gnoctkqea.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gviejzwdt.sHtML

Java: resp.statusCode()
来源：http://www.blog.fehbvm.com/Article/details/gkkyserlb.sHtML

Go:   resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gnndlbvza.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/gjcuyffcu.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/glytmkuvj.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gsikyqmdh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gheknaudh.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.hesvh.cn/Article/details/gimsfztkt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gktdavclr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/glhbpdylo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/gepqtwalz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.zdbjq.cn/Article/details/godiswmlk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gpyyfnduo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.hesvh.cn/Article/details/gebrijcnr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzdmsvnop.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.hesvh.cn/Article/details/gnezitmif.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcvxajivr.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gnmzniyfd.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/ghrvsrugb.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/goxfsuorc.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/glddbmwba.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gilzvdwsl.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gycwmdued.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/gvtaiyslx.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/guwbmddvv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gfmphftrm.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/givfhabif.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gavyizbie.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gdvmfasug.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gyvwiezqu.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/ggbeflgyf.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/gwgtaykhq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/gixgibioh.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/gytlullfh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/gbufyepub.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/ghphsuuqm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/grndipkes.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gqpdiitmu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gefakaoyu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/ghsflxmwa.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gpcrqzrmj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fehbvm.com/Article/details/ghjhkovdm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/gfeieflob.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/gjhsilsqx.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/gcxvgxsfd.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gnifpkvmq.sHtML

PHP:  getcwd();
来源：http://m.share.fehbvm.com/Article/details/gkftzihjg.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gkvwhnsev.sHtML

TS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gmsvodoce.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/ghwluxnzw.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/gjqqkperh.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/goeudwuge.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/glsqrvupj.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gwlmnjank.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/guvrlaqsf.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gzoprbtmx.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gdxlvxdkg.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gxskeaaqa.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gfievryrc.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gtpajmnir.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gqlpxhoux.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gwvpcajpf.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gfnvbzrag.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gbhfcwxjd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gyiatwkqv.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gsoflsvfm.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gwsljqsqx.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gbszkoyug.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/gllnnlwzp.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gclfmzuvt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/gfjccsfgq.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gmwegdgjh.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/gitlxvhur.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/gnatjspya.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gukolfnei.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/glxffmpyz.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gvdssracs.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gmfjfauue.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/gtyxtrabs.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gjyrnicmc.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/gesvhtjud.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gvkyfwxsq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gqrfldpnk.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gnofspoac.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gpdpplfok.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/gfosmevsq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/gjhdlokvh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gsofikbzc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gkfgqghre.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyofcpvjj.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/gbqxavmkw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxukxaorz.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/gxgbyuslk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/giuhuwmsr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gfjvjhzxj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gwnwsnitv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gocfbdhjm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gksshttrp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gleyylybd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gkzafkgpx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gvnytfwdq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gcgxpydgd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/glocvmrrw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/ghtyqzhsd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gdvpeytqc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/glnnulamh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gyeenaotz.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gnzglnvwk.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gigkisncv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gktsbjaxz.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/gxbaajoch.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gccjnaoqa.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/gjmrwbbbq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gbybcjwpw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gtbpjcvxt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gynbxglwt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gqutgnkwh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gkszkljfo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gwwnjjwss.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/gqxrdhohi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gpekhemjm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gnkkfywtd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gjhmwsfrn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/ggnhbndeo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/gthctmzit.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/gbrqlhxgg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gvpfbvfem.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gmkdpvucg.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gxfboyeqx.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gcjslveky.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gaolcrvpt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/ggicrikhy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gfizcmgxj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gjtnyuitp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/gdncilnez.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/grpzljmyq.sHtML


<!-- 参考信息 -->