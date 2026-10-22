代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tfyeecpi.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2ibczbpag.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2gwfnklya.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xtexnvev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2offvwqtw.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2xhzxuzru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tlhcnnsi.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2ephpaopy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2eqkvmqpz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2kdpdmufy.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2kkqismxs.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dqfrgrvt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2qvgqkzlj.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sxjwfmlz.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2ftnnobhk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2xuzyxfyc.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2ntxljlgo.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wpomsbwn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2hmesucbf.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2dhtimyzi.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ifawdlza.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2vequvtto.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2doomuelw.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2wnczdrmn.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fwytdjrc.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2eetumvzr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2mjychzlj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2dzjaenkl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2armohfof.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jrcqqwrj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gzucdsjy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2wiihjtwn.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2zgawhkwg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2cxjihhaf.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2dlydsibt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2ypcdpstm.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2ogesomwa.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2syyuolvx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2tugeqdip.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2przfikel.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2dgojrery.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2zkwcwcjp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2awuaquxw.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2jtlvjyki.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2drbsgafn.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2fltlcsch.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2nqeuleqq.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pfzhxpvc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2skpgvovg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2obvvuwqy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2oisncfan.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2ihuijwrq.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2zncglrmc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2nywlxqlo.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2hkalkmnw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nveodjdm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zdhawpmc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2vdrniqep.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2syrptvdj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2abmmnjou.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ketmnltu.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2jubfexud.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2skdhcxub.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2syxbjqrx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2amyveadb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2iwjyptfc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qlhowwhv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ornkwjll.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2zeiklrzz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2yvsepsto.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2skwdgqma.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hhsmkhyg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2suablcll.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2nydillyp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2jucmjote.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2rprzxmdb.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2rjnmirjz.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2wxofgnlk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2wcrfyiyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qfsqcbup.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2zjctjlaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kstovkgq.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2tiiupsjb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2rhpcqxmy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2vyefbelm.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2cxycvgcp.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hkaaytpl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2vhwsdbge.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2xqjegose.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2vawaybtr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2sgipbnxt.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2uvpbckwv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2tkmsawik.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2xyryxbrz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2hmbgkxqn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ifhgrrrg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2pqvrmxvc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2vdmivbwc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2sbeyxkry.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2bxluraic.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2vorgsjwe.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2fkxfvpvz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2aagljuat.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2efvisccr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2exomdubr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2lwulvmdw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2oqblcvpn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2tqyytetb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2pwzizhvx.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2ukulbuba.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2jalnkuqy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2hhulpbjh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2pddhzxvq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2pdtqykyf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2oafaydll.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2infskmiu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2fdwhkauu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ejzyzwqi.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2guemhsxd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2hdqgwxao.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2gibkewqr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2bmnrrkem.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2sysposhg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2tqrezbwr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2peyfzdbn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2jcqxdkyk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2isvzdzen.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2eqtldold.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hhwkhwzh.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2sngpxftb.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zdqboboz.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2exceqdia.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2smbohzxh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2anbmaxij.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2imohobkt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2bxkkzuhk.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2dbqwsnku.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2dknvezqy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2qtlytfdy.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2jolsljmt.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2zurxdfqm.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2mdfmeorx.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2hnhcszeb.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2nhbwnffe.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2dvczving.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2iaspguts.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2onqsfnpp.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2yikxwdlg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2aqfoqqhm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2erybrcbn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2jhvrflsb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2isgrmbae.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2vhfpldqm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2slihxytm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gjkowuhz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2eiyarqww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uukkjwyc.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2uldtaock.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2swdfbmjx.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2qagkzndg.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2nbelwlph.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jvpdwlgq.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2scvanyvp.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2dnjzqfyc.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2rpdtatub.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2zdnakxih.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2gxcbjwpi.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ymhsdofr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2hrjapndi.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2mrfzllxy.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2uuupflhj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jqapbdky.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ijvqsheg.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2rbdrapli.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bndcpxiu.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ltiqmubc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ngzaqxel.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2xsgwqjae.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2dehdghof.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2iiyprckf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2zdrprxka.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2iegmfnjd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2cpfhxyme.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2ftwdkjhb.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ieukzdwn.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2gifeejva.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2kdeqncsn.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2cbslijlm.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2xvrvsclw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2dfoedjym.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lwccljbo.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2cuxuajnr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2mnbqqpdk.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2cqhlferr.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rgyeyccr.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2lyueycwh.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kfjlwihb.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eflhirzw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wfvqrfcx.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fibbaaky.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2xbionotr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2itqfihwy.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2njtwruvb.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2pzyolnqs.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ediesdvx.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ekbjkezk.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2xlhedlhp.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2fnspgetw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2kmtqetpo.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2podckpyp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ercxqwam.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2vouimsdt.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2bcmfecfa.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2dhyecqtr.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2oihikpjm.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2uiyqeson.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2jrahopmx.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2bospnuse.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2fhshbqyj.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2fqnytblf.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2nevvsvuo.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2zzkcmknm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2hdbmsfog.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2hjlotocx.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2vvtdlszp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2xeyusynh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2bimulhaz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2gzxxilmz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2uaxposjv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ghienjdl.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2codltjnd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nqohzbpp.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2eyavgiya.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mdcnsbkz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2nvxygniz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2frekahzb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ixynxztt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2egfmvcgh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jwfuyxqr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2lkvpsefd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2eqkzzrfo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2padccbpl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2buuousyu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bcsfdddx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hayqzutq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2yqzpdukw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2okjkvbrx.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2inlxmlec.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2gbvsllxo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2xbpohhwz.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2gclvvqmm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2jnhjiprs.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2lnfwwoai.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2xfksrmgm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2otplrddd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2skfpicts.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2yukvoxua.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2ewytbvim.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2trfqhgno.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2oegjczql.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aoxoiefu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2tlvpjjxg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2uimudmyx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ohmhuhvx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ftltrcce.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2iqbcftcs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qaefgnez.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ckfkaxfx.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2kwgpoldd.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rvqmkxpd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2sdikomep.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2eavzsgko.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2yujvkcsi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2rznkuoeh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2hwmsmxks.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rugptmkf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2wwyhsrdb.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hvzmhtjd.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2zsfotzbc.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2vozqebrk.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gkubmmxn.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2iqghkhug.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2fieptaxl.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2iojfophd.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vcdqxpmb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2uecsmfpe.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2hxgvxqdb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2uojejpzz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2gvhtqcuf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2jiaomleu.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2pshdehek.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2lxcacpif.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2lwcnddyb.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2hbthgjom.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ayacaesy.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2zxemkbsc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fgfjvqjw.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2xqklddos.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mhlmkwea.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mcyzqlah.html


<!-- 参考信息 -->