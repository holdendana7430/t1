代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.fehbvm.com/Article/details/graxvcqbc.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.zdbjq.cn/Article/details/giiwlpzkc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.zdbjq.cn/Article/details/gtxmiwphv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gvalkkjdk.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/gtrvccydg.sHtML

[J08] 提取年月日与星期
来源：http://read.share.zdbjq.cn/Article/details/gwebjzvgu.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.zdbjq.cn/Article/details/gjoromyjs.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.zdbjq.cn/Article/details/ghdkdgfnd.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.fehbvm.com/Article/details/gbyequufu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fehbvm.com/Article/details/ggtapbpnh.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.fehbvm.com/Article/details/gwqxhphhm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.zdbjq.cn/Article/details/gdreypcgl.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.fehbvm.com/Article/details/gfyoffdwq.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fehbvm.com/Article/details/gumckqzlz.sHtML

[J09] 时区处理
来源：http://read.share.zdbjq.cn/Article/details/ggfszizbq.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.zdbjq.cn/Article/details/gvwjvvdcn.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.fehbvm.com/Article/details/gynedxnwj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.hesvh.cn/Article/details/gnqqelfcc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/gswfqmiig.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.hesvh.cn/Article/details/gahzfumnb.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.hesvh.cn/Article/details/gjodkmhaw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.fehbvm.com/Article/details/gmtpbehkp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.hesvh.cn/Article/details/gplxewtic.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.zdbjq.cn/Article/details/gjmqfwrcj.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmkyciztv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.hesvh.cn/Article/details/gkolidsan.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.zdbjq.cn/Article/details/gbbdhburt.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.hesvh.cn/Article/details/gunnwgldr.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.hesvh.cn/Article/details/grgorsblt.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.hesvh.cn/Article/details/gzxadtixa.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.fehbvm.com/Article/details/gziuseqcx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.zdbjq.cn/Article/details/galaxevzr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxyrfzznl.sHtML

K. JSON 与序列化
来源：http://3g.fehbvm.com/Article/details/gxcnvbvjz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gigubqwqh.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.zdbjq.cn/Article/details/gizmmvpnb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/glwzgwiej.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/gjpnscebj.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.zdbjq.cn/Article/details/gemalonzv.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/ggjhdokzb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.hesvh.cn/Article/details/glorujrov.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fehbvm.com/Article/details/gndhimauu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.hesvh.cn/Article/details/gipugriwa.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.zdbjq.cn/Article/details/grvenahdp.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.zdbjq.cn/Article/details/gjpoqabkq.sHtML

Py:   json.loads(s)
来源：http://wap.hesvh.cn/Article/details/gsrlzfhvi.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.zdbjq.cn/Article/details/gwddefkbj.sHtML

JS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/grmlhdxwt.sHtML

TS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gomdkqqrd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.zdbjq.cn/Article/details/giscqaaqd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gsfrzupeh.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gnirqogol.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.hesvh.cn/Article/details/gwfzjwzgh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.zdbjq.cn/Article/details/gqqzadcjw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/gyycnvzom.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/gbubiefhf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gmetsgyxx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/gnqkfnyix.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.hesvh.cn/Article/details/gjliflqup.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.zdbjq.cn/Article/details/gcbzfwwsu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fehbvm.com/Article/details/gxlabsqkj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.hesvh.cn/Article/details/gxlxzcoch.sHtML

[K04] 读取 JSON 文件
来源：http://3g.zdbjq.cn/Article/details/gmyipconf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.hesvh.cn/Article/details/gjodujsru.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.hesvh.cn/Article/details/gzpjxixqi.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/gqwadlwtw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/ghuekcvfm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gpxlelflf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gxavulzco.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gromhqxic.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.hesvh.cn/Article/details/gpvheuarb.sHtML

[K05] 深拷贝对象
来源：http://www.share.hesvh.cn/Article/details/gonpzrcdn.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fehbvm.com/Article/details/gmwfydphw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fehbvm.com/Article/details/grebrlvnv.sHtML

JS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gsqemnjxq.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gffomopcl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.zdbjq.cn/Article/details/gblvsizii.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.zdbjq.cn/Article/details/gxnsscmxv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fehbvm.com/Article/details/gltfqlmzn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fehbvm.com/Article/details/ggjhlmzqc.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.zdbjq.cn/Article/details/gkkukeqea.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gewlimpor.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fehbvm.com/Article/details/gjmspxiik.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/gqzkygwhy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gssmszxag.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gkmheqxnu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gyfapmsou.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gpjuwznvy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gpikiazmn.sHtML

[K07] 进制转换
来源：http://mobile.fehbvm.com/Article/details/gfzowkecq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/ghckoiisi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.hesvh.cn/Article/details/gnuehutaa.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gjltyscbo.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/giesvhqyn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gadshgdbr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/gxfmqiifr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.zdbjq.cn/Article/details/gpyshpgtc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fehbvm.com/Article/details/ggqdlrvsi.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/gmpyadvkq.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.fehbvm.com/Article/details/gsplyllcj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.zdbjq.cn/Article/details/gwupdnwwy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gkzutbuvw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gljovlbmd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.zdbjq.cn/Article/details/gbxlhrphs.sHtML

Go:   encoding/gob
来源：http://baike.zdbjq.cn/Article/details/gquzbfuuc.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fehbvm.com/Article/details/gogiddbtx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gmslokfbu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gaybfsbcn.sHtML

L. 网络请求
来源：http://mobile.fehbvm.com/Article/details/gbtkedpry.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggknsgzay.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fehbvm.com/Article/details/gqoyociki.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.hesvh.cn/Article/details/guwzsdesc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fehbvm.com/Article/details/gqqiocvga.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gnnamiebj.sHtML

TS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gshlbouab.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fehbvm.com/Article/details/gxmozzyga.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fehbvm.com/Article/details/geilxkjin.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.zdbjq.cn/Article/details/gysnkoxtq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/gpgtxkarw.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gahqfjazd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gaarlvxnl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.hesvh.cn/Article/details/gqxuebcyv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gokrlsruf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gqlxlibhj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gypohotkp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fehbvm.com/Article/details/gauohckxp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fehbvm.com/Article/details/gobmoiyvz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/gryhdvhbd.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/gokvojhzg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fehbvm.com/Article/details/gkxzarurj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.hesvh.cn/Article/details/guqshllyn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gicuwpbxi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gyrefbdam.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/grxkldwxe.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gucufksbi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/gzoanfynz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gycmwqqul.sHtML

[L04] 设置超时
来源：http://mobile.fehbvm.com/Article/details/grpnfdlhm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.hesvh.cn/Article/details/gokaplqfa.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.zdbjq.cn/Article/details/gmgkgdfgh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gggcnsavr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gbaqjodhm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.zdbjq.cn/Article/details/gucimliqg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fehbvm.com/Article/details/guzhctosn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.zdbjq.cn/Article/details/gauxzjypf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gbfdqhmvp.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/garlcwneu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/gsgwfjtjq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/ghctjtssu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gthkfqgcd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gnwmqqlyu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.zdbjq.cn/Article/details/grwptzvng.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fehbvm.com/Article/details/gedxxtqlc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gmaposdcs.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.zdbjq.cn/Article/details/gclbxbiay.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gipvlxrww.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gvquctpcv.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/gioqbfwuh.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gnklmrnsu.sHtML

TS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/ghekfhzep.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gakkmchun.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/glgwshipz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.zdbjq.cn/Article/details/gajnnxwlc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gltbnvoon.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gwhjywsnl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gtszfczic.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gbbflnamx.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gsqodknex.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gttpdudwj.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/gytmvnjzw.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gasbyunmi.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/grspzanig.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gngrawpqr.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gsjrigloe.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/ghxfnkjhd.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/gaqvvgztb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gxiwentyl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gndxgkajf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/givniqsel.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.hesvh.cn/Article/details/gffixnxku.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gqyxqgkjp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/grkddituy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcuktnlll.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/gogpumhsz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtsulemgs.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/glkglpgog.sHtML

Py:   sys.argv[1:]
来源：http://wap.fehbvm.com/Article/details/ggucjmqde.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/gsxjuovft.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gufruyxvw.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/giismoqoe.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gvxvlaihs.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gfqztluth.sHtML

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/goeluxniy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gewwiawtu.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gfczflqpl.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gvqfdvrdy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/ghoekynst.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gbcixmfvv.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gmggjllpq.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gywmrpxck.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gjcicipvz.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gttiycnld.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gomlobbsa.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gfndobmnw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/gfrnfgqxp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/ggznhfgjo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gzujtvfcx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gcuvgyejc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gduzyyjhw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/gpgasyiyc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gzfpfvflr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/giklvtsqd.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gofzjmjfi.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/ghlmqsytb.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gqooouzzs.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gstdlliaw.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gllhfpdba.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/ghnbsfspl.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/gucbsidgo.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/guwgraqox.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gyrsfical.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/grzscdroj.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/gmrlynbrg.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/gxfzdoibi.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gnvccisrh.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gqnfbtbfl.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gsqnnjejo.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gnepmurzt.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/ggimsjwhs.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/gklegnupt.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/grftukniw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gcqioilct.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gyuflkcxy.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/galfletuv.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gpatfvklh.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/gxuaiesmv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gpxyviube.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gickjksix.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/ggmbnruzi.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gnoktuxup.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gowgxwikc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gwdwtdicx.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/glegtoxns.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gdlmzckyg.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gujfbuudq.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gtycjixru.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/guvtjlgfx.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/gdvhfwakk.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/gaqsailmk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/giwcztjjg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gjhaukpqy.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/grtvzilgj.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/grkhznkoc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gayuzkrbu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gbfpqbdkn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gfedhhsqq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gopnvipzf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbmgqtktw.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/gaqecwmhl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gydbtuoum.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gbkciaqal.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gqmrerkth.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gmfflfjex.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gqhqqqgfq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gbbxvszsc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gucitrcol.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gdoqmcetg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/gwdmcbdnc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gnnubldkp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gblhugiig.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gxulqanhr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gjimqtrko.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gopxzowtr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gcsqdjdor.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/goatqqbpl.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gyuobzjyr.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gyjmzsfrj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gfnpagsml.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/giuavphln.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gnivbxbdm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gpkzamrfc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gpneyaazr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gvcalldsr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/ggqgddnwh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gvpxnxwks.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gkiahxura.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/giiououol.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/gcarkqtij.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gzyakfpgu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gvnbpenxo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gdvifzkgh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gntejkbcd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gegsfhrzq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gafwsyhjc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gebfoqgxi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gdxydoxai.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/grlbdkyce.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/graqxhtmr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.hesvh.cn/Article/details/gzrfngnyk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/giizsudmk.sHtML


<!-- 参考信息 -->