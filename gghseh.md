代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2xqmyqeao.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2mjogogmc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bqyohrhk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2rrwpcluo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2csqlbvpc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2jaecpsye.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2zmicsnft.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kcmtarng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2amdderhm.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2ktwnpvzh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kgzkwcta.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2jkzjvovp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2uxpgnuch.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2jvbvnbra.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xrtbsyuq.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pbbbprxg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2jvojyoiv.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2koqzeina.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2iwwixocu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2ekretlkd.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2fpsqhohz.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sstraseb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2zarhjqfb.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2krkexjib.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wqbhuwjo.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2algxrlor.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ssvdvjxb.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2alhnrnyc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2itdsweoy.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2uuuyqjqg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2knqbvggu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2owtxlvbk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2btpbieyh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2cshbxneu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2tebesimc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2yhielelj.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2ixblugbu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2ydupenjd.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2zdcxevem.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2hqkulhsv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2eegblxjg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2citndqzz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2idsynvon.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ymjsttem.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2skgaayoy.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2hqhrsoul.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2xirgijgz.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2mpsqnuws.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2auexijii.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2oewvfikm.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xdkdhwdw.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2vcyzghjn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2mflasabn.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2uzhfjqqb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2rcgriacu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2agdffqpm.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2nsunzmmi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2dscksios.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2ycfbqsaz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vflyocgx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pzryyeax.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2hgwwhagn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2cbctckkw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2pshqxtne.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2kzwdppff.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2bjnnkscg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yngslvtj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2ldblvxzl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qrujovkx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fzdizgmj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2tohqnrom.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2mkytahcp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2uzfgrixc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zauymhld.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2djoeftbn.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2kthnapxs.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hmaptmla.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2jdztqudh.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2tnfqlbdv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2tcjegxpw.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2bwtrscaj.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bouobmac.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2tlpgezjg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bxsvntst.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2dzfnnxfr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2icliznor.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2weuyiude.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2azplfvgz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2nptlyuug.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2xiktkuah.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2pnkaachm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2rkizkxmu.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2zpjbtsfi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2layyilfy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2uitaerie.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bbbckwsn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2favirojg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2ggazekqx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2cimmyfeq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2btyvxkkd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2maoovutr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2pqtlxrrc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2qnotioow.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2vbtdchws.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2fxhjghrx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2yrkajnkv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2ioqjsvls.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2zlapjhqz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2lbnnamgw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2vfumjehw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2echfroih.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2xmkzydvg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2vsvcfyak.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2dkkjjqlr.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2zzuozdpk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2rcfmqfmy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2mranrwoq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2lnrsuxvk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2qymlvymu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2msuzztui.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2lbpwqhab.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2pzmdubss.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2aknxgcvj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2sxuewtgp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2slwdevjr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2lqzuynet.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2vjrcbgjv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2npebrlkr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2vqtoealn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2prroqutr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rkvcwrbd.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2jrfflkok.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2pdicmmgf.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2bjocqjph.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2rtrharzs.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2khdazyyg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2krfpdcdk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2uwuptsff.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2sdlaautj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2srgbnazz.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jbbafbbc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2prcceigm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2losksfps.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2gjxbbnuu.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2zmlxcepi.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2pbitmkov.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2turanrtf.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2yishhgml.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2tyclxxne.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2kqxerdwc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2zvieedju.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2cfrlcoui.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2oswtlcbb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2dgnzzkie.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2akurciir.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2anpvuyqh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2nhbdfwgv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2bbcpzbjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ipjldqwx.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2xvlvgyel.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lceqjjmz.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2tytlgjpg.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2uyaigdjy.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2nhmkvjau.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2siucxowv.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2itmcyhng.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2xarvvhyh.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2viyuzdce.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2pidobcra.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2pwgkneaw.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ogwocwpv.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2uqlvddlm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2nedqnxtz.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2xxysmlvr.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ddfnwtee.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ewnritnq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yqrjiojo.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2vzxbjjfj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vvfsvznu.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2jirysmvo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2nmeoxhsn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2eybnazit.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kglaukbp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2hdsvjspo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2srndicyp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2inwwzgzl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2fyeilmzs.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2fawhsirj.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2jmhxqgkz.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2mtscciuw.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2qebbpuzn.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2npmpmmte.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2jfhibyqs.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2vfajvaug.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2emanhdln.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2wvtfxqmm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2lzstgbmu.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2qmneqegk.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zmzndlqm.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2ibsnaqru.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gjduedfr.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lefhhhyw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mjaqvvgj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yfsjpppi.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2jmryyddy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2adkmfnjq.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2qdogprsw.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2dpwgnzke.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xpvfguqj.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qewxerht.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mjaoiney.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kxhxcgvs.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2kqleefak.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2wjshmspf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2clexomuh.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ucjaowha.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2xkxkolnq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2lsshjzwp.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2sshfhnzm.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2rtkgmdht.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2imgtnhvf.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2qjiiryig.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2bpgyqjdu.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2glvzwvxw.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2dghavqah.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2aziviata.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2cqscrghs.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2hbqxtvmk.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2qxhuspsz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2llekosjs.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2bgfalnkh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2sntvlync.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2lzlmrite.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2omszvytx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2pmlvouha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sarlohlt.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2jfnwsrdc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nvadffcx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2sfslqtph.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2bkumyuyy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ascdwxkj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jaqnpsyb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2iqahecmh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2rlbhbfak.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wvkansfb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2wbdldtwl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2uaeavvdn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2sdqetkdz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ezqswojr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jtrlvqfe.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2urceojvn.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vlrhvilu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2azfkvyws.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2pmihctrk.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2coakbwxg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2vhpjwemb.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2enkdwyqe.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2snminklf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2bqtjzqti.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zicdqgkk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2utzxghud.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2raffxeuj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2zeormkej.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2rihzxvwo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ogspyqwc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2nsnqcrew.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2fqjmdkmn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ektjshhb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2qfxlpols.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2czqhzsur.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zzcmcymx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2olqaiudp.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2kdznkkjg.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2twabccnd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cwutvrsh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2onxfqaau.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ofjwjfzy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2hhiqqmnm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2dmqsavvi.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2isdvwgrt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2oevvvdea.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2wkxdtqbb.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2rtbiegqq.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zqpjtcdm.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2paxdbxnt.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xsnypnpp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2modkstvw.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2njpbacnh.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2blnswcwo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ghvvfgxg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2kkzajxoe.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2mpqwoffo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2bicphneg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ggvedlyi.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2kaolzlft.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2axrfbidy.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2fgabdfin.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2zjlvixiu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2jvrooaql.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2rfghzgbb.html


<!-- 参考信息 -->