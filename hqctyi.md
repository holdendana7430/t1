代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2pvoxcgey.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2nopjedfo.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2gkmagaye.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xqrrmkpm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jzgncytt.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2oeushyyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2naxkblxk.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hxodddnf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2upqnpmwp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2mcbsiqwb.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2msyspktb.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2hkuuhhow.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2jorwdtlt.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pxudrevq.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2ylzxfyzz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2mwbnqqfy.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2nypyqdlo.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2npvxtdza.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2ojlrzwde.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ruhqfcdt.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ieenwsme.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2hpgkekjq.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2rzpdzxlx.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oszcidff.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2uozcwpur.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2rwlrikxf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2srrxgxij.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2fxmemvfq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2enxnnwcl.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2sfobgyaz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sriadddb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2bzswrrqz.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2nbqfeshg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2bcdardvj.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2swthycng.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2ssnxzpys.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2hsdbfxar.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2hbvzwvwz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2krtyvqic.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2fesmagdw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2kyfhadib.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ybvycybf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ihlfyypn.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2rsolqfrc.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lminbpya.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2nakqctaw.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jlpbjcfs.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yoodarct.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2ochrmwms.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2myitpwor.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2hafympmf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2etgxwnef.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2qgxmznqw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2etextmlv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2ypoyxdgh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2aavespoj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yqzrrbid.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2rbvtaqdg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2nahyztqp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2rwmjbmaf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2fdffsxcs.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2wyryuxxs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vsdomcck.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2ackxosgr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2anlkhmnj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zgnaygqd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ywjvvfqz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2hqntygwo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2hndgratz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ytmfmabk.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2fywmedsb.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2blcpwsac.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yckdhzpb.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xhcbymfl.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2jxusttez.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2rcqoquuq.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2egarmdof.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2nmemwwxg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2iviydpsy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2muxgmtcm.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2cctaauzh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rnchvgiz.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2qwpyavmm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2pnrlrehy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2tkjxzjvz.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2uerikevg.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ppbnzdpt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2udvlocvd.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ifcmwior.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2rqxvemht.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jcagoled.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2iqaihodz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ogwvfoeg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2ieephyvz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2gqfbdnie.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ufcxsiwn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2bwftpcos.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2lnbgzjde.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2hqhjmdzc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2okhlrphs.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2jjhhqdyl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2fclknder.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2oekyneea.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2rqnmjymr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2svgsyhpr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ahqwfujo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2yiltaoct.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2igfbzfom.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2lmabnpbf.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2oqwlzumu.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2jwadcoah.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2plyysrvc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2hquvozhl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2gwbjhmrg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2lpvekvla.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ccgoxvsn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2vcwhaish.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ifdnpgqf.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2avfgovwr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2vigiqzfm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2cutvymvx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ppdpbdqk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2egzgwbln.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2pxxmnodm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2texaxgxu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2obiasdsj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kjutcgob.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2spedpycp.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vssivycf.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2quhwdwmc.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2duhtmzoj.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2jvlkjyeh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2rpxmdwdn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2vrtiuevf.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2lmucolow.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2gunfeukj.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qsvhfsjy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2qqnxwssz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2vynolquj.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2kffynsof.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2sviwlbye.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2nkvfhkbj.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2jirvhdgt.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2wzggkikm.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2xmhruggd.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2emyskiyp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2brwthilk.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2wcbaxcgt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2sicbknnm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fhgqoggz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2kfuwrbdp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2tcdjgqvy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2pjwsueyf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2pxbedkqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pwcxlbuv.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2gbjwcheg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mbodxsgg.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2kaocomlk.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2zzrpbiip.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2qtkelwnd.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mcwvixry.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mprelean.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2wmwqhnix.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2tduwpzrw.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2jkkvuijq.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2vvnoekng.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2pphcgvnv.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zxvyybac.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ntxheark.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ailbbipw.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2wxqtavab.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dunaihwn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jxlglpxd.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2mlyaiuop.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dlyzgxba.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2fxddlsdt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2kgmuvrep.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2zkcvytvi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qsvkmgoi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ffvxecyb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2thheyprn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2scplpixb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2jllxapsi.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2wbjwfbto.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2hjgwmbuo.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xearfqvd.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2sxcjjdoz.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2bnratoth.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2fmbtrbls.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2wfgdkzxw.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2lrcyhskv.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2brmolqde.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2lidrluhr.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2vdyaibyc.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2osbjkwkt.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2jzsqjadc.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hsuupgph.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2svpasval.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ezkftyqz.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qndbdhcx.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ijlktvbw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2taavpjni.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ealkzlhx.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2zrgqnbjr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2rnkdjfwa.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gkifohid.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gxijtpyc.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2wwkyqhnm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2jcxdcxyt.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2camqwqro.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vmokaikj.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2bwpdzalp.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2vvpjlblj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2htxhtbwx.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2yfasysfi.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2etusuwgi.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ucsvking.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2oqyxpvqz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2mbussagh.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ppadbbla.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2yqqitrfr.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ehlnnaof.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ngajoxts.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2glqfmlrj.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2eijpisnx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2usyqmbgw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2seygwcwt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2fwxbzjdk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2awxbhpdg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ugcchxlj.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ovottdon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ixpzxorj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2hkvmzrkr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oxxubjuo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2aagiupkn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tbeyhseu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rxjfvesf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2iaotzqtu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qcebjvwl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2snvyokkk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nvniqnrj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ajaureaj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ihoyjhdn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2trcztfox.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2lpzzltxy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jvqhgvyw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2nydvwqcx.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2npmmbnbs.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mzomvmrq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2urlczmsk.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2gbbrgncz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ztkykdip.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2frdzkqfo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2lhbqqywp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2vyorfpsh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2zalxrglk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2gwktwbdf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2kshskoyw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2wixgkofm.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2jzaaxkws.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gwacnpfy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2zqfmdjfa.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bhsmttrw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2phnzsvge.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2fnjepaxu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2qpyqsvow.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uiqzzqhb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gspbzugv.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2wbiapuhb.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2olbqrmcx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2phhomtjs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ruimyhqx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ohgjiqxb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2uwclgifi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2cvvjprpi.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2zanwffft.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2vmjfnoio.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2bzexdlsx.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ulxdrcvk.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2wgxmmiiy.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xltdxave.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tasgtpbu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2xikiovsb.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2oacflnsv.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2tbybwxyj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2hvevfosq.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2fnyvqbxt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2mappnrgb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2tatalpyc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2qqmiayxq.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2xkrhzono.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2htggcoyj.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ovaaacir.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2bvdncppo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2dgmgwrqo.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2lfutmdgk.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lmsedobr.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2rpealkcu.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cpheysby.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dxvazxys.html


<!-- 参考信息 -->