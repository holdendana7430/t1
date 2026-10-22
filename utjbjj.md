代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2jjbyhkgd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2gifxebaa.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2xfbgxzzy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2dwodirng.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2atdpxgbr.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2cavgevlc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2otgmbsyk.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xxrgdjpq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2cfknbgdv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2fxzznlfl.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2btjagbzz.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2teosukwc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2etnhagkv.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2wmtnvdje.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2pnhjfreq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2gykunckb.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2ksalxynq.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uqxhpmcy.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2zlvoaevn.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2stpxnrjc.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2anbpwhwj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zfcgyvue.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2waunzulp.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2sydhiwur.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wxqbfane.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2qejsexgg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2bkkuswuj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2cszyikqi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uzuipcif.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dtqglkyv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2jcnakhxn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2xxmvuoao.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2owtxkqid.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2ntdzhbfb.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2bucxdpvq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2epucaevt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2vklqcuos.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2phimtgld.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2yoxgiscv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2vlfcynio.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2akgqzpsz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ltqhmuik.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ovydzcog.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2whedjtrm.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2ksgxflyx.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2zwpxipbk.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2mqfagwac.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dmclpxbq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2uqeyspga.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2zqqwijfj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2bpokaugz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2tyvvpzon.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2rynwbvjt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2aqnibsum.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2mkosxuie.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yiffirtm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ewxoujyv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2voxvmdaw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2julxfixd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2qjpakszh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2qehhpbhb.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2jomnddfc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2snvjqiyo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2egyfqppj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2avfqmdwx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hklaqdgh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rvguzsxe.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ofccterp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2rcyoymhh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fzgaagrw.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2ltsbupdw.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bakdmoue.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2gbkeaygc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2uegnhxle.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2rxxesmyh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2wwswdqfj.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2gmkcqjym.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nugfetll.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2xpjitoiu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lsxqyovq.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2vqdyrihc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2peivgvyz.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2uszxyknu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2aslfjsus.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2ibcgiiet.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2mmaseeib.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2fngildkk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2vhvwnuve.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2vbezlotg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2ttpwssfm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2ziddqbai.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2xlffkyng.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ticonuqm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2bosysqbm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2oeahjijd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2jrijrtvu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2jebeeiwe.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2etnbjebu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2utvtpvft.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2hsdkzhac.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2lxxglebz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2uaahfsjj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2sfrvfwfb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2mxlcjpws.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2xmhpmaqu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2usjnhqgo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2xaiogtkb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2cnunxmtf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2lnopdnho.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2ajnafjis.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2apvqjjaa.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2onqnmjrf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2mqglwhoq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ytnlelmr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ojixntso.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2hglcdvvi.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2hxpnrupn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2wrkzhyrn.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2eqyehbjy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2qbsafgxw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2mnutoccq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2nwkhhyfs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2argzypad.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2kyytptpr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2rnbhwomy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2vpcfxhlk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tuatjhga.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kqxnfmwc.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2boalkmbo.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ladvbpna.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zwnoelww.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2gnatefkb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2kgxbmgct.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2sweoworm.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2zlchttjs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2guwrehzr.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zxyltjja.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2zqvsgitw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2etojnrrg.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2fvwujmxj.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2wualupcr.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2yfycmsyv.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2fketlxht.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2fulyguzk.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ueijxyeg.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2etakuiwc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2cvmfcrxt.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2qaxmfbaw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qbrrvxde.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2bnbxddxk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2hbzedbso.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2pmpwoxdw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2iavrrnxp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zuvhgmer.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2whmjijly.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2tjiragov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2isbkvrwv.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2izcphtrz.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2tlhnewqe.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2owtejmws.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2asghrdpp.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2iweorfkp.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ilxjsufs.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vyljcvrj.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2zafimmlg.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2oqldlded.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2reisodmr.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wttsxtdy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2yrpggauo.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2npkyidei.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2hzcweiqs.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hoztvtqg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vxatphnn.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2yehbndbj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nmccejak.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2iwwujvmc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2sxntilhm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2uqvktili.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lapzgbag.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zhtfhpjx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2wxflufbw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2rotuuggs.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2vctlalaw.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2uagbbewi.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2gzjyyzmb.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2wesaemhk.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ytiiylty.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2zhssyefy.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fytiqwxi.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2qhgjayiy.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lfogtbin.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2nauxflul.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2iftmmfbu.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2jhggyjjf.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mavndzkd.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2opvzjrka.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2skdnochy.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mbuynnbv.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gpzsjjnn.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sjhqngwb.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ylqaqanh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2vuoebrrj.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2zyxasneo.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ijzbaeui.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2thvzbher.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vwrfhfll.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lqzrmaxf.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2cthuwfyu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2pjnfajes.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2aygyhhjw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2sfbutolt.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2phfgnoxg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2yzdktddu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2anfmvlds.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2hziiziwo.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2dhuxfwux.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2zcpiutap.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2mwwaglmk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2sejmncsn.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2rsfdosdo.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2bktplmeh.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2urihkjxg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2xxmuqfph.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2doftzmbb.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xbwzkypb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ggicystq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2acythezk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2lviqfsaa.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2cdnjsuch.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zwjjkjeo.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ezcohjbt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2crmhraip.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2qhpgdmyj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xvpphmxk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ssjaetui.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zcsbbdgl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zrysldlz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yptlskuw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jxbcwuje.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2fhtusjly.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cyjxttbr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2uglrlitc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2yarcikrq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cucirovu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jkuewdmq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fwuvzadj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2rzcvhsur.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2nnnjhmln.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ajrajeux.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2konpzjyl.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2ivfemuel.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2mxssgwuc.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2cecukgbq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2llinvseg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2mvruxrfr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2fltxxgfe.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2qrrumrmg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2kbutannu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2aykrcthe.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2hkmdkwtn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ozdlokow.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2pebuboib.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2aqmkkdph.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wqusbfcg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ypfhddcn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2qohpqsxc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2vjyfemkm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2prhvfwqm.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2micaqpfm.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2fqbvkmir.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2vblkewaw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzmkyuok.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnkodtnn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2hdydghne.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2zonjejtj.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qxymubfc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2hcwvxgsz.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2shjmveyo.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2qbtmrdid.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2yzwjhgmi.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hcfyxlhn.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oecuevtz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2lvagzewh.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2oslyzrnw.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2hzvwjrpx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ikmgqujt.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2zqfguwfz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2utvktowz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2gyqhrzsj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2wwgevwta.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2uwhmgwzm.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ckiahasm.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2uzsizadl.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2jthbbbqd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2pqofghcp.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2symghzzp.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xxylylvs.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2vaslmycb.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wayhwlhu.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rpduzxzy.html


<!-- 参考信息 -->