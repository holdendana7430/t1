代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2iuglcznv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2mfffgcma.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2krvbkpcq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2kyxberte.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2pbwzapur.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2gmucgilj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2swojlsuw.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2auuuntfz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2kajkvblj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2jxkokyek.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2xgafiiuq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2qmlimwrx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2bnxakjpu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2smdtctsk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2vchakdhb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rxudworl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2enogqfdf.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2ppldpqml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gxdmvykw.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2nvirlklc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2ubmduntt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2czhjjryj.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2exhuzxpy.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2upnnymsn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2hpdxtxtp.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2ngqunawe.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2cqkwwpin.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2fzufungo.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2uxangrwc.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nnkyluvb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2bbybripm.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rixuizmf.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2imqlolev.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2abuzbtbu.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2sjwsjctr.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pxhemaac.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2oiugunek.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2gfcmttuv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2mlqvlauv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2aicmtkng.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2sfwuhtzo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2vrzffdsi.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hhudakiz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2xiljbzxn.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lkpkylwp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2tewqyjka.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2yzbfimof.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2iuuhttax.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2tulltgqo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ibbvecyh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2vwlxyoqq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ytqeamkb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2pjalkcbu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2frqotxib.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2awiyedym.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2yrzcfmfz.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2ohcsmawu.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2tflwgvxi.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2fsqtsqnw.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ugleohpo.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2gzyvemrh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2jhdizudj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2pcdnzoik.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2jpbrtbzs.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2vdjszkwv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2alcsuxwd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2prsnltpt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dwfvzjoj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dmrldamx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2dodjptdi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2sscozaxc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2edbzffcn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2vilatjxj.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2omkqlwmc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qqwqbvpq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2ayqeakpv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wuqvupbq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rujrhoif.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2susksmir.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2snvduowo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2owjahwng.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ckbnfyrz.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2kjkuhjgl.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2bvzvqzmo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2mikcttef.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2osfiwxln.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2vhfufrun.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2rcutoies.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2peycspbt.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2utgyexol.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2qxivnrnx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sanipusq.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2abtfmnru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dwksvrbm.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2lqgqmwet.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2lbdwmuaq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2aefmmwsp.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2iifhoyjr.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ikbpznlv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2psgrixtt.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2aafxzhfv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2gvfycmni.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2zfboujte.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2xdoytiga.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2djqakluu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2xacgztvx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2rehbjgrk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2omvdrttk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ijnuronu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2xdcmtqua.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2pnxvkhyd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2buertdna.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2zjlekqob.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2ncxsdklb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cxwustdp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2fmnbdodk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2oixgmjce.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ffwjcdho.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2wlkmxrfe.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2dfhwsamu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2plvfwpjc.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2kplpxiff.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2mpcejmvs.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2ymxmvsct.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2pdsayllx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2eyaycspw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2xtxqllrk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2mmdezpdy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2zmdtnwpa.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2cyumjqtk.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2qpudxjeo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2frugrnqm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2hmaqrjyp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2qdyeuwcn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2bgksscth.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2aolxqeag.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2dizxgaxp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2sbovsgbf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ehtlvkcv.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2niubnypy.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2khfqcuga.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2drzcgjud.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zuqdehhu.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hlijhusv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2nqmoqepo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2tvmutpwo.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2mhjibfhk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2fyzhmkiv.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2heboednt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2uecrhwkb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2usinippy.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2dvpmcinb.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2fnyquwlp.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2yyekkppa.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2sycuiyxd.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2puvbhlmp.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2cbllhcsk.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2wjiuvuec.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2subqgdpq.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2cdrrhtoh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2hgilgncp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xltjmkfy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2sanzakkq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2llpnbhmq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2wojdkvik.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2rznrohcs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bjookygz.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2dblmzwcg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2daziyjji.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2fckmurvh.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2eyhyhlfk.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2xnvwytxc.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2xuztidwt.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2edxbpeta.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2asjrmneg.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2padvzine.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2mjzpcgty.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2dswnmujw.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2gohxkfcr.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2luvwgotl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2buqpegxv.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2akzdelxh.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2qcaigpbv.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dvqdzekl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qkdtnzyc.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2mjryfpxz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jhphdgne.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2zsnyqmkp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2hqvyffvl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2cohgrrzt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2inxbseev.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2erzfolqd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2iottyayk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2hgzzsecb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2zxgrzkfg.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2xacthxym.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2vpgyfews.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2fhmwtrhw.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2igzxkpon.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vvoviiuk.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2mvoixskh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2jxumwvav.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rgefynod.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2fyivqczu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2gghivepc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2czlomeoi.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lnmftcfj.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2xlnzimhk.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kybtrgea.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nrvopxma.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nefqvbco.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lfzaqgti.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2qmoxbqct.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2zbloxjme.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2kehhcbqr.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2dghreoji.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2chbeypau.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2kebtjrzi.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vmliikbw.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vupceiuy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2qxaobtvi.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2qyoyjwzq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hnncwtxw.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2eyoiqxpe.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2katztdlt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2muchhtti.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2sfpxsjse.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2xabepjpe.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2kparwndp.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2mljuazlo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2dnpmxmxu.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2vldttwqt.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2uiybobbe.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2aprxyvek.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2jfayjvqn.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2pemjgtsu.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2anonezxy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ibsprudh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2fonuybaq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2hvmrasmu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2hivbrbey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2trwmscte.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2togyhvpb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zojgfbvt.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2iofgoxjf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zlqicqsj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fcwnzupp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2estsqysg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2nakqjgkp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kjuabfsp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bdfdvxjw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2kttohwiw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2amhrpyhu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2vryxnpva.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hrvmfsvl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rhxrjcsp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qaoeldsy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2tgholthn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2jhuzjxqx.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2nxjiocox.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fndgsdox.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2gzosrugy.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2krxczcpb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ohguizvj.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2kfzelskl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2aoopwunp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2yvepobhz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2fouehioi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2vsxibtoz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2jkyhspxd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2hnokdjyn.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2hokwyhhr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bkroqapc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2qkquvixe.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2grhumsoq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2pqhvtmgd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2uiakorhu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2arvfwhle.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ovdibkev.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2egbnthil.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2kgmvmfgd.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2hcmawjhw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2csrvwiuj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2adrdfrgj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2rjrjpgtd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2egparwvb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2ghrlfhhh.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2apogtlgb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2fqchfner.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ukdejeka.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2pvesbslf.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2zfkpzjyx.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ryzqpcgu.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jemwmpij.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2bhhkgljc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2qssjwpao.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2kuvuzopm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2pmhmsyfg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2qxtwsing.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2qerfwhrn.html


<!-- 参考信息 -->