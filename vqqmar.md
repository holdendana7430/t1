代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3fxgkcwzv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3bqlpnlpx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3jkcthior.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3yueyedlp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3ypjzcobd.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3raqdbbnh.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3jarinhqy.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3msxtwodl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3hstlzurk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3rzrwhauj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3xhpijruq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3jlmjyuak.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3qqaaocen.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3uncgvrti.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3ibuingyi.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3zlkawdlw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3wmaseyqc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3rvyjoyyz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3byxskjyb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3sqoctqjk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3iridixyu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3nslhophf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3fiwxpqnm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tcoqyfle.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kbyvzhbc.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3nemntqip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oxtkfmyt.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uudzstjd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3vmkzslrr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3xvkctkpm.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jniiwpge.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xruacuel.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3zahjsqkl.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3zsueglhw.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3kfxvveat.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sudjxife.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3wwcrkwjo.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3touprago.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3hmxluorz.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yliqwwpe.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xjkkrjvx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ubqshuxu.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3jvindfda.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ublrzhls.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3wqopelam.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3moyqfeiy.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3yfzeiyua.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3ffqyggnl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gmlfxrgj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3ndilxsir.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3htblsegs.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3avwoyspg.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3okmffzcf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3ffphfngw.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3nixeukcd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3bhaerjqu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3xjoqtywu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3aoagbljw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3kytwkkty.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3rjusbwat.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3nqmxkawt.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3tqjsnfrq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3lyrdxnyi.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3jadvegno.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gkwlgjii.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3brphgmte.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3vpdmdtbr.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gzulzkpg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3nyannipo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3kpukvjhn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3kffrtpko.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3tqyaepay.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3xfjmggui.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3mnzzbpgb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3nogxrnkz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3pxmcsfgm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3habmhykj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3tjclegho.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3pbeibuet.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3hvhpqgsm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3crgfchpp.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3cojlmzat.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mpepfulq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3alxlhvrr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ngmhxhzm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fxmcnlzv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vzowykei.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3tabmcvzh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3jwakwnxy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rlqmvwqd.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3tjntxxlw.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ewiprpsp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3ltjsirlh.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3xaqfotxm.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3zhqyvnqo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3cpevxjgt.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3sfasdepb.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nhgseged.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3zomigepc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3taubzkrq.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3ytqxtwfg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3axfhbqlp.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3vlqdtnnp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3qxsyqrsz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3enjdvmtb.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ahijuuik.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3moxhvkkd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3qzeptjzu.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3ppdyeamb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3dtwqvruw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gdbwkzic.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3eyrlwscw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3rodzwitg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3yiezjhsm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3nfugxzxo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3noyveflr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3kmofrrze.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3wpbxshin.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3mffqafne.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3vvbbxuun.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3lubpikgh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3qwdgcuwc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3rhtvbgae.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3xprfqkzq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3egnofkql.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3apoglugv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ijazfmwe.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3oezsczam.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3nglxqqhp.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3goxusaxq.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3mogorbtb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ftytfllh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3sqebxxkq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3oaxlfifh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3cwputhrx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3epljznus.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3tfzvrnyu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3xtuuooto.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3vaitrfya.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3lzswmoyd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3qtiixedq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3cpsmbmus.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3iuclolcn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3rxldphfx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3qdvcwyft.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3ufmcxgla.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zulkoepa.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3suhjuaos.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3egxqjzcj.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ndcfkmuj.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qcjmebao.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3lqurvrdn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3vhnspsyv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3kskqayko.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3maocdowv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3zgtdnwxc.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3pcrbnhvg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3ymjhkikn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3aexfyuhh.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3bupiikzw.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3pycutuvg.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3pwjuolvs.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3anwjtnht.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3aohtlsta.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3wlqjjfel.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3pkzklxuq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3xcrdaojs.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3neqdkkxo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gboxohjw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mygghcwo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ogbuxckh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3osmlvteb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3irfxanln.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3toqjzvtr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qvzyarfj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3buxeupcu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cajdzlfb.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ykhjibyz.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3fyndotiz.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3jjfsvwin.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3wkkvetjy.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3reuvyalc.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3jrhbkdxq.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3jhudjobv.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3aqcedfkf.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3gzeylsis.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3glzbhjen.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3eykevadg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3hmglxher.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3avxdaxit.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3paolldxh.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3idvbcygk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nxuehyav.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3txxjnmav.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pzebcggq.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3bfubnujq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vfichsre.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3xfhxlmcy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3gurnbepf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3hhdwazzh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3jkcwhkwi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3rftdaaiq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3aluwczta.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ovbhqcai.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3aaokxava.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3diskgyzp.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3xwxnmyan.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ehebcaau.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zeevrsww.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3iywykdgq.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3uduteeao.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3goqazyyc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3lrzmaeps.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3wsoffblj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jzpuafou.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3wlppqtri.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3otvmqkxr.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wrcpskby.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ribznbbn.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hvhdbojk.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ttuedqbp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3zfubdxpd.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3fknpodbd.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3tqiunylr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ycdfjhpd.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dtebqjwg.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ksjinjdl.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fnlkvzjj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3lponvwlc.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ureuvzpn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3pvaicegf.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3cpqlujbn.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ypxfdosh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3wqrnovqh.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3zzltzosb.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3vwgfwpmy.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3btutiayf.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3euwprilb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3gmmcjciv.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3mmsduiak.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3pmzhhbsn.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3zjxpzigf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3hkvanpcf.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3hvbbawqh.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3qlycglzr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3tjqmpwof.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3uzhhvneu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3zkjoubru.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3oxqbmhmr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rzeoijgj.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3kfmfrpms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hctqwyke.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3diqzjxwc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yctwzpny.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kgjceztq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kzqlryzz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zoxmayks.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uckgnqig.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rtaerdlf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3wcfgrnci.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gzfgzats.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3kjjbolzj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zmpjmqhe.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gvkrqnal.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ncptbanh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3glonslhd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3vrotfjmf.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uzwxholi.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3bvmishzg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3fgpcpbau.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3yvpdxtsk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3elffzyjc.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3akdckchn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3bfqdnorf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3yeylwtps.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zbscrnik.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3kdqzfuys.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3gxktpglt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ueuolhpv.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3kjiunhqp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jcaqimih.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3llvsmfdr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3afdabxjs.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3lzkkebza.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3tawvnrkw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3lnfgyisz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3rklwvkxh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3itpxqqyv.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3nbogbysk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3edhlsqpg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3svplqaho.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3egyknolc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ghssbnra.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3xlkivwqe.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3wpuwphbe.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bhxfcvei.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3eomjxrta.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3djsyizus.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3jrcefygz.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3agmmtjeo.html


<!-- 参考信息 -->