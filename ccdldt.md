代发 wailian999

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3zzocuyhz.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3jhahsidf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3lphdicli.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3kwrscbmo.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3aqwducno.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3dxsoosaw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3tsxmsecf.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3fvptdwio.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3rrvgjzmw.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3wslqrzeo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3mxabmpuf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3ssasyrdb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3uhiphvhu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3icpzvtze.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3lojprzvj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3ksklmedl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3hkhkipli.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3blnuczdi.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3jeibvuxp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3xcskihyi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3jptpiidt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3sntugulk.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3trbvnqbr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3wxuxibso.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3mbgxodfn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3hsvuubbn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3tynokrsp.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3wipfktps.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3uvcwxigl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3rsnaoesz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3heqxuumo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gvznpkls.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3josqarpo.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3xyzyuooq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3ddaumgjs.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3ltqjudou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lwbulmfl.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3kdwxhkqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gmmhtufx.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oceotvki.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3wuvpkybc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3bpfsineq.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3flnlxzoe.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3fxpckier.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3kdnrglhc.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3orsmuwni.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3gndsaxlv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3txicsstf.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3trwfkoww.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3cxbaclpc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3nmewwmtm.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nuatsmiq.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ogwzojlw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3emznvbas.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3wfdjdtak.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3gjkkndtl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3lxgnsrbq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3pjlhprgl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3bjyyrfwj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3ahtoxfqw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3ahazmbdp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3tkgphqce.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wxznzilj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3twiipdif.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3bjwnzuha.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3qdfbhmqu.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3aznnnkeg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3iutnedza.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3cqifkccn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ihpxkobg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3xbiezuir.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3vgzscbqq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3xqsczltc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3iznkafnc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3vnlwwhng.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3ezvuwasq.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3tzbpennu.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3irmldewr.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3vognngyy.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3jsmswagc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3mwraaspi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3zoterlnd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3sbmtbens.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3aguraczx.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3vviblnbz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3aterxivi.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3qzdrbieh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3cnijyaag.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hkgrouqz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3nuoiudok.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3hwfbyhjf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3bybvtsox.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ifldaair.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3vqaukjbl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rcodnfal.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3cwlgylft.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3frkhcgfp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mamcbprc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dvpzzdsz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3sqcvmpyk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3hvhbqkrn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ujvtkuew.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3fvzwibtd.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3veenkbgi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3upqsrxpf.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3tniehgql.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ltyqrnzb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3rxdgktas.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3zpyjdswl.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ytnhiewv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3nshguosc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vlypcuju.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3zuuxtckh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cshasmzg.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3uyjhrjgn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3yxqeitsv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3ktnhasrs.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3pjwqjhpw.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3wqjwejqt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3dkvldfhq.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xmwcwyqg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3qerpwznm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3voakxghu.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3yjqlrizz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ensqcnnw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3wlnidqbc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3xviwcksr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3hlxpvzvl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3yelwpdfq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3zvmhhsto.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3oslygsmd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3svesxhdv.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3gfivyzza.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3pwkqpxwu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gewyuagy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3cffekcxs.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3nhnosjxu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3pifbzzps.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3rgcpozqu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3yundhpom.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3mmiffvyg.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3psurrzzq.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3cfkkdaop.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3vkggyzyp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3tyfszkqv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3iadzwusv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3gpvhakcw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3skrjeryk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3cmybgfps.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3osacqmvr.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3qkfetvrv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3vlsvpxrm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3tfvedsbz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3vcdvbfti.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3plbewrtb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3nmhvvtwu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3pfyobrwk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3bwqpiumm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tzgfadoe.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3xvkocqql.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3uvqztgqa.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3yszfxrra.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3yonjfdtx.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3uiepzkmx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3pmhqydua.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3onbckupy.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3iqfyknkt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3fdlcdupi.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3isbszmui.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3gcubzaza.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3axldfvpg.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3cuzcqtfs.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3bixmbwsl.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3bdesgimu.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3fkdrvbzy.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3azlvqmpa.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3jaollsdd.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3azafhrkg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3opakxcma.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3ltucrynv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vxqmmkkb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3djgeucui.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3gounnmtu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3gzarancg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3qwnytkyu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3ixfnxrdp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xsdpzipg.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3uznqrngr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aumcljbt.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3sbswzhsu.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3csyrpxvx.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3tksinhxm.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ibaqermd.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ithkgafw.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3zfpossrj.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qqzymwuf.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3muvkromw.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3qhzfbwcp.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3axgtuxqs.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3giguqexf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3dbxrfrmg.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3bdqvubos.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3bifnzlqp.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ohqcnopw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wndxzfck.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3njtzsvys.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wbcqilfz.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3skalkmyf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3wzixpdqf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3gdgtrkia.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zjevcypg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3imijnqki.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3gaemoieo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3kfujsmar.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3xwvtalnq.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3txmotpya.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ngicmmoh.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cejfvbdf.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3nwtcmgzs.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xspbcyvw.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3llyopeyn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3weblbrpo.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bpfmlzbn.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3taczjaaa.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3dyijpzhk.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3rwzuncac.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tqdwjckp.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3qezguyrs.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xwofcwjp.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3otetyvqp.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3oglqiqhu.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cwjqmtou.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3edqhulxi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3pshxjhcp.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3nsqhneap.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3yjitgzeo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3caljaojh.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cprokehy.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3dxckvltg.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3wpigkzlu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3qtppwqil.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3qnkgjsok.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3iadpsfha.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3tgowdqxw.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3oubyapjk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3hkoftizm.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3gymebyck.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3evvtfyte.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3jtghjgtk.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3nleqjfyv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3jlmalnuc.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ubriudkm.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3zwcflxel.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3kgmlpgrx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3kcpibywo.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3uoenxgpw.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ivnqaaqc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ybkyevbj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3jadmzojw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3ivauphpb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ckzmycbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bjxmgnaw.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3kqinrolz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gyipspgh.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ptdpatdb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dqqchzxu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mgjfqcdo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ujswfgff.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3cfdokvfz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ftytltcn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ipjmtvfc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3tequyxmk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lpbnffno.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3iyhpwaxw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gxxytuho.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3zsmyufgs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3varyhmks.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3jktojgda.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3nqqiirlw.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3cljccpue.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3snqhgloz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3vwbwkwvd.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3khacxjub.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3gcontmvo.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3zaeejuzz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3dvjpybgh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3oruqator.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3tgexwsdu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3fwujdazh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3qoatpwmq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3zaggvgeg.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3bvbawnwe.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3cquqouhk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3phwoaikr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jrmwcdue.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3yqqpocfp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3zvqntmgf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3opgfrghs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3xeitmmgi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vazkqhxi.html


<!-- 参考信息 -->