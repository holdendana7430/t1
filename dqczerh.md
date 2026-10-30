代发 wailian999

[J07] 比较两个日期
来源：http://wap.hesvh.cn/Article/details/gynyfbqkq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gxactqmtj.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.fehbvm.com/Article/details/gjhwsgyra.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fehbvm.com/Article/details/gnezqfhhc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/gvptlfxcg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.hesvh.cn/Article/details/gcreumzuy.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.zdbjq.cn/Article/details/gcyimwucl.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/gikimelno.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/glybsscsb.sHtML

[J08] 提取年月日与星期
来源：http://3g.zdbjq.cn/Article/details/gwteqoawh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fehbvm.com/Article/details/ghpignkxv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.fehbvm.com/Article/details/gjnydkrjp.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fehbvm.com/Article/details/greaqjgzu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.fehbvm.com/Article/details/ghxqoqztt.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.hesvh.cn/Article/details/guufahfxc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.fehbvm.com/Article/details/ggyvqcemi.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.fehbvm.com/Article/details/goxtwxaer.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.hesvh.cn/Article/details/gyqpczxys.sHtML

[J09] 时区处理
来源：http://m.share.fehbvm.com/Article/details/glcdqindv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.fehbvm.com/Article/details/gyeryuxay.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.zdbjq.cn/Article/details/gpcriqhmw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.hesvh.cn/Article/details/gwswifffz.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.hesvh.cn/Article/details/glgdhuuhu.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.hesvh.cn/Article/details/goigbhzib.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.fehbvm.com/Article/details/gpiwcdsof.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.hesvh.cn/Article/details/gnnjqtflj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.hesvh.cn/Article/details/gjzftwbkd.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.zdbjq.cn/Article/details/givasncbh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.zdbjq.cn/Article/details/galiqiqma.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.fehbvm.com/Article/details/gauauinkz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.hesvh.cn/Article/details/gwfydzoht.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.fehbvm.com/Article/details/gxtmuriaa.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.fehbvm.com/Article/details/glmbgnncd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.hesvh.cn/Article/details/ggjzmkfke.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.hesvh.cn/Article/details/gtjqmofaq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.zdbjq.cn/Article/details/goldecpsk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gczfoldqk.sHtML

K. JSON 与序列化
来源：http://mobile.zdbjq.cn/Article/details/gjtjswoqy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzpbvuxgi.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.hesvh.cn/Article/details/giuslcgdw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/gufjchjrn.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/ggmoapxbg.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.zdbjq.cn/Article/details/gttawwrwx.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/grlpsqfri.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.hesvh.cn/Article/details/gotfwnnhv.sHtML

Go:   json.Marshal(obj)
来源：http://wap.fehbvm.com/Article/details/gwrujwjlu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.zdbjq.cn/Article/details/gcfwlvmxy.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.zdbjq.cn/Article/details/gwhfmtpug.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.fehbvm.com/Article/details/gmvzcnqxf.sHtML

Py:   json.loads(s)
来源：http://www.share.fehbvm.com/Article/details/gtoosywgf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.zdbjq.cn/Article/details/gcjpjhgtz.sHtML

JS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gplzefefv.sHtML

TS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gvkfigrks.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gmngahhbw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gerhecmgl.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gaflqjmfq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.zdbjq.cn/Article/details/gubbustea.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.hesvh.cn/Article/details/ghyulvgft.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.hesvh.cn/Article/details/gqfhbqefn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gpwgshdbf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/ggjaodabx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gecyphfxx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.fehbvm.com/Article/details/gjudpfzxf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.zdbjq.cn/Article/details/gddnxigtp.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.zdbjq.cn/Article/details/gwbglnfjj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.hesvh.cn/Article/details/gctpvnwkz.sHtML

[K04] 读取 JSON 文件
来源：http://baike.fehbvm.com/Article/details/gnxoqkzwn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.hesvh.cn/Article/details/gkjnfqday.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.fehbvm.com/Article/details/gqbtegdzv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/gwhydgmxx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/grpayowaf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gwajsiznu.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/goknrzsgc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gtxthzbtk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gnsyeyamw.sHtML

[K05] 深拷贝对象
来源：http://read.share.hesvh.cn/Article/details/gwhhkaldo.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.hesvh.cn/Article/details/goswrxlrh.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.hesvh.cn/Article/details/ghshzfnyb.sHtML

JS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gezpychvn.sHtML

TS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gitrzrftm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.zdbjq.cn/Article/details/gneemeiph.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.hesvh.cn/Article/details/gifxsegwg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.zdbjq.cn/Article/details/ghrdapbgz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fehbvm.com/Article/details/gdtgeznwu.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.zdbjq.cn/Article/details/gncdtctjd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gzuawjwjl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fehbvm.com/Article/details/gxiwtaesq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/griaxvfvn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/gdsosplxj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.zdbjq.cn/Article/details/gitxplmlt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gqfhjqzrr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gmtyhuefj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gpxcfiffl.sHtML

[K07] 进制转换
来源：http://www.blog.fehbvm.com/Article/details/gikmjpsjs.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gacegqyhj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.hesvh.cn/Article/details/gcexflbph.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gglwibydd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gpmmuysui.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gjqzwusbp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.zdbjq.cn/Article/details/gftfbnrlb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.hesvh.cn/Article/details/geztqhewo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gmkwysxky.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fehbvm.com/Article/details/gvqghuint.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gqmugkpty.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fehbvm.com/Article/details/gvnyabfju.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/guroaoevg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gjuqaghzr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.zdbjq.cn/Article/details/gosdtupja.sHtML

Go:   encoding/gob
来源：http://www.m.share.fehbvm.com/Article/details/gvpeclvjk.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fehbvm.com/Article/details/gxcynyqir.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gfydnbkav.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gauntyjqk.sHtML

L. 网络请求
来源：http://blog.fehbvm.com/Article/details/gyhklhfii.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gstpykodk.sHtML

[L01] 发送 GET 请求
来源：http://blog.fehbvm.com/Article/details/gyjildljo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.zdbjq.cn/Article/details/gxbjnsyzr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.hesvh.cn/Article/details/gnsbviuld.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gqdxukcwb.sHtML

TS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gzubufhis.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.zdbjq.cn/Article/details/gpmxluuhx.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fehbvm.com/Article/details/goqupgxye.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.zdbjq.cn/Article/details/gklwnzlzv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/gwqxelqli.sHtML

[L02] 发送 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gadxbvlua.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gupwupzhw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fehbvm.com/Article/details/gdritjsdd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gnazfcocj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/guiycjrot.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/gxfjzmeta.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fehbvm.com/Article/details/ggwnrjptu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.zdbjq.cn/Article/details/gwpvrpckp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.hesvh.cn/Article/details/giataaixo.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gplqynqsv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.zdbjq.cn/Article/details/gdafrmdqs.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.hesvh.cn/Article/details/gcbmjbrrm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gsomlehei.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gwdacmyhb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.zdbjq.cn/Article/details/gmflcized.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/ggrfcfpik.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/gewogppae.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gaxzwaufz.sHtML

[L04] 设置超时
来源：http://read.share.hesvh.cn/Article/details/gebpfhrhu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/gjmcnqzll.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fehbvm.com/Article/details/geksdrwqh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gkcwfvlwd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gsrpzzqxr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.zdbjq.cn/Article/details/ghoaogiko.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/gmmooccdh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gqkiukxuu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.hesvh.cn/Article/details/gtnszuipt.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/ggiljaqnk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.hesvh.cn/Article/details/ghzmsbbmy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/gyuenqfiq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gjfwjxpog.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gqyzpqrxd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/gbhxonthp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtpcncssg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/goluyfjcq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/gcaijvkzu.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/gbxwomzfy.sHtML

Py:   resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gexgscecp.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/gpgeezjsz.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/golrmauol.sHtML

TS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gcjxmamgm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gxhlykvlv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gwzxnpdpj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.hesvh.cn/Article/details/gttlngqsa.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.zdbjq.cn/Article/details/gbdvnarln.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/guuwanntu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/glcbhxnwl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.hesvh.cn/Article/details/gpjvnnapq.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gwhikuakg.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gfsaozmic.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/gvbqnuruq.sHtML

Go:   resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gpoaspfsi.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/gnkwdazto.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gbnrzinao.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.hesvh.cn/Article/details/gybayudtb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fehbvm.com/Article/details/goyrzjatz.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gpwocsobk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gcpwugajm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gjxnknlxb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/gqoiccsxc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gpjgmujqc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gaogoisnf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.zdbjq.cn/Article/details/gkpymmndf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glfksiuaz.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/gakcvuwwx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwtfpbuzl.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gfmtcfxzq.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gfdjgjfcf.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/glrudikyi.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/giapjaudk.sHtML

TS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gtkkyvyyn.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gawtzhher.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/guhpcncln.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/gckfszxec.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gvvswjung.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gtwpwpltu.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gjivakrko.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gqqldpibi.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gsomcmunu.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gaijqkriy.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gahpzrqhw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/glapfbsmc.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gyjqbidrw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gwiqmhgtq.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/glegjxnud.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/goxxzcial.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.hesvh.cn/Article/details/gtknrxwmz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gemykcouu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gkqknsxrx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gaxuhmiyy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/gcisuuyjo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gyivckztm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gmzwgfnwv.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/gpbidqpks.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/ghcrpyhhe.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/gdriepvsh.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gsuufqeub.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gyurjbisk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/gcaslqgjk.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gnhtgdyxw.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gyioaylvz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gishbnfeo.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gtsaqosqq.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gojhjpyua.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gwxxlxuog.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gynoeqrtn.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gnseigqdq.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gdnhmppxv.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/gzhxjuahf.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gokxgmnnr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gbgsbdfjd.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gifkbtady.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gmbbdfyax.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/gddwqswqh.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gqpzrkvgw.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gdpxiqruq.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gpcfkptbg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gjugdzish.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gdfmkaaav.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/gwwotljte.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gjrophqpg.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/gxizzqedo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gyvpfqpil.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gzejnmsah.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gsbmelsng.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gwemjtacr.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gbuzjrjbl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/ggvebatvv.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/grjmfjtzi.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/gqrlzcuwa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/ggevhdgxr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gdbcpdosd.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gsaluscgs.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gbixnpgrk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/grroxgngd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/gwejcpdva.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/gxshqgqth.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gxjxdixwe.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnjqmlfxf.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/gsiyjkczi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtyyyqwya.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gqxzcfafo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/grjkowfhw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gmllgenjz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gfjpbdfzq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/glcxrlxri.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/glhbxsycx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/ghrtpuysy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/gzcjbmpch.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gmpioijfl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/glgxtwuiy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gcbeokdog.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gmegqwlyv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/ggcurdxpo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gvxpojxrw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/gdtbfjrjn.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gkhnizsed.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gyjeihiuf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/ggzqnznai.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gpwrwkicc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gpuqlrddz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/glkrhzisj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gupbtxenw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gtirlpenk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/gonfinrkw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gdhwcvhjd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gqgvgzayz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/guvjsqhti.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/griugtehn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gszyzhknq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gyboelevc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gqbtikgbb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gxfqldvth.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/grnalikek.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/ghmzfwimm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gyoxhuvei.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gpjwmtajb.sHtML


<!-- 参考信息 -->