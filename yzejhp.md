代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ukcefwsz.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3qdbftisb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3zvrxmboq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3zhnywfkp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3ekcdltvm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3yqxctzys.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3vmmuibkz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3veohzouu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3cnghiveg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3jypslgiq.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3kogsqmpy.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3hgxtuhsw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3mzcvgcjf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3nmunwmrz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3uzpkxxub.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3bvuuuxwx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3tflcvpxn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3irgqoalk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3yuyhraji.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3dhwozqzz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3bqcwcggd.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3fxfquavh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3bdopezyq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nefuljzt.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3ocbchjir.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3jyuraqai.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3goveyowl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3xexenonk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xudnyaaq.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3qoqbkqkc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aifqfybz.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sdkvlaze.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3nviznevl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3gxawhqzx.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ajrxfljt.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ddcqinvf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3ixiwntdf.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3ocooxfvy.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3ujevuhoy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kzkrzqli.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3sqsignqs.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3mewehrwv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3teaegrma.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tjkhodyg.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dfnoevpj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3chcceofl.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3kuzgefjz.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3onawkacp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fmvrssrx.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3ruarrjsx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3jbxhtslw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3yvireavp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3efzwbvnh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3iyuroshd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zrcjusgy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3pzscdwgq.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3mtavqzgx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3tapsrzjz.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3xrsyewkb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3udvfrani.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3hhzyvcrl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3qzjqhwaz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3cryntbqd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3lmgjydoc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3nrlqqdob.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3bpytjojj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3yodafpyj.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3awiykegi.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jpcajdgp.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3nwigvffr.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3egeqfsdr.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3lznsvyon.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3obtbgvrq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3vitwsbgj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3bwltylgy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3lywklthp.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3njuenmls.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3pqvmiudx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3dirziaph.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wigufvxm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ngqpesbm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3dincatng.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3cpdrosji.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3fcwyhzxc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3kbikojth.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3rhxyjwmo.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ahqkwmnv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3ndancdkw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rluhmqnz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dpyoypxe.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3milpxzyw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ylbksqbk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ufqzuxog.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wbbaemvj.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3abzdnmnb.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3sysgwkbo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3qkltrgro.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ywvxdyjc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ljmuzjsa.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3aqxtyour.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3roistoyd.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3bcfdxzhm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3hhrnyiwy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iwiwtsjx.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3bzkuszxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tvkczlfh.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3awqssyvc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3gdiaznsy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3yqsugfro.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vxhxlsda.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3aweypsgb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3sxeulvxl.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3nlrvamzb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3dmrkzgsr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3mlwontra.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3lazojhix.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3txsjoghw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3egqfxggr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3zhwawmvk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3lnxrfypf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3xxmvpccv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3llamkfve.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3mefbdcvo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3vuvsjigx.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3mcbyamol.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3opgktweh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3afugxfrt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3nbsynmkl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3xfreofxn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3hqjrynnx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3awvesgfo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3xqcfnizr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3hmwssndu.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3ftnzvnek.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3qxwrcqww.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3gebjhive.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3kldwmhqy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3yhcfabmx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3htsvvmdp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3bgqzaipy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3mxnbohyz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3fxahvzoj.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3hfqnanys.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3fcrwtxgq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3fifwdxbi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3stykphbh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ewticuwv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3klarkcfz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3xyalpgrq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3ezgoypwe.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3luozzasw.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3jidputoo.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3yfyocgrh.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3twfjgxbp.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3yxrrqssi.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3dojmhmuj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3voprwpot.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3bccpyuoa.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3ozzzcmcl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3fceagrtg.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3leohlqqy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3bgixxfij.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ewpklozm.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3rzsrfxsf.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ujusayrp.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3daubqyrq.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3xqqqtrbj.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3vuetfvdi.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3igamgjxu.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3axtezwsd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3tutddnkd.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3hxnvkvou.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rfgqtpba.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gmsjwtys.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3jjlrhqdk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3tgoxybgc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3bkfzkjge.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3vndclovr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bjmmbaup.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3urcikusy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3llahbjwk.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3abovqoqp.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gwcmwjjq.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3wgnqbhcx.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3esaydcdg.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dxkjyfvo.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3foolgbyg.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3pddvsmym.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3kfvdsmcm.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3cirydvsb.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3huisvfal.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rzpkiplr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3rhiqurjd.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3exqnyyrm.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3tehvkehh.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3sgfcolbf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ycecxpfi.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3fxmgjebv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dkugzsgg.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3njfxrqwl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ofklakos.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3sjykfowy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tvdrwxtd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xmarhpze.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3vmpsooba.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3icvrtqea.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3rbvzooml.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3afqwqmgk.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3vomwaxtl.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3uzgcrmdz.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3pfsvdsot.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3crqcuknx.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rzmeyahd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3bramcrjh.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bfxqvimk.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3gwqezwdf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3yepnohrx.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ynxmwszm.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qhvyoerb.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3fglfwgzb.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tbjsszav.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3segafyyw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3drjeulib.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hwpdzxiu.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3bqnhsfnh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3gvjwymuc.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3hegkknyb.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3vtszfcjp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3urzktyzp.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3odfrsqzl.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3sfmgyjcz.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dmrfcyta.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3qpjwctvk.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3souvrtwh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3hswepwxi.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3bjbdzvki.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3kfuyqipn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3fmerzafb.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3elyjqydk.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3rdcpzibs.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3lancawqr.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3khzfnpzi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3gwjgiijd.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3gisooguu.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ttfutjrk.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3vfdthpqf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3jboysxim.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3tcljvueu.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ayikpega.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3mltcrkeu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3ewgohsky.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3jugizidk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ntvozrgz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cgeowhqg.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3stgcmknb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tatjcgkc.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3pabrhlxb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ujrabnon.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3hkysairx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xgujehzq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3pgdebqay.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qfedlasp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wyfyitpa.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3veyfunfs.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yfughuku.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ocuosmzb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3cjsbyqhd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3geqgkjqm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3uvbjnozw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3dchiqcbz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3esbkpvec.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qofpbxrs.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ljqeadxg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3fmvgngth.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3uattsiqo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3rcbgtnvo.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3dkayxvuc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3tmfqxsdx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ecyahspr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vjqyhkml.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3fyowmzkl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3jwallodw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3mgqccwzs.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3dvzchoki.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ouvuqopz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3vikgvmmv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fxydfrwo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3cuktljxa.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3qejxgpue.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3zhwlqjpc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yuynhkfv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3erkoocgw.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3fzfaiiro.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3kbqxfikp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3yxmiichx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpkhpwcd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwxwxxcy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3oxvfvjwo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3zbsfgnsx.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3hbfsfjff.html


<!-- 参考信息 -->