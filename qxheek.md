代发 wailian999

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2inhugytk.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2gesugkxk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2mzwbixvf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2xeksipui.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2tswjdphx.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2ebamaycj.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2ptuczufd.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2qbgxacvq.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2fgwsjkgj.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2wcskwobm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2bebcvcly.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2harnsiun.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2pfelhxhk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2dfygpooq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2eielgqst.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2wgpsqzzn.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2tqgnbqnx.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2lrotikeq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2guhrfsno.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2cnnstxri.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2ripuphyc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2fhzbzwid.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2mrxjrepa.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2gjnkialu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2oyneihqh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2pldtuhuj.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2qosccpsx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2glkutrqo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2bdhmysot.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ngkkdqez.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2wezgbtmz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2vmkiuemj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2jlavgfaf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2rdptxfxn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2crjzxmpz.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2ezytvfde.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2oqhhokli.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2smgiznkp.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2udnootjz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zuhqzvsd.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2liuzfddz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2xdkavoyk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2jtxultzk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xuynlxbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2svtazzii.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2xfkoitjz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2quihnddc.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2emvpixqi.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2snbslqyn.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2nykiwder.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2swmzpapp.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xleatncd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2wtxkvzwc.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2ystmmfau.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2egaszdzu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2argwxjkw.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2smdwiivd.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2drvlsuzj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2qgogaekj.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ospcmoqs.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2frlxyxyb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2qcaeqbin.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ckkivbaz.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ldpgcsyv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2ldktdntu.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2eafjxckq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2bymfysvj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2yerjrfys.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2mgsnboxp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uvplcuyw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fchpgfay.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2kuljhwca.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2trazzrmp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2xtbnwqcq.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2myjjuzaf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2uuvvmntf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2clpknowo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2koqibuab.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2yynwhazd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2wtyltoeo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2rdmouafd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2sbobrjsf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2hfnfdxba.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2eedvoqsl.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2betufimt.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2qkxszwas.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xexrzclm.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ikyhjwbt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2kspuvtpd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2unxmuret.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2xxznackg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2qrwnlpkb.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2xeskmqsq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2xlxedeju.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2hmxqteos.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2fvkfplog.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2svussdfv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2jrbuiqxu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2sbibvtms.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2cudbcqzp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2dgdmecpy.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2gwuudrdg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pocyfwpn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2mwvmgsox.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2awrcmjog.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ewfbtaxf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fjliethb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2nuwrhozm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2rbouveld.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2dbhbceos.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2ajislhen.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sywalmfa.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nwxzgwgc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2vlzgpidl.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2kwhixwwy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2bnqtplku.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2trwdpyvm.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2htahyfxm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2rixsqcri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bwphcica.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2scizhfio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2idwmhzwx.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2tdrnjooe.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2zynpqjbn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2vwzlmdnr.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wwkglfdt.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jmpiumlz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2vmwdbpss.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2kiswhgia.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2awekaker.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zankzwli.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2gwnfypoo.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2uhcmvvcy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2ipncqavg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2kaahlhrn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2arlsqubg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2miqdrysy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2iiztcdct.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2yqobxpfn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2uzuwpbpu.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2kbkuwhrx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2zykgsrxd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gwxypfqv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2pcqlyext.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2fflkjupq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2trzgpvxd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2yuyxvpik.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2keuhzziq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2obabvndx.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2ydjmpecu.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2xqyrexfx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2jrhdcpkj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2sjudlsjz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2kqutlihf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2djhvxvvn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2csfdbiad.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2xlnhxanr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2aoyjdpbq.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2gejohhbw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2sxnoineg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2nhtniirj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2smrhrzlj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2gzttkkyk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2zvvinege.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2hmwfykba.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2lyfbfrsl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tlptjqne.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fresicud.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2iihsbhqo.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2gkgmuaiq.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2orlpizrx.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zeqhymcb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ojugjngt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2bksxbtee.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ujvbojth.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ejnrlrjw.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fwsrpubk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2mzpkrujl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2rhfqzrzc.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2yyhnipmj.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2nrkhozbo.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ynndplll.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ecrlqihw.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2uannjaba.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2zppvywzc.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2rsenyhvd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2gygxvtjp.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2giypzwrq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2tgqngxjc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kcbrezac.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ltxcpgjb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2lvgpbghq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2csycvaie.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2ihkhbkdo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lwdfvhxf.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2rfmykoml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dxqzfhtw.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2wfzlablr.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2yuvgujpd.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2kukoakio.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2dqkxvefe.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ugdttnsk.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2mnihspua.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2rrmvrwgr.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2wapbrlpi.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2bpmmvodv.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jcqpdxeg.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2infihhqq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2cbbawqid.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2nibrgxqu.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2zldzcqnj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nzfyqlpt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dnhnwwaz.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ggwsukwi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ttkhdyng.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2mkgeywni.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2pbrvtplq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ydxmgaoy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2crbyzndj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jkfuwhll.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2chabwyld.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2iutdcazb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ulnydzkk.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2cqpjiiza.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ophjoyiv.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2junjfwpm.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2ujoebgik.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yixuxfoc.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2tlvrqunb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2nalpuxba.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nolmkbmc.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ifzuhgpx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2aelqogkn.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2glorjbdy.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hxdqjgdm.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2srtezyst.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2untdowfw.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kwwdlitj.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tehzygqb.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qghkvazu.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2miequfdt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2xymjwaod.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2bwflvzen.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ctgebani.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2wxiflhwr.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2bynepccj.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2smlrfblz.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2yrbaivmx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2pteompri.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2veqrkske.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2bgjsfeag.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2vxtpedds.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2vbcxodcm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2nlofgfxh.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ylbedpio.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2qktdakue.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2nrtaxrtv.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2hpvgpzca.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2juztgdcc.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2owqkzcro.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2fuhkkwwv.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2csbzloeg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2hiwqkpbn.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2kxrjvydl.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2nieeqybn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2bcryfcbb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2cyrzlahx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2gpqtjyih.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2gieydymq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gumgkltr.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2dhdhbzbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ksbjmpqk.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2kbqtweff.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ojpczasi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2gggodgbn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2yxbxblny.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2uojfvbml.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kjfdhwmc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kenjqrdu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2aisrukos.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lgwnlugn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2rlabyuxi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2tujdhouk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2luoxzijk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hgbuvjtn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xghylvjm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2bnbguseh.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2abqoherj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2alqypbor.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2dvqvjxjh.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2uvvqxmyy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2rhwbnvrn.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2vtctdnai.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2dgrrlqll.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2kzrxfylu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2pesprrkw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2kpuyexqu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2lkwcjcdp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2roozsedu.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2lezmsnzc.html


<!-- 参考信息 -->