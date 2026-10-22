代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2vtwksdjz.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2ayqbrkpu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2rfjzncvf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2fkwflnig.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2tzwnifaz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2mrgnflvt.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2uiuosfaf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2nptexhgm.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2tzedghpb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2oicjldaz.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2alsfsxfh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2ovubpcut.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2vajtkltk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2nhjaewnk.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2pknjuazy.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2kdilhaga.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2kfnsdcwp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2rkzwqbvz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2qimhncts.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2fmzggqbx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2puomatkg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2rzdaprrw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ywoxlqrn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iwvadpgm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2nrhqqode.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2fqrodpwc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2hdlmfdfp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xmdrurqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kcxtspse.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2xcgorcsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2imqlxnjg.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cfkmhnxd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2gugppqba.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2kxanvrpd.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2rjeinckp.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2shnzjdep.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2nqjkdtqx.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2jpktzyuo.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2upzcakkq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cuwqjcxi.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2vhhpqzrn.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gxksqplo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2khdsitmz.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2kfjacseo.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2oshtgvgw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2cdwurgim.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2cdwupern.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2jkcsvety.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gszgbzfn.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2krwmvvpm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2tyxxeszu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2zwevnqce.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hkgcpsna.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2zufnunzj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2okexyzpy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2tlbianbf.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tsdtsomg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2aqfcxorn.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2feecbcih.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2ukswcvvw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2tluwbbtr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2pktauggs.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2mmjqffis.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2dcorxlns.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2vjsgzzso.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2eapdttbj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2cwhsuery.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2ydxzedmw.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xjuhjrny.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2nnogpchp.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wwzvwxhf.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2wljdlzyw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2ruhkprvp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2ysxvsrru.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2riqelbqy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2npqnhdox.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2bozrjadu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2kvwccgoa.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2pwprmlni.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2hvatyacv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2qdxeogak.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2vzsrqnvy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2imvtzyli.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2vkgkxvve.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2jmcmshes.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2pafzdfxi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zahqujwe.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2inbfftqi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jgghfybd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2eybaenhu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qkootlts.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2qworzbwy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2cktqmroz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2sivazqzr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2pukopolf.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2chtcituv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2mldcxfsn.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vxvcsqor.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2wxirhahy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2iotjvngl.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2htfihzhg.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2lgioekdq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2eftcatph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2moxdumzh.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2iuszgkzc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mjldnrbu.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2fwjxyikg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2ncvbcfgw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2xsfpunff.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2jdrdhlpn.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zddfzdzi.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ozyxcviz.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2gpefhici.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2lkwohnty.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zvyjfevo.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2bwgbnfky.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2enzobwys.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2uzhsysir.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2gwsbmntr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2rqhlcpnq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2mjijqxnt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2mhflaztp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2cagaaban.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2jynmbdeb.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2spxmzwud.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2vthwhsop.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kunsobbf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ecqbewkp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2bqwmdffs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2cppifkww.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2gkzlaxxa.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2rvohjske.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2iqvqrqmm.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2jiysttio.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2tfpcrqqa.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2xmmaaxbz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2zzlqqfpg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2rzthsavi.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2vbkgrtuk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2xwplmmgp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2rgzeigcm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2uvbswvjs.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2xmaawkjf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2tordibcn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ceilawfd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2upnvokiv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2jxqobrig.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2bqugsqlx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2yhmgxijh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2noxepsye.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jxhcdxec.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2yqxtkqll.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2xqoidlzt.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ytnhknav.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2daipckhw.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2iycopuig.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ivkclsku.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2pfqogfzu.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2zxbnxngv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ujvyajep.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2qyuporaq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2hfmereou.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2drrqwpne.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2boanpqnh.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2rdqluqan.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2jqebkstd.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2enpcxcnk.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2gamxmeqj.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2pphxfzac.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ejjqoywx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2bmpbjcec.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2bvvowxif.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yqqbupvq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2yvinlwkw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2sccnjxxn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2uaxobbog.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2verkmjsz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jtsdojtk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2khbjhmas.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2qwhuwueb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mohmpecz.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2euspeohm.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2cdiokref.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2jthpjtaj.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cncexpkz.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nrazryeg.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2zbbexcqm.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2tjdljxrr.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2qnhmbspz.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2fnjtagcg.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2tsyiuhtw.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ysolhyyk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2rgorlquh.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ffdzsxxf.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2lbrhitap.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dgzbrepr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xlgvdrda.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ljrxeziz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gxdbkeiw.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2adjuftxn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2vsmxmscx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2wyccfejh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ftpbjvcn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2gcdwrsir.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2onpupxmz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2pzsjwljy.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2egjwblds.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2viuejeep.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2iaklhbuh.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2dhcnnezu.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2oxmovoto.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2uukocpdn.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ejfqtovc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2lccwpgpa.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2axbywxld.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2vkctwfom.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2wivcseqq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2nawepvfp.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xlkdnqel.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2bjituycs.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bywkciqq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rirffcep.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ibdetalw.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dxbtmfen.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2nhzztgio.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2beqdarmx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2iiynzuuj.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2quqllvzd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2itjlfext.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2zygxwisd.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2juscuhkk.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yteiosdz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2vfhbmjzf.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2lhsjuvrb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yladhijv.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2zxycfglz.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2vwqlxdik.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2qdqhggfx.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2nbiwoyvm.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2gqkiubrm.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xzkgempl.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ovqzjmmi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2viyeqobn.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2utcahcny.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2epnoswxq.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2twmgxxkr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2rjkyfrrd.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2urvatpkl.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2omtyqauk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2gpkqzxmb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2pizvzked.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2zdhgbucs.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2odpsgsns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xuvvpnwx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2jgvhbxsp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wskshdej.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2plxdnqds.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xgbhaqxx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2emzzlwho.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jddfjyuc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2lvcztdgb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2umsrqriz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kusygtnm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2ldhjuhfq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lkmmsvvm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2jtswnutx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2idpejtyh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2inqikneo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2puvsowsf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hnyvrzby.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2wnkcawzh.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ojrvskdr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2whgnasrq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2vspxqofs.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2hchuxwsx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ufjhsrqo.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2gcplcacu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2cxkcxxyc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2zqekjxpb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2qgydpznn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2tmrvumyh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2zhdkaekl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2fpryjelh.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2czyzocce.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nlfqgrlj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2hxuuixve.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2iyiwjfol.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vkelzjbr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2unfldmxi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2ehzlqllo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wlpcpygu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2tnyimuws.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2orjtqxkf.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qlocxvcd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2knautxup.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzytmaon.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2snvnbbae.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2mvyynkva.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2eryazvfy.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2liuiyksw.html


<!-- 参考信息 -->