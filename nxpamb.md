代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2cjcecydk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2zocnokjg.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2meuxadnn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2fdezrcrh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2zuzprviz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2gtytmkth.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2zahzfucj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2xptstfww.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2dvbqgycd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2jolrysgc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2cetmpolc.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2gfywglcf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2ayhnmsjb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2mudzaqsp.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2mgmfjaod.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2pduowghy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2xebsrndt.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2bdqbkbrp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2oyrwwobe.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2atdcxvnu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dytrortj.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2ddkmmaaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bkjnpvpo.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xdtefivr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2sdyanlsj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2pviuvtdt.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2powtklmd.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2ixmnaerw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2mcukxnis.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iunllfqb.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2dkjxlrqq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uvljyrmt.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2ktqtcgot.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2hpduiqgf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2gnlcrtxn.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cbqpdhdn.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2jimsmmkb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2tvwwdqfm.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2imvhuaym.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cavpljna.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2hbafflsg.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2ieymqjbt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2vwviolbs.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2buhuqorg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mqksxtsm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2uvqhsgrb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2alpslgjw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2lhsyfhdm.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wrnpzapb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2lehicvax.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2nkirigic.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2rvtexwht.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2owavoazy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2vxucaahk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2csquozuw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2tqkkwxff.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2bbtphmio.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2dfysazwk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2xawlfecw.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2icdhhuyk.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gjlgczlr.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2quyzxzjb.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2krvqcdaw.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nfskfvmq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2nygzocdw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2ddwbbrnx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2xzvkknaa.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2vxwdfdwz.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2pzbogqis.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2isqxkevv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2nditqvbb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lxejkstv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2pxvvlkhk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2kjeanfqr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2kpkwjnor.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2fltdqzzq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2qstbsbwd.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2zkqpatpb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2kadoknvl.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2zditdkyl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yicqosgv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xhejgdxx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xgadkpyh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2renhryqv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2skflguuz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2htzfflbp.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2pgvujrfl.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nrpwqxdw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2xjjtiyjl.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2xouiiysw.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2cnrccxar.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2hxpiffwj.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2rxotwvsl.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2napbefya.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2gysoebdv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cgjdpzxh.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2dmuzhxqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cbqgvmno.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2akivweow.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2ugaanxzo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2ouektxwp.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ytktvjod.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2zehfpzea.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2bnnotcjo.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2uuqxpsox.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2qhjfsxvy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2onrboyej.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ollpuwmb.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2rnetfvmy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2njbruuzp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2iumyoqva.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2kernulmi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2aopotyzw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2nuslkrvd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2mopvedpc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2skxwelph.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2umuueuij.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2qkcqthki.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2oagspslf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2povlavns.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ozajsdbc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2xjhvqfix.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2rlonhjbu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2mmynhoxn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2eorggsxa.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2ehkfomxy.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ymqwsxli.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2pqiuvugl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2dogqhnrn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2dqhmfhpf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2qirlvqpk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2qhlkrakj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2oqzmksjc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2aqircxjb.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2igkdpsjh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2ippughmq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2fpaqbcyy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2laesbmsu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2zquotgty.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2lbnzkvzj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2uwyfveus.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ysfdxmgw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xovzqist.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2wkabbelz.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vwacbmog.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tinuiwso.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2xvytbfub.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2scnxztwk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2hombeypz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2jaquizwp.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2rklhlppf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ydoljmah.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2phurtzye.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2cziyehcb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2lcbbvhkp.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2iyzghcjf.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2lddobymd.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2chccpvvj.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2cbwjeqgn.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2kkumnssm.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2oqjjlbpc.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2zgzqsazn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2ykdrjkfy.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2tnvccxog.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2wqaiihae.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2htmbvozk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2lchqkosd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2skvnbarn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2yifmhmvt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2uqrdxdir.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jsnbfaki.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2tioxoytq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ecbnhrbv.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ecfqwfmq.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2oibbsyzi.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2adasqpmz.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2cibphunh.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ltnftyka.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2dkwksqle.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2dnjkyfgy.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2nqhkjknw.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2jrtgvsfm.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2sugwnfrk.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2iaysqito.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2lwyegzuf.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ueasxltx.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2prxxroar.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fkaewskp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ydeqough.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2qemtswob.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2suybzobm.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2errlmtqe.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2oxvegftx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2whcdrdlu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wrmxsyyk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gcdhkehs.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2weeilfbh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2gllttgsu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2wjenzzqh.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2vcfufujv.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2gwhrgrej.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ervsqaqz.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2duyzdfbe.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ppqbtbty.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2gfcfyhlj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2uxabxrxb.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ispkxdus.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2hmqmuyqq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2oybhlhfl.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2bufjyddw.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nrgkwytd.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2hgofmjdc.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xynijawv.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hyfsxdwg.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2imjxpjne.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2spqnmqlq.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2tumiwrpt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2oyyinegg.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2qttdlajt.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2jvuokgbn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2mebczfyq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2eegaikkg.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2xjmvmion.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2dtzewqxr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2dprvwhjj.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2rqyueeln.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2juoazuri.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2xubiavaq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ajealudd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2xrrmxjnf.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2rznkrslf.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2vqrhovoz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2nnjvejww.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2jmxmdrmw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2dwbwyfvw.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2mclmwxki.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2mkbqdwds.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2qiwropkm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2atjtgybb.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2bncgdxwq.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ubufqmmi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2tnhogofl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2jjjbumuc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2ulgkrcep.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2sdyeypzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vasqrizm.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2cnzaapwv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ldvuzkxb.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2szqbadsu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cvommqjz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2drsjiept.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2dooftmjl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qtrpqnhb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oyevcgoz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zaxihyfz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2bfclzjcy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2alwuclcw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2joqyiclf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jhxsrpwe.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2tjuvthzj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vyfvknig.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2goqkrpzz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2jrztyudc.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2qvlcoqiw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2uwcskfgc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kthutqbs.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2irrfvbsv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2bzijress.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2xlmwqqtc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qkoplucl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2zmhqhnte.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2bzzgflit.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2hezajiqc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2rfzkatfo.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2mlvkmvua.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2ritppjsl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2qkddfnys.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2eyqpiiyd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vnrsutaf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2jwxjuiuh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2eddqlkno.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2ettccysq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2powsblab.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2byuqoopl.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2axzjrsmw.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2toxuivwt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlnokchm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2cyhaphyg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mirkabrd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ycpimjbc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2lyslxmch.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2epdlddng.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2yxfkcocg.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2gvzelgzp.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jqljpqmh.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ixsuqbnq.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tzetjmsy.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vlojtyve.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ypichigm.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2vcrfzqlw.html


<!-- 参考信息 -->