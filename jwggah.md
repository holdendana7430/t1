代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3luqmyjsk.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3conxovfs.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3fnmcxxdv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3sonsqeyy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3xjcvvvow.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3mpcbvgad.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3dimvgcsr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3xuafiekw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3jhzmxemd.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3ldbkbcez.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3pdircqab.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3fdxoevxo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3zpwrmqfo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3tginzcch.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3jexbfpem.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3xxlmngov.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3vlpzkbrc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3pidisbnk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3kmqhruxa.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3fahcpwbq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3grvpnqrl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3jmsttltf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3teqxefjl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3frryltig.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3ygauojeh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3jwdrbznc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3djtrxmco.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jasiihbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3felxaakl.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3ilqlbwbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fegsgvyl.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3bnhtxtig.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3loiukrbn.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3fnnmpvfc.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3zubagcje.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lvcffdiz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3pfwlcmav.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3ysolzuag.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3trujojlu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3wevzpnqt.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3isipkasl.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zvejhbxd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3rtdixluf.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3yjofbojq.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3utajhddu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3vovlbssn.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3cgxyjsml.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ivppkign.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qgajjbxu.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3efvdmaol.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3qhxczsup.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3xeljaihy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3jgyszhwi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zqwtoynv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3zkqmiits.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3hyqhnwnf.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3qabfjmpf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3fclcnwzz.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3ksfozuyi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3xmbuubud.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3vkedysxb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ukiakdeh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3iutaptnk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3cgjbncak.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3etoiemnw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3dhjxkgbg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3staurdnq.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3uvhlofya.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nhomwywm.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3pdcefkxs.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3jngfdsdu.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3jztlkcus.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3zwhlcyzh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3hueshzrt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3homjdvlw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3vlfzzexh.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3cbcgcetz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ypxguywd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3jgpucpye.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3qcnqucyx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nfviqoci.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3bmifkatj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3szmfpfvj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3hiqfiaij.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3xzfkjjhj.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3zvirvllp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3csvefdbc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3zuvlamgh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3hkhugmvr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gizifzfp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3glexhvah.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3kjeqrlre.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3aqcugpqy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3bqpqasha.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3gyvzpvkh.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ytjbpivq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ucaltwbk.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ugdbywrw.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3rzuyxmzo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3uhemiarn.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3ootcvjak.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3npsnhyzm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3pbaadvkf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3euwvqzoo.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3thlyenfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bthfpizp.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3moscvrmo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3xtwauttn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3yzutzmsa.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3cfcwwfni.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3dipnfkjd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3eqqkqzny.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3acpklndi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3akplmufs.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3acpwfcvp.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xryfudey.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3syfrudcb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3hprrvhfe.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3hesrfsmv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3vrmvomhq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3tlqqimag.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3tggtbsrx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3zkltcgvx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3onavyyzl.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3uwbughaj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3crrktsoc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yhfzibaq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3vjslsqej.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3tpvudnwq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3iiglbpbw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3owlkmgrl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3yzvbzlds.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3fltjgxcw.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3ihsnctyw.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3hdggazoi.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3sfutbwqx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3yyseyifc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3vzqmnwgh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3xjgorvuw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3hqwnpbsy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3brnaqaql.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3kehpakcj.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3xhxwxzca.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3opltcvwg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ebauewvq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3rwktkbyy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3iouvqcug.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3xwmmjdrj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3gnwiowdy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3nkdtqsjt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vdbdlztj.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3oxtlezys.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zegxajrr.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gepktmvi.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ngrmtebh.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3gerwumky.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3tuvenldf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3xhexmkmg.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3bwozfqye.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3wznsxsch.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3gfpkkarn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3jlojixft.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3zoefhmqw.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3uaneqgoh.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3cgyvaird.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3gedfkdvl.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3vhxmqnbe.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3uhbknfmr.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3uaiovorx.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3zfwebenu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ickgqfcr.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3sdysobge.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hbnyjtnf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3sdnatcdf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3onghuzff.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3dkpdlvqa.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3upeuizvh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3lvtklmre.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bfisoifz.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3rvndehcf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zroxjehc.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3tpyupvub.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3gggfqkrr.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3rjduspzz.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jpozdgtg.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3aoltzuru.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3fpjktvmy.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ndjrbcmu.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3zhlklpbo.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ottqmfgq.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3zyfsbhzw.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wsyiaabk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3vqesbujo.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ysxehgqo.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vhkhzbwm.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3doiynxpf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bvuhbxml.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ysjjmhvd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rhmalkiz.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3jomiroib.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3tbynzgii.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3mzpmhpyy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3vsdqmccg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3jthnysmj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3jgociisq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3suuzmgng.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3qejfqqem.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3ejpdwrlk.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3ihrmlpog.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3rljsrmle.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ajeebhxh.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3itxgwihr.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3pcgjovuq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3olwrdquz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3rwhiujuc.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ejydkycd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3inmcsdry.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3zndoiral.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qlvhublx.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3qwhodugf.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qfubplaz.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wtukwssf.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ontjjags.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cstjjegr.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3edxkbuau.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3aqlqyvtm.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3xumrkjrw.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3uyvdujgd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ophokdhu.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3imwmwhbi.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hrpselaf.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3swggpdnr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3functesk.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3smqtgzdp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3neawraar.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3xkybkfhb.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3lnpjbpar.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3xgigchqn.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3zumegihh.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3hyptuaaz.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3nmezaefe.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3fzkikzsx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3dyzyegxa.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3wbwhaqsx.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3lctmhsam.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3xwyvjktj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ksomlhgs.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3bdrcukjt.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3knpxwuvh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ynrmmmso.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3hllbclhu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3zkasnkbi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3lkiuqsij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ddxruzdp.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3yrekmfoj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cfmoxrui.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3rgsqpcbn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3srptwfut.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jyggtzqp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3crxylxga.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xpvrklqw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rztyzhrr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dyhijbgx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3rayurtzb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zdhbeyjt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3xhyjjvzn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3hikgdzaq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ymkkzkqw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3bvimbjjk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3txbadwyi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3kwzvonpr.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3scovpviy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3njlzvstv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3dttbyqql.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3zhsacoyf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3kaconndq.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3wbawgghn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ofcvewqf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3lwkfuitu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ukjqkfii.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3ctlatbed.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3fiueaobz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3harkhoqw.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3wrvpnlnb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pppggbpo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ufxkmpmt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qgylkmhd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3gffoyvzm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3qxtrcinu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3xgwnxyia.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3rqbxjdwg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yzulnfvv.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ilbvwirp.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3pebcdote.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3feyzgxdp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3cfohapvq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3bynlvhjp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3lkwtkpux.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3scrhvnay.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ukfhvmty.html


<!-- 参考信息 -->