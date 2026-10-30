代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcashnoc.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.fanxiaobao.xyz/Article/details/gjuinbuow.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gegdtnphw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.fanxiaobao.xyz/Article/details/gynhdcemw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkagxutd.sHtML

[J08] 提取年月日与星期
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmcbbljd.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.fanxiaobao.xyz/Article/details/ghvdibfmn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.fanxiaobao.xyz/Article/details/giwwimyau.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.fanxiaobao.xyz/Article/details/gukxbojgt.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.fanxiaobao.xyz/Article/details/gdqclwqxm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.fanxiaobao.xyz/Article/details/gumxyiegy.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.fanxiaobao.xyz/Article/details/ggunlvbpd.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.fanxiaobao.xyz/Article/details/gooqaqthd.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fanxiaobao.xyz/Article/details/ghselrmte.sHtML

[J09] 时区处理
来源：http://m.share.fanxiaobao.xyz/Article/details/giempylvn.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.fanxiaobao.xyz/Article/details/gccudmtpj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.fanxiaobao.xyz/Article/details/gqezlyfsw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fanxiaobao.xyz/Article/details/gejvbtiyt.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fanxiaobao.xyz/Article/details/gyfttmckp.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrpyidrd.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fanxiaobao.xyz/Article/details/glwukeure.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fanxiaobao.xyz/Article/details/gonwxlhvq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkncqqbyu.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.fanxiaobao.xyz/Article/details/gvapvieyl.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fanxiaobao.xyz/Article/details/gjzysysfc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrhztrxl.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaocguhtl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gguipcrug.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gujyknknu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fanxiaobao.xyz/Article/details/gvwphrdmb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.fanxiaobao.xyz/Article/details/gvdxrnhul.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gviabrull.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxosdzlw.sHtML

K. JSON 与序列化
来源：http://blog.fanxiaobao.xyz/Article/details/gwlfaksud.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmyumunq.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gfranspog.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fanxiaobao.xyz/Article/details/guexeexnz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fanxiaobao.xyz/Article/details/grubemnot.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauhnctno.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gkxykbaqx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fanxiaobao.xyz/Article/details/gizlxitwe.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gpfkfdgxp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fanxiaobao.xyz/Article/details/gpojvueke.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/grolwtage.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fanxiaobao.xyz/Article/details/gjisglisn.sHtML

Py:   json.loads(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gtxcpbjol.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmmaxiyj.sHtML

JS:   JSON.parse(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/giyshqamh.sHtML

TS:   JSON.parse(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdllgsgvk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtikbyfs.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fanxiaobao.xyz/Article/details/gczoxckbc.sHtML

Ruby: JSON.parse(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gmbdbswpg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuvwtqpo.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fanxiaobao.xyz/Article/details/gikhbbomr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxwzljdq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmhjlpxq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gfgrwnyvq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/griqqgiro.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvjdqbhw.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.fanxiaobao.xyz/Article/details/gtlwjticf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskrrpfny.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.fanxiaobao.xyz/Article/details/gicgctacb.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqprbdru.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfiubhxi.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyveveqk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gptlqqndb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gupfyemqr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbvzucms.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrkpopob.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fanxiaobao.xyz/Article/details/glxgoyswc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fanxiaobao.xyz/Article/details/gfjstmdyr.sHtML

[K05] 深拷贝对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbsrazxc.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbbltqmv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbgesqcq.sHtML

JS:   structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gyczmrbbj.sHtML

TS:   structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcebutpq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.fanxiaobao.xyz/Article/details/gwpallwvm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.fanxiaobao.xyz/Article/details/gsycsfxyu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnblhvqpk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbgxjmcn.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fanxiaobao.xyz/Article/details/gndgmawjd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.fanxiaobao.xyz/Article/details/gxrrjvvin.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fanxiaobao.xyz/Article/details/gitkloubj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwhxwppz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fanxiaobao.xyz/Article/details/gjtifyfbp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fanxiaobao.xyz/Article/details/grawizszd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztjbbxvy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.fanxiaobao.xyz/Article/details/gzblutdel.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrxqfnxp.sHtML

[K07] 进制转换
来源：http://3g.fanxiaobao.xyz/Article/details/gjlsrfmxo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrvjcaus.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fanxiaobao.xyz/Article/details/ghesqsgec.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.fanxiaobao.xyz/Article/details/gorymxmzw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/grrfjbvmw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gdftnryty.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fanxiaobao.xyz/Article/details/gfuciqvsu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhheqlkd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhovjjnl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmiqlqpp.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxzuxvmd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouyinevr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fanxiaobao.xyz/Article/details/gqidvabqs.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fanxiaobao.xyz/Article/details/gzprfsgkq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyplglyk.sHtML

Go:   encoding/gob
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrtjlfzn.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gjlcnjcqq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fanxiaobao.xyz/Article/details/gefebudmc.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gjaencicm.sHtML

L. 网络请求
来源：http://read.share.fanxiaobao.xyz/Article/details/giezcrjrk.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagkhdqcc.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsksxdqk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fanxiaobao.xyz/Article/details/gzzyuecre.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fanxiaobao.xyz/Article/details/gvdqttgdn.sHtML

JS:   await fetch(url)
来源：http://blog.fanxiaobao.xyz/Article/details/gfubwcatd.sHtML

TS:   await fetch(url)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgxpdtwf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fanxiaobao.xyz/Article/details/gvykxngyy.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fanxiaobao.xyz/Article/details/goniimxne.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fanxiaobao.xyz/Article/details/gjvoknxwb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fanxiaobao.xyz/Article/details/geoscbduj.sHtML

[L02] 发送 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gktiyofzq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgteklzr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnhqczzc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihzecphf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fanxiaobao.xyz/Article/details/gpctwotxo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fanxiaobao.xyz/Article/details/gmaaoufot.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fanxiaobao.xyz/Article/details/gempeogau.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fanxiaobao.xyz/Article/details/gatqvwbxi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fanxiaobao.xyz/Article/details/gpdyaadjf.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmvhlfaf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fanxiaobao.xyz/Article/details/geyxrfstn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyotvkns.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxwgkrio.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fanxiaobao.xyz/Article/details/grppcbrnp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fanxiaobao.xyz/Article/details/gruptmoeq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstpihldz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fanxiaobao.xyz/Article/details/gzwuqpbjv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fanxiaobao.xyz/Article/details/ggwzwdtuf.sHtML

[L04] 设置超时
来源：http://3g.fanxiaobao.xyz/Article/details/gjjkhagdv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fanxiaobao.xyz/Article/details/gvhyunnmx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokfaqtyq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fanxiaobao.xyz/Article/details/gfdtzfxqd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fanxiaobao.xyz/Article/details/gdnumnlne.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fanxiaobao.xyz/Article/details/gqidwjlrw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fanxiaobao.xyz/Article/details/gijrgtqqn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fanxiaobao.xyz/Article/details/gdqnhumua.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhsdwdhj.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fanxiaobao.xyz/Article/details/gymeppftn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fanxiaobao.xyz/Article/details/gplizuvnn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fanxiaobao.xyz/Article/details/gdazagogd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzehmkpd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzanhxkjd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzhcaphw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fanxiaobao.xyz/Article/details/goyaupmxa.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfycccfv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gwztpqiqw.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gsoalsclv.sHtML

Py:   resp.json()
来源：http://read.share.fanxiaobao.xyz/Article/details/gogrgwrmh.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/glluexaok.sHtML

JS:   await resp.json()
来源：http://baike.fanxiaobao.xyz/Article/details/gbyablsix.sHtML

TS:   await resp.json()
来源：http://3g.fanxiaobao.xyz/Article/details/gjtwvclek.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fanxiaobao.xyz/Article/details/gyiaipyyf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fanxiaobao.xyz/Article/details/gzbcmcjdq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fanxiaobao.xyz/Article/details/gndsorrwp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fanxiaobao.xyz/Article/details/geqtmkvja.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbormitcj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fanxiaobao.xyz/Article/details/gzblyxcut.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoqcmqav.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fanxiaobao.xyz/Article/details/grqjsbzwt.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaaihsug.sHtML

Java: resp.statusCode()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxpnlofe.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclvrntwe.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrwomzxe.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchnfxfxf.sHtML

[L08] 并发请求多个地址
来源：http://3g.fanxiaobao.xyz/Article/details/ggfgwvttw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fanxiaobao.xyz/Article/details/grseargsq.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fanxiaobao.xyz/Article/details/gjgmaisgu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gwnlzjbdf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkwleqvu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fanxiaobao.xyz/Article/details/gszepiscd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fanxiaobao.xyz/Article/details/gfaoyixfl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fanxiaobao.xyz/Article/details/garngcujh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpvlvpwb.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebbysmyz.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geelkwttg.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gtscuzfkx.sHtML

[M01] 读取命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmodfiie.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrgxuljb.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykpgxazm.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmojzckpk.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqrmyuwt.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrmszczb.sHtML

Go:   os.Args[1:]
来源：http://3g.fanxiaobao.xyz/Article/details/gvsbcxvnv.sHtML

Ruby: ARGV
来源：http://3g.fanxiaobao.xyz/Article/details/glfvdzhrt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjvqvjam.sHtML

[M02] 读取环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gvwwzhulx.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fanxiaobao.xyz/Article/details/guryablfh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfixqleos.sHtML

JS:   process.env.HOME
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcimfxzi.sHtML

TS:   process.env.HOME
来源：http://baike.fanxiaobao.xyz/Article/details/gvwkugads.sHtML

Java: System.getenv("HOME")
来源：http://wap.fanxiaobao.xyz/Article/details/gcxkomxid.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fanxiaobao.xyz/Article/details/gegkbsxnl.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fanxiaobao.xyz/Article/details/gdoqmfixa.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fanxiaobao.xyz/Article/details/geehiruta.sHtML

[M03] 执行外部命令
来源：http://3g.fanxiaobao.xyz/Article/details/gbnnoyyjb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxlvwgds.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fanxiaobao.xyz/Article/details/gvcssqndh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxzagqyg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fanxiaobao.xyz/Article/details/gbhzjsmon.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzlpdxps.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpmvymdk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fanxiaobao.xyz/Article/details/gprgjtyqb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzxvnqyh.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gncpxmeyr.sHtML

Py:   os.getcwd()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxfvlrqi.sHtML

PHP:  getcwd();
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwnxbcow.sHtML

JS:   process.cwd()
来源：http://blog.fanxiaobao.xyz/Article/details/gppkvnjkl.sHtML

TS:   process.cwd()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxvzvpnj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fanxiaobao.xyz/Article/details/gvempgqzf.sHtML

Go:   os.Getwd()
来源：http://blog.fanxiaobao.xyz/Article/details/gkwpjwjoi.sHtML

Ruby: Dir.pwd
来源：http://baike.fanxiaobao.xyz/Article/details/gmtpxxfem.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fanxiaobao.xyz/Article/details/guohqzjse.sHtML

[M05] 设置退出码
来源：http://read.share.fanxiaobao.xyz/Article/details/gtelhbhqy.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyogoquwr.sHtML

PHP:  exit(1);
来源：http://3g.fanxiaobao.xyz/Article/details/grhgyfovu.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotptwlvg.sHtML

TS:   process.exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gpafhivrt.sHtML

Java: System.exit(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxssddfd.sHtML

Go:   os.Exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdevhczy.sHtML

Ruby: exit 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrpxtgra.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fanxiaobao.xyz/Article/details/guxmfizis.sHtML

[M06] 向标准错误输出
来源：http://wap.fanxiaobao.xyz/Article/details/ggjezbstn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gncintgxh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fanxiaobao.xyz/Article/details/gxktnzxsf.sHtML

JS:   console.error("err")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgemepqk.sHtML

TS:   console.error("err")
来源：http://baike.fanxiaobao.xyz/Article/details/gjofnbcls.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggivlkoso.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fanxiaobao.xyz/Article/details/gqashmgcn.sHtML

Ruby: warn "err"
来源：http://wap.fanxiaobao.xyz/Article/details/gzuzjzswf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fanxiaobao.xyz/Article/details/gszxbfhkd.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fanxiaobao.xyz/Article/details/gkluickhd.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fanxiaobao.xyz/Article/details/geudgxfce.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwidlautq.sHtML

JS:   require.main === module
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfsookdv.sHtML

TS:   require.main === module
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxomhsab.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkilmsme.sHtML

Go:   func main()
来源：http://baike.fanxiaobao.xyz/Article/details/gccmwzprp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqiymsyl.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golnokhjr.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkkakzaa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fanxiaobao.xyz/Article/details/gtoplrosd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fanxiaobao.xyz/Article/details/gebfzwukf.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fanxiaobao.xyz/Article/details/gayivodsg.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvrowqfj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnopazlzh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyxsaxzw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkwhuwkf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmairoex.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqkcmylk.sHtML

N. 数据结构与算法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkyuadng.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxoqqntb.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gxbbjisol.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gkdkevhxy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpybgvth.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdwsexrj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfqowwsd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtaprtqbj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxseqmlsp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fanxiaobao.xyz/Article/details/gyrieekxh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gnecugysw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjchcrktx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fanxiaobao.xyz/Article/details/gsraozuvh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuqyikdr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkigkrcvl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwnqehdz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmhqobwx.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/goegfwyzl.sHtML

Ruby: arr.sort
来源：http://blog.fanxiaobao.xyz/Article/details/grpphkjaq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrewewdf.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fanxiaobao.xyz/Article/details/ggkzporvr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fanxiaobao.xyz/Article/details/gjvgynhqq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fanxiaobao.xyz/Article/details/gkfxqeydq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fanxiaobao.xyz/Article/details/gsldtocgm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucwafiky.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fanxiaobao.xyz/Article/details/gpuxjqudq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fanxiaobao.xyz/Article/details/gfgpjjejq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fanxiaobao.xyz/Article/details/gizvydkxl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxowsmdh.sHtML

[N04] 斐波那契数列
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbltkmbc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gtjiyogmx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpbnemei.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxjuxinr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/grmdgrnkd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fanxiaobao.xyz/Article/details/gxvbryfxl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goaenqjmi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gpiympucx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbvfiqzv.sHtML

[N05] 最大公约数
来源：http://read.share.fanxiaobao.xyz/Article/details/gehbunula.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlhurxzq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gipsuyjvn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fanxiaobao.xyz/Article/details/gztjzfmtn.sHtML


<!-- 参考信息 -->