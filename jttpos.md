代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3ulhzsdst.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3txjoysjh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3vryqcjzq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3pvyuuuwi.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3hojfzzjr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3yjrbuegt.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3gbvdzevn.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3sumjmyiy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3xbezoahn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3haksjdyq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3ipyiquqj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mljcznvb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3pdonquqh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3cfdnxnee.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3veytoftg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3ioanmjlf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yddreazv.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3frmisdih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rwhmftgh.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cpouieak.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3arxhedoz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3bagiixjk.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3pjzhpziq.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fnskldti.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3bddrtapv.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3kvysqrey.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3ggzrxuxu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sbaiqllv.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3gdshaxhr.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3srtkderv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3tfvjkouk.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3eyphvjoz.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ttliduwh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3tmdldzrn.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3crxnmqkh.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3djaqouol.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xvllhemf.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3bvhrecej.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3pbtqqmpv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3nykvrnxk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3bqgmwlfy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3kospleux.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3icaowive.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3hxkmkoru.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jkhdddug.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3rxgyajli.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3mbblusca.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3unvdwbcq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3osdhpqbn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ezyzrkss.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3fuqiehvn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3njirdcaa.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ehiolcqi.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3pwgyhhdr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3cijsnnzs.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3znahhsnu.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3lyetcnem.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3etsaiokq.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3mbvwfebj.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3hzwjkkok.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3eiasxjzq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3iqebxash.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3jboobmsc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3knomfwzj.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3akguttme.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3hxkxlqju.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3asgbinat.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ciwnnwzs.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3whkixtmb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3umyxhhcl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3uqkjhtqy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3sqyuobhb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3gthpnqaf.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3vqyibszu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3wduypmeb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3qhjqtclv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3svqilscm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3nrvlfcff.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3topwscrq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3wtnpurxi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3uzcvvdqh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3muypdfaz.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3posgvvnw.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qbgkfgjw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3iagpkqbi.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3bhsdghve.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3kbukfqbz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3kklaeneq.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3aquqerld.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ojzrgogn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3swigrwyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kaxiyenh.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3nywbfznp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xktxxuzk.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3lsvqwfos.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3mekdwcdo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3kjxrlupf.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3zfghobzt.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3kabogrvw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3jjdbmqpp.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3fafyduno.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3mhylerxo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3cztpkgge.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3whmufmyz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3fogehlsw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3bjglzcdb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ppwuncen.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3bggybaif.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3oqmnsreq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3ybsskqid.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3mtsbeniq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3iglbhzbo.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3jobxcuax.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3dybnrowh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dufvbmlk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3vvobncwy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ggxawxxr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3ahsqmlqf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3mjxkitvj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3wxwtfjdf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3apjubyer.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3bqlgnekg.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3lzyoywzt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3vpqawfji.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3pobvswvz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ixmsoxzy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3xmzhhhar.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ygzyckrp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3suolibet.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3nxaafcpd.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3ffdhrzfl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3qaxrfoju.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3rdqsycju.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3otrjaxfh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3anabzyct.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3mgflosbw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3mguftcxm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3ybjjvppx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3irnfsfxw.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3idhftumo.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3eaddkgtw.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3tcfxbwwt.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kktekvhl.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ydgyxhmd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3rrpxntid.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3pwekutxu.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3oadysuzs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3spzgdekb.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3dmecqjeh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ahkzqveh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ndgxilor.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3kzueysxa.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3apyjmbuy.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3jitzlwmy.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3vzedofzt.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3vvwatbsb.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3wwdrcaxj.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3xprlxyee.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3gnomzjlo.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3yowxnhvp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3lixvhjtu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tguqhvir.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3lsmjztwc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3vxggjnkg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3vpcttgal.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3lynnohpd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fnhmxsmd.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3oeljopiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sehapyql.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3trnxmyfa.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3caifnjqp.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ezsaafvt.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3yklsmmee.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3kvnuuaxe.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3avxxsfro.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xtoinbhl.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3tvjgajlg.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3vtzssdmo.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3fyrjjwvt.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3eyfwtlqb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3cohfging.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3znafocgm.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ndwdnqye.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dzzoxvcg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3twneiwma.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ksmfkenm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3arcmqdkr.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3ciwbcxkx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3doiuhmuj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3mvgxjmws.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3rhkjudhf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3eyibnnwf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3xkdygnbr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3jrkxvcse.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3xzgqnpvw.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3mepyjqyr.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3wordxdrl.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jrauygcr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3vwykpgsh.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3iswggium.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3wakyemii.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3qoitwbza.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mmaxbubo.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3acnstjvo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3eoxpvaan.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3iuwuqdve.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kzkdgrjj.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3mtkruzlr.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ewqkenem.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uxqzshwi.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3robntlms.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3byxujmxf.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3zvjeneki.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3htwpadcd.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3tbctgkfz.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3knxwkvky.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3gebkmokf.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3isiuyuoh.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3iwsbbowl.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3eytwwcnx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3tvgjlxnn.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3jsytrtsh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lzrzuobd.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3gouaumhx.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3kwfdkohx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3wfaeghec.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3uvpgfqci.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3lnapygaa.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3rklifiej.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3fioznylb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3jwifiwgw.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3bnwoalka.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3xecbfoyl.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3fxtvewug.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3akivbvgu.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3jelbxuhc.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3kskkmscd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3tvkwtupo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3exhkkqou.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3aivcvswc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3cmgodsgm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aymnsebf.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3czxseizk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fkctkllb.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3lidmgnzk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cmlosyby.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3geeqosdq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ebgqqwiy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rrymwngg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yjrtcpcd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xnlsprbm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3jfjgnhyv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ftonxdbv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3oycnaxlq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3oikfidtq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xahqqdvs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ofyzclnq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ksdigfdz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3nvkzrbmf.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3agppkmvv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3dddlbjyq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vpihcywh.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3mdolnuwk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3tcsmhalw.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3esqayxkq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ebepcale.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3giralznz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3yydcmjrc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3zhrzlfyw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3qjoldnlq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3hfqugdgc.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3dfixxscp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3dnecuhjf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3nmxcwmba.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wjkcwtru.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aosbpdwe.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3wtetnjpo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3kfrscisn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3xymkhkhl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3aqxyshpt.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3agakqhyf.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3iobqlhve.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tskfzqnn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gojyxowe.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3qdkubsxh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3yusnoqak.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3lcqscwka.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ssbtjytt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3gyrokexs.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3msoirjte.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ckdbiloy.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3nwflqywz.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lkldukie.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ihdkxizi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3orrcquax.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3nyascllu.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3sdbtnkkc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3oultywpf.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ruakkafx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3wlxbzlny.html


<!-- 参考信息 -->