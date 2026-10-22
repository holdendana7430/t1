代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rmvcgrhq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2lfgpzalv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2nwnbpkel.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2vpzrhppz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mccrsuxk.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2lltnojes.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wxjexyts.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hdcayvmn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2elcssmdu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2xyjwthlq.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2iwynohcy.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2plezauzd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2ogwajmzm.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2kpkkovqd.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2bidmwrum.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2ceailyki.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2xctibxgn.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2ezkjxxga.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2hlalvrjo.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ockgdzub.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2vdphikrg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2xmxdqkil.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2mxwnnhex.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2psmzclpb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wbzmmfwn.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2hhoqtjfk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2pgebrxfa.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2zojqrqok.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2kvoiirik.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2etxcaxve.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zgjghjwz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2smrazgvh.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wwhsumhb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2lmkdarwh.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2npqkqrhh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2lfcgdabw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2ibwshqkb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2kwsosadr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2efyfeirf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2awraimdb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2puntmtbs.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2smwfgbie.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2aeilfxeu.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2asktgtai.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mrgtuucx.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2yhrzdrqy.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2bbwqyhfa.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pjcivbes.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2fjgsjihe.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2mgzyvujv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2fqpuefvj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2jvvhyeuo.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2zkaarxwv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2nfjjlhja.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2nnzizggm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2akpdrxdr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yfzmxvjl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2edtheqkg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ptqzcqqf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2njrivcko.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2jcuvuiie.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2owsrrkaw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2pdoukfwb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2vdvjnbqd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jmmjbdxt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dtieinnj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mlfwqjnq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2vllmiqnj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2dfvjzqpn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2iyqjvuld.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2esfnyzvv.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2hgtweiep.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2gxzpxbpi.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2fpjbbahh.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2tfiwtgbh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2fihlznch.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2mkearwar.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mzunvsux.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2cphbscbf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xbiipodr.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2qzgtkeqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dbdyzpvm.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2piorezjr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2pjzcbhhp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2pxatiyea.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2rlyyjtqa.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2emcasbvf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2tetdizxp.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2ausyuhbm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2rsmkxwun.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2slazuayf.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2lhoaglhe.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2tmvmozmw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2pbzvgjlc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2rkzpzgcn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2wdfnityx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2yzvroaik.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ehpgnnnw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2zizctgnf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2gzelhmoi.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2gvgfptkb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2omvfomxp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2fezffrtn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2yjgzqsnx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2nysfaaiy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ykjphvtw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2fczujevf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2bxxxungy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2hyvxwcss.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2fyhcnvuk.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2rpxkedpe.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2zffkzmtp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2bkfapwbw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2atlhbrvk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2zmrnebnl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2xsogkqpm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2vbxorczf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2ylwszfqw.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2ekldmwjq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2svemitix.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2batbajqg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2mkaguhkb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2vxyyuzlr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2evbfnpdq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2fddwyfbs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2ccptyyfe.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ioiwvrab.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pnkcdsbl.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vuxnpchb.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2jwidpsxn.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2fqurppwz.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mstcnfxo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2frcoprqc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2lodkfiue.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2hggikqzd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2bafmmpyv.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2pcfivphf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2lrhjixab.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2strlzbyw.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2qiudrkdc.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2lhnzrwry.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2fpqtqpsx.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2txmvpznn.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2udybisfu.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2pqixuqkh.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2tcewqaxn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2rihyhdsb.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2ajjtruwi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ifbnqign.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2evtyjbqr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2kobwfphr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2ttfxphtx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2wdkjgmtk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2agaxupmv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nzdvynja.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2yxsdsqrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qbipstjv.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2xkaczpxy.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2awuffnjx.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2nxntdatt.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gdkrzwok.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2msrlskes.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2dcyrvafl.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2otyzxcee.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2fohhthap.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2zquudzkx.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2rzawvvtp.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kffpdogn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2jyknjtxz.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2pxbekkks.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2vsxkaump.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lddbrtrh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tebbcznp.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2nancimvp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fckomgvq.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2cxbavozl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2ucqqqbdw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2kpojyvgt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2nswgzodi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dfzebexk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ivifzmzv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2icoqnyzh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2nlamituc.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2zhabbuuu.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2xinjlxen.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2urzvhaab.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ycahgedc.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gxymymph.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ifldvamu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2cauhdhnr.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pyxquoxt.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2dhmmkgil.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2hisbcqsa.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2nlljwnkd.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cvwvzetg.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2uixxnkxw.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yelsbyib.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qxbmlwxf.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fwjvkkwh.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ytdccyzi.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2czhuftoa.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2mgemaxip.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2idmlaljc.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2poglnjjs.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2oaksgbxu.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2kduwhaoe.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2spiaccos.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qlrrlqcb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2exjcfvlw.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2zwetjecf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2rvxejuuv.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2xxirilpz.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2otrptney.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2xzmqodes.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jjuykzwi.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2mkvelngi.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ovqofyfz.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2jtgvqtsi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2gzoxixkd.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2dpkxfmid.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2awagyqud.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2qsdsirww.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2doueyjpr.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2vyilieox.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2cvuupzif.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2aidmklsc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2fpulayuv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2xbizaxmj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2yfrvobvk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hjcsrtlf.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ugvbwyfd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gzhygddj.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2jagtikfl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jsvmklmj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2obwxcltv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tpusjreh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fwetvvgm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bhnqmsuz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gvfehyjl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2pbiclank.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mferiyst.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2mhwjcjta.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xlqrwewz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zxjfenuc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2tbvcwioj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2wsbiulma.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2cerhsxly.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xnahoget.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2jpmirhmm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bxaskxka.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2cyablgnx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2gazrrrsg.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2nduxmbvz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2xlksrmak.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2xfidntbg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2bavqnqns.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2bfazmnoc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2mnfiosjj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2kqnwnuhf.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2rkbnfugm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2opmspuxk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2dgbohkev.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hfcpdzii.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ijmzoobz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2cfaveuea.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2bzgwukaq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2coxospwk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xdsgzqmn.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2asmotgrj.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2zfiahjpu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2rfpfuemj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqsgmnzi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnvdyclo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2bvdwsbgt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2mvsxbtiu.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yqsevoac.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2dprfyygj.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2cwbbkhff.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2mvhfoyah.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2egocxmya.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ltupwbbm.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sxcmuumn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2wgojbhoe.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2qxnppepp.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2bkjsnkzr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2byfysxen.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2snkkpbmx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2ppkhgtlm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ydpntvyb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2zgztmzpe.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2phryudxa.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2gowvlrjz.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2moxbqbov.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2rqevbkna.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2qenjicrj.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2vluhutsz.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rpexhlgz.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2rwqdwkme.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mntndndj.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xwjlkoak.html


<!-- 参考信息 -->