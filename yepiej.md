代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3gfqjqlmf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3djyxwlze.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3nzvjgvgy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3ztymdihd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xyhepkea.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3wvuihsde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mbsqgrjg.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vkylxlsk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3zhnnjerd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3krubvvpc.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3puxkwawq.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3ehyymqog.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3cwdolamn.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3ndoyrdcy.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3pqcpxskp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3qisgakib.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3creqzele.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3lduyxoyt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3vtgaetdv.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3tgawmpem.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3srxtgugr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qejlaghn.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3kearchox.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3euqgztyb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3enklzxkk.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3cgycocyg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3ekhqvvci.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3gwbrubio.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3nyxwwfik.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mqowjtzo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xgokufdy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3wjffmfgt.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ealsnifw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3dczvuhhr.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3tqlwphkb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ppnwrfti.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3mbiolguv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3aqiiwlms.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3klqradsq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3pkgrjjcp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3bfpgxnuk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3smyfifak.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3biwtumtw.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3aoxmopfm.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3uwmhpovu.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3qmczzktj.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rgonnutr.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ftfubjfu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3gzxyubic.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3cubxbjxe.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3ertvxrng.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3reafjlna.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3mniipgog.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3vnhymcea.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3kpkxovpf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3cnwmmcvw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3sttxbkia.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3kavweowb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3hincqtiv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3tdlywgxr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3gxiilsur.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3eznvexsq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dyafxkhb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3gfiihopo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bmoqmnqd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jftagzny.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mblxosud.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3rpivcyof.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3fotdtdks.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ragyyiny.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3qmosgnmg.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3uyoaqbfs.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3efkuhmzk.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3jwffmcra.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3repsgrbo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3cnbnkjfk.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3grtyhxir.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3uuieglub.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3rmgtmtwa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ipwhmkfk.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3evigazet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yqfehkpr.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3zaytefkw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3sjplnreq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3urziuubw.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3uxsetxjv.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3jumnbkoz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3eblxtlgh.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3dicllvty.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3hwbehxdx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ezaaramw.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3kwlkpxkk.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3nztwfsbx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3nkkterpu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3xcbosqoa.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3qdgsmmli.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3mbkykffu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3xzaihgoj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3jliuhzyn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3cxpnwqpg.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3ljtxtzgt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3hybefefv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3xamwumkn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3drqnvaft.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3dsqjiumg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3ycemuohd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3kyaqufgz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3leycuvpw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3xnqkizlb.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3mqtrhanz.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3ykgbvale.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3hucvoguv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3naclzkmc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3kotehvpx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3umlbrrgb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3eymswrli.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3qoxennfv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3tdrtdnrg.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3abxpgnen.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3zdbavfve.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3pwckkamw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3iurkcgzc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3pyapawgq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3gxrkzwgb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3omnlvuvt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3pgdrdptu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mphvljef.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3dxgxihpj.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3xrvrbads.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3stsachir.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3pphptagp.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qvjmupsd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ubrpimmk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ubsewfjo.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3prydeplr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3lrpcmotb.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3larxcmuu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3mpoattjs.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3umdkwaiz.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3igpygboy.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3wozeaytc.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3dlssxecf.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3tosgyksj.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3jvyysbld.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3njcawotc.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3sanhrabg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3khveodrh.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3dnalfzpr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rhgtfduu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jfzbkviv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3odxmyxqf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3ozlvscwr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3rggxstvg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rldxienh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bwcixlyj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3uaxsrkhw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3waatzlsm.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3vatohngh.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3hxoxtddf.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3dkcxnyia.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xbphissb.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3spdprifq.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3vyyaogxt.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zfrnlilj.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3vrjgcoxl.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3xkostpbq.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3eneixunp.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wlnreabz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3pznajuhm.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3nqbfokgx.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3pbhixpnu.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3spdbmyib.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3eitgqzjk.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3fioxqdrk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xsbswvja.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3jayezeit.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3naltxfuz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3xidplclm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rakidrhf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wiecekjt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3eskwpzyg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3dxvatuys.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3zsxsulxp.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3hejefpvp.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3iwdxjeqe.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3iewmojry.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3exureinw.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jibbyfxl.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3zjuiddtd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3vdajotob.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zlmxbfmp.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3gxdthmeb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3mjdxllyq.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3lyorcwoi.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3advgcpeu.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3qpujonlm.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3etoevrjm.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sotpeouw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tahkngix.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qancbnwu.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3njsokvqx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3arcasfyl.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3nfrxdhyj.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ueckxegl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3xptsspwn.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kbmqncoi.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qvxdbmcr.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xscvwpyb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3uxkhyipo.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3jxdcfkmp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3hdmsizkb.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3sroorust.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3ihazxwmy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3pjnafwsw.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ozlfqwdv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3hkximmfi.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3igscvqna.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3kcdltfoa.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3iofqitpu.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3qkloytqq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3xwimskvv.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3rdedxusf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3kgllvics.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ivccmoab.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3mvepgpay.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3edtuhbca.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3onyxyyml.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3cwtpuata.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3kuickdhw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bkfmlrjp.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3fxbzegdd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rrwqtanj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3rtmtrqfw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3usjzksqg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3dxthmuye.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3goyyctwf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3yvtenlva.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dfhrsiok.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tqiwmhtj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3nlcptlnk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xyksotbr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3efmefrqc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3frwaslvt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3chsikhvk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3fdaruhhl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fzjoemxx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ncqvpvqv.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gngnnalo.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3veemnmjo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3wtrilbbt.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3pepxjiwn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3qbrgzpcs.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3djdzouga.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3yczcseme.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3lkdhsowb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xvrtncep.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3xnhedytu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3vtqtzrqg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3juhzihpr.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3wirhjttq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ttgyqgoh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3mbfmqqjp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lfpuqkpo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ujqbdtxs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ehyzajur.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3neroffvf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gdiozwaf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dlrfzijo.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ffynjdqt.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3brqvfbtz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxjisomd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3cpbokzhp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3keagpnmf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3tjfzdrij.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3dzltxvpy.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qvpkczsh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3vquyrsur.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ddeyjqji.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3gxwvyqft.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hiujdsei.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dnfedojp.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dtyzmgkq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3xzlgqtfz.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3byvhyepd.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3prfzbmls.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3witalmec.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3qszrbznr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3xlioqhpx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3eohgvbff.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3kowketqv.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3icifkqxi.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3wsjnfjmm.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3ngejbbix.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3qvsidqwh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3fysshbir.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3dkkwkevo.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cknnmnqm.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3wlzyocum.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zupfnmrp.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vsarcmfw.html


<!-- 参考信息 -->