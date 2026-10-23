代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3btfblbvi.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3oqmwrptw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3dhanlyrz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3navvrzdt.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3mzepydmh.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3jwowybpa.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3srjkdlxt.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3tplwztnv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3nlcfojfz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3itirongn.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3mnjiawlu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3rrfhuypc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3ihjrbvzr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3hjssuwne.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3tcdrscci.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3baseihua.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3espwbvdz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3gcwrcrhc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3hurxxlya.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3vdqlioyk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3raxowris.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3dchfssxd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ubxepxmo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zfadsybj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3omyvyytf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3vzomoiyx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3kgqdvawo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3wohdjuqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eshrekdm.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3rkhjaaoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ldoyyyjp.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3odqetbyh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3fuoodlic.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3piprqxww.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3lwslmplh.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tkhnxdwo.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3rvnbhvmw.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pmcoudup.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3qsokaitc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kkxhuorc.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3nzpclqdc.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lnsbfoio.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3fiufjumq.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3dwbkihoz.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3fubhoiox.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3brkxthql.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3gwldbkpo.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ddmqhjyi.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3tsnezjqr.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3clcehyte.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3ceqvpzhj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3sabfcrfv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3iyevgecm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3kglckkqj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jxlgupgz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3nljqiohz.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3glbxlkud.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3oextmwey.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3cqiklawv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3syawsppp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3dgzusqzb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ixgkjnyb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3mshkvmve.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3zirgqhgq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3wsaobapy.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ycrxzdva.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3vrsgycsr.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3uhfupsvi.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mddgsryr.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3roldjrqn.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mfwtxnpc.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gecxtklb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3wvryjavs.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3qesnzfxg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3xxdlhfqi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3urtefzve.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3rblpunho.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3xhjuaeoa.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3vtiqtiku.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3otpdfmkf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3butbpzge.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3hagtsyuu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3wbtttzsi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3qhthtdsa.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3vzfomlsx.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3ldhetdwg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vqrzsycx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3kcqmmdve.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ibkvtjjg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3hxpwkikq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3hbljqluz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3tymfgtdw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3eesofrxm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dddgqhom.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3kwznetwi.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3yschspch.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3uauxjtwg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3asyouwur.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3kwonjyuw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3nczlwpsl.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3odslkpae.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3fmrpkhsj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3motqzipr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ayvjwyfr.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3gbstjpvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ngizutxg.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3pazvwvbj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3vqhzdrvz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3iyvxkneb.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3danrhkgy.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3qmjmwvea.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3eeipzgcx.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3fkkwuhyg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3ufhtvorw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ewouwqho.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3raqfdxvk.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3naopfrse.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3kzukvygl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3hlvzgohw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3mkulfmkd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3euidyvug.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3lufcrzws.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3gdzhzxni.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3kqbhqmil.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3ngtluyhw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3taxwkwjg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3okrukdro.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3lquwegmd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3erzsyhqg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3rzgtgset.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3vfnaryku.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3nynmpodj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3tguahxxo.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3uopczkyg.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3eehqwgnn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3rmeegjle.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3nzmfcoaw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3fcerquzo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ucrbafqg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3bulevhvr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3fiepxbmm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3koriydup.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3jgmlvrmu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3lgobuhky.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3cbiifpmw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3cugnlpnu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3nwtrvxoy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3trhnqyxq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3bhqwbhmi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3crsqlbto.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fhyayelu.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3loyvtwtu.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3dvbrhfyb.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3jrhnqfrj.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3hzlnehjs.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3wkbmfuhp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ctlxflgk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3cgmgjfid.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3ghaqhhas.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3aplaljcr.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3cnoeodht.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3wpvhnptw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3eyhwyuid.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3zncsyvvu.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3wigweosq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ykqgjrbi.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3vextpatd.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3xfuxcpmq.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ovidbavf.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ezfogsgc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3tywobdcr.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3snnxpeux.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ztwwcrgs.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zegvwrfy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3aqzhxtog.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3aoaazyek.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ihbjxnfk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3aalowbce.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3upbwkgzi.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3jsckclwc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mqxfpvgr.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3mioxcovq.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3eugzoixf.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3mgkcaprr.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3alhoafbv.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xbakwgee.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3owrihsfq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ldjowrlw.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3urwlwruj.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3pbptgpyk.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3oxgbezlc.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dfycnntn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3usogwejr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3xxhkjzju.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3nbadpekm.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ycdyimis.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fefegmvv.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ofpeursg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mttzirdo.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3dbpzkqgt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3kyhblhyu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ejhrryel.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3elhjlruk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ynpeddjc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3owgvsbyf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ndoeewpx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3xweenhha.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3gtrozkvm.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3gdbrexxx.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3dsuxogwd.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3fyezklev.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3htcidxir.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3utydbwdx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3jcxljqqm.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3foxggbhl.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3ugcywsxo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3okahsrjf.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3hgqsfwqi.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3efzxybtn.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3lidlzpuk.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fozuexqc.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3barnsgnt.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ccyfxhzu.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3udiikzdp.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3aoedfztp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3wzllcolx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3wtgqyrig.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3wfdxqdjv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3prfbymbr.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3bwuqekzy.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xuxzkvym.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nsucbbnk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3rwtphehn.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3jyfnlkok.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3nqpdbule.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3vseuvtrq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3wivleynp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3mcghaqho.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3swrxrsaq.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3evtyozlp.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3osefdtqw.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3peninyzh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3iwssiqie.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3ykvqlfmd.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3dyiwaqrl.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3kmhjfkno.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3wdvbqrgb.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3idizggvr.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3pcilgtln.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3uqyldiem.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3qbrqrncc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3mpjhhuln.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3kflshszb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gmkwlxee.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3fqvrohpn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qethizlj.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3gjcmtupl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lbzyvaag.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3buxeqlre.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3pfzrnshr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kufdzizs.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ykrtfhvo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uekysodu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3winwzhlw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mdbbyulj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3jyymtkvc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jshbwtfe.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gswrvuxi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3kymhmpuf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qtpbjtej.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3juhmzool.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3hwarlinf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3kauxxnoa.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nkkmylcv.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3csnzhpsc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3vjdeljon.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3arqdhqnt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3kgssmxds.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3pxgyirqu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3uvsjduye.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3esrqzkfz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3zrfxnjpk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3taksyjea.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3svxrdujh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3rdpdhjmz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3scuwyndu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3cbmupjof.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ioqmjjvg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3fklindyr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ullxomdk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3sqqdqkin.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bxtlqqhe.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3mmydjbup.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hkskydvm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3iotpwyki.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3gdvslubq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ritzcjvv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3qwtrphgj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3chsqeiix.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3smebyipn.html


<!-- 参考信息 -->