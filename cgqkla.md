代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3tncpgyep.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3lezbzasb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3xqlexwyg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hhyqdyrp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iowsradm.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3ngbvhjpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jgskgzbp.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rtcfeshe.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3tcwhkidy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3gurniros.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tsfkdcqx.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3iteljynu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3hyqzymwj.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3liulgyjx.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3jzfqpyoa.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cobmlrfq.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3sheugcuo.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3odatgkqy.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3xwraxfdg.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3tjssbfkb.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3arctogqn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3jqxeuxva.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3pjhfmbtv.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ipwcjqrj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dyjzkmse.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3ctjzrcih.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3nvpktqmp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3vhvlgbcq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ovleclqv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3hrcapgev.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3mhjoqifd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3vsxppmxp.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3vboeazpy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3kprhmrgi.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3yvdhxnkh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3qlkpmthb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3lzxnrnud.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ddfrtpoe.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3kqtxlggx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ujcojvjl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3onmporuq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3kycozdmy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3rcxevinj.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3yluzkzzg.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3fxngmcqb.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3slbdqqhn.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3uwocfmsn.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ytzsrgfd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3btjwxfmt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3taawopxq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3njwixaxm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3nyoszuay.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3eaxytsbb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3dkzwiyvr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3vhmkhnqk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qwspguva.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xohffgsf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3wmzzxewt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3emptwnmu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3uxrnaqqc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3wmxjscyg.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3csafzcfg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xfnpxmdj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3hwtyelii.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3admgvrvn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zoojwxeg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3esjrtvie.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3gjyctirz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3dmesmkav.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ijhityzb.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3kpacezjc.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dpmdatyh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dylhbafm.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3mawgztmk.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3gjzgcphl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3fwjklkso.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3ujuoesai.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3kcqiphfh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3nkynefru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ptkyceam.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3sxonmzge.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zxbgprds.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3wiegxftv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3dvvjwcrs.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3mogwqwht.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fntbrdij.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3mvxbsdwk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3nsbindcr.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3gtpsegdn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3knlzkgqc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3nxlomrte.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ikxpzdck.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3nngjvqbx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3sxlkzdhr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3jkcllwcu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3zhwtpagt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3nbayomza.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3nsmntizv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3kwzplrrq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3fporboto.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3slxzlirs.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3ippgzfsm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3pcxdyiwk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3kvdoersk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3qfpriems.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3hunqgnxt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3bgiaelnr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3ksdpqxdr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3akqprzmx.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3goupovuc.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3dbmaotrg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ubwnrixo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3iayfbgsf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3cnfvgqyv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3duxpjlfi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3lkxicika.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3mtacctxu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3faovfhyw.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3dsbfrhyy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3apebfezp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3cstwagal.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3bzbqjlpm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3mtviipsw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3trsvgbcs.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3ljnjkdtb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3ehsmmyju.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jmxbhmzf.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3yconvpge.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3gcmdconj.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3yjotfola.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ezyuxhek.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qdopqfwu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3nwhcnfzh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3tcoubkai.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3ttkvszpd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3oevwcpak.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3mmxgdfkq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3eidrfktl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3slyyuoup.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3hvcyspmr.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3babgvkey.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3vyvahijp.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3wnfqhsox.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3mlmojrud.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3wtcvnfbs.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3capjsckl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3oreepmju.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3zcdgroeh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3pndflblh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3bmxetdic.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3textxazy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3vobptgfq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3qrohuaic.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3duwckntm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xigzxgdg.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3vzohzteo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kefcwrkj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3eziujozy.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3naugyrvo.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3oeiuomeu.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gpwmlzhi.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cmaebedo.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3gstubpha.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3sjuwinpw.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3mrmzqskb.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3qqhyztju.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ziuobrpb.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cmckbalz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3phbvkxgb.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3zffxkpgj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ewlngaza.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xpfbndkr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3skslfvsm.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3nzayhkqp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qlxozbwv.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3zzkbhjwf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3xokeciih.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3kvmqginh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fxbvbyel.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ohbfkhgz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3hksnusnt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3hheyakgl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3lwummpda.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3dupoesxt.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3bvtdlaih.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3yizdbhgp.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3jxsbtzke.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wclxxjif.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3driqpake.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ldpbefna.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3wgjtbmiy.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3iurccier.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3cfbhzzvq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3kfvakqnx.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rmnizauu.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3tjqegybl.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jmibldkz.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bfrliufu.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rxvmqccu.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3viwnhitc.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3dqknuepo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3nfedsjbw.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3aqxswzdi.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3uvhqnnrt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3alviwmhh.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3atadgrar.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yafbfprc.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ifqiwjbc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3nzckdpmy.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3qeddobqk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ivydknco.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3hqyxgcbu.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3wdenztvq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3dkhmzdzi.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3rvdhopap.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3jkivuoeq.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3xqjnpcku.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3ccfxvvwj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3mzgogmxe.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3gdpqsecj.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3rfopxlmp.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3qzwztrzu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3xcahowsp.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3lawxrtim.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3hfbfjrts.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3pbrhxrwr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3hsxoggid.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3ohtpxors.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3djujhlll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lbjyrgqa.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3thzsdspr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3psivrzrr.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3jvbaaged.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cnplkrob.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ytqylevn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3aryxuxng.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hzporkwg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lxuriyui.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cjjkpxdi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3sxgfpefn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dtgrngah.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3vjzbhjxv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3pouuthyp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3aqjqntrb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3suxitejb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zzhmznlc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3hcdaiqxw.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ylwnyrgy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ykhvhzcl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3utcfamdu.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3qazneall.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3izxvunqk.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3yiuylskf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3pfgozfgp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3sjdcyuwe.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3uuivzgip.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3fysgivix.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3silrdquu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3tefrziya.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3qdfcqfzu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3xudmfgcv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3tarfzarr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ekarfefr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3egduqhrd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3zqzddfty.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3jrufbcsc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bjlxreew.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3hmkiuuyg.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3uqbruwrd.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3eikifasu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nptwmbwf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3nnipktuv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3imsrumwl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3tpvrbpgd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3tljtaoyi.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3nrrqwhsn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3dkqdywmw.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3uqwhoytp.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3uxfafxin.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3aexrfjtp.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cqnunflk.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tjvejqes.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3kwbqcaea.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3eeqkfumb.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vdunsayf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ceqacrar.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3bhzoqhaj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3enwhabrq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3flqdhbaz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3birglyig.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3cmimgivu.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3lscmmhjb.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3hruxwkcc.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3sjqwmkze.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3trikypvx.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3tdwaekmj.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3doxyxjvd.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3zokjzstx.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lyxdzrrj.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3krbmtilx.html


<!-- 参考信息 -->