代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3zvnsipgd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3bznsntli.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ikwowliy.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3jnptvqhx.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3yjmrlixf.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3aoumbcbo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3ykpfsdkf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3tdmtcoda.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3egboxvwm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3utgcuaho.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3gasidcwv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3grzuqahe.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3msteqvxc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3svvhwmpf.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3cqghbvas.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3zddglndx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3kcnxswws.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3bazfmslt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3gvjqhktt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3clwvwyrx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3pdakqdbt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3jthlxtak.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3zbfarwtk.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3srtfbhzh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3tnkjgcus.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3rthyquxu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3thjjdypd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qkurkifo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eckkblhc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3kfgzqpnd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3ykhvaxfz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3nyrflobo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3flckvhsx.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3xcgfpfoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rxxmmgxj.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3uwkoqnvy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3ulwrmbhu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3xvfrnoxp.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qkgzgojn.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ivyhuwaf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3nbzorsim.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3leenjllf.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3ozqswawn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ubqhpdbq.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3kldlxpys.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3emrhdncl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3acsatbkt.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3opmbticy.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3muhbxwps.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3rcycqrws.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3orafesxu.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3rtlmcsaw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3ihakwrak.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3fytxbrjm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3zpjasqmm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3vwzysgyk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3sgpycpgy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jrxuwlzu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3arbgvnpt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3ioqltsqa.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vltpccri.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3swhodfed.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3rzvxhzzz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3wyhribbu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3wokatxre.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3byhbwmda.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3yfnibauu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3hyyyqaih.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3qhlkwspj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3cjlagdyy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3znznpmvx.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3ypxygmqk.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nfpayrob.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3xnbfhvqf.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ivexrneq.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gthvsddt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3hojucxag.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3zgsorygf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3blennlbw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3krzpfume.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3zouhzedv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ghwatdvu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3wvniqwcr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mllkaady.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rhdalkkr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ewijjnte.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3flbacqxh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3jfnaxlwp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3quojinmd.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3buukbtmn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xauymdyj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3hjyviswl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fmztqhnm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rmllnkde.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ysxzyotu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3kqauezar.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3wzumzrek.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cqcjsxmi.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3nouddibk.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hjnerslh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3samzumox.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3evrfmglg.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3xgaqsfyv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3vbgouzzc.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3wejgydqd.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hhiguihe.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3xtjeonkg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gasslezz.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3igwuxhmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3okfqjsks.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3hnaifjij.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3ofadwcvf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3caahuxfz.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3wogxwnzm.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jnzlurdz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3kjeoxdno.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3nvwdpxnk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3fwahgqjs.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3napnnjlm.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3gmougluu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3vgugswxx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3bealfzqq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3owqyrgcm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3gvjjwses.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3rqelhiii.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3maqmdvyt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3fowhkhfl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3qimqtuqw.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3ledrfvyq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3wuvitztt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3uyvcjaes.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3eorzdehl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3hvzszgqt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3bajvowkm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3xugnsaep.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3wmgeuxfg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3jytwpavs.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3cqxhleys.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3otgtbqjx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3enbeszkx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3yvhcezfy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3wzofpnkb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3rduecqml.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ngekkypk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3mntqlojq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3tltpqnmk.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3tqtmdcmm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3ditcdqly.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3dlsrtuao.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3umtshmjn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3hkttdsvt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3mnwgqxmz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3kjdmatll.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3zlpiudpo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vgrrapft.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3uvbiwqnj.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3gcwtntqm.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3npccpfom.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vahtwyiz.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wxyozjrp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3qtsidrex.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3hdvvwpyu.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3zxlfeqww.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ikhvxwyx.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ooyasigu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3nxmhypwv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3xdistlwl.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3jchsryyq.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3llxiyfbx.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ngnlbgda.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3lvcsjvyc.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3ckydtxqx.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3xcglnywz.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3soxuszmz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3lwscdpvj.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3fegngyyc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3rhyrgtbu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3aeeejyfz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3emfpmhxo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3yszxdsed.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3iluhqjcc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3wubsrcqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xvxijyjs.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3tbiffnzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yguijxqk.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3zepyflvn.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nuoyrpvy.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3xjtxworq.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3yidwdwfl.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hdacqawq.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3aktjhrmw.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3utquaifp.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3shlpjsyh.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3dczhpkqx.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ifqkoxps.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kscrvzqf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3nvztlkvn.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3obtynafz.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vseinvgc.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3oyqeknwc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ovhxnrka.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3alxcuqha.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gqiljlwp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3ulumprqw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lezklcjy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3nlosmqlc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lgajzoba.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3leytdhwv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3idkvxppb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3annmtfso.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3bwawxoly.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3wrdpenkj.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ziethntv.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3iskruxbu.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3vgxebzdy.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dqbelbti.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3slpmywrb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3lsusqgdt.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zewhlrrf.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3pvytemqq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3zronxhio.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3kklqdxlf.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sjhptqvv.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ihzgllbm.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cprbxkml.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ftvaltme.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xcygfpsu.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hhcwluki.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3hgbaqiqp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3tnjdqudw.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3kgwxxnfv.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3wnyykjsu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3tsldpvoe.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3eugnpsqn.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3mxhojutd.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3awxtwika.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3uihefnfk.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3pmkufxyq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3jldfohgm.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3obqrfitx.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3tsbvtavk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3hghevndm.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3quqhkmzl.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3fsspqxet.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3xwwwifhl.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3ociujrta.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3jfiwirid.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3idufurct.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3rimjiqmu.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3qikjaone.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3eyeabjev.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3tqnlvlhc.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3nzrsexlo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3tphuucms.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3oimgtmrc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3zmqdjxtk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3gbenjuxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uuwpnewk.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3jfnvkpxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gidgthcs.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3icuaxumd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iwyendyf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qubppvgk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zjnhpoar.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3spqdrkpd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xgraxbdr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kshblnma.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3rcydcsqu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wkompumd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3nxotriae.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3cfwisljb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3wbceynwp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wihupfgb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3jacyfocl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3xathwbao.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uogcgphl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3oomktipc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tubdstae.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3cfyknyej.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3rpfpztmp.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ctwvqjkc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3zgfanicd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ztsvgtjb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3hypcxelm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3vmoejbbt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3zvnvbouy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3xibcgfsw.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ojndcikg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ggdnoyzu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3vrmjikrz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jdxdvkqt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mcurvnia.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3rnkcceid.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3jkyyrobq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ywrflstq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3afxedacn.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3odltlrxc.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3cojokydf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3slvndcwc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3zlaggsto.html


<!-- 参考信息 -->