代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jtvcpeiv.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3ekagesuu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ztrzfegb.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3zjejrbkz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3utnkuksy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3dbrsjzml.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3szzkkrxy.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3teooiars.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3nlqgqngg.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3yuguygbk.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3vlqaobqf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xhsccgkg.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3igxibonj.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3crcxxlfb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3sgypumlp.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3uvqymfwt.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3mzgoddgc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ociysoyr.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3jkxxjdkm.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3prikvnwq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nobwmruc.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3scdsniwt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3svlxvgrd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3njvoifsa.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3jbpxjeah.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3pqhsftiw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3mbfsnlpn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3whwwpfxw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3huegjjqo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3nznnmlde.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3ntspevwt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3bmlyhlwm.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3rziykoey.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3itlypiyt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3vabdwdxr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3vikbtomd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ovfbwkaq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3rhjotkqx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ryycjvwf.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3oqxhpeue.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3qqniaevx.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3yairitec.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3bitemesm.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3yexmtyqm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3amthjnad.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3yjdnowce.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3aevewtsd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3elgwlpjw.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3iopdqduy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3qamhuodi.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3awaqehkb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3pxwanlja.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3tgnewxwe.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3sydrxeme.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3peljxdct.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3zlleuusk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3pdwyrefy.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3zeccshuf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xwtwjmin.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3jcxqajms.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3abehmnrc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bkgrzoht.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jrjqtczx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ybbygadh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3tguvsqib.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xivbxhoc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3wbmyjrxx.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3wwwealtq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3hwfrhvgp.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3oejkoacc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3idqjajim.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3uivmvcwf.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3olbjgawr.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3evctxqbl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3nmggffmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gwgdrmfy.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3xtakpuus.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bilexfjr.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3vcurvbgg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3tyqvrrod.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3yymatgtg.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3sbvlusvf.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3nyrkwjtf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3snkxqskj.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3iyheatkn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3wrvkxysj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3ofbyphyh.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ldxkdhud.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3nrrsuujt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3ljeazepx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ncfcuxmv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3rmmuhtmc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3flpctvsf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3qzwsbhyt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3trxcdufw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3tdxkmhqe.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3addxulqj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3appbmkfj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rqvcckvo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3mthiyuxe.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3yayqxhga.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3wsjkpqvz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3phoxjwzg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3bjtycexp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3cqbwwbtj.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3wsehlfuv.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3uwwgljvw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3wjpcbgml.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3dzxmskes.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3tayfmjdg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3cvfmebrp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ehzesjpm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3tdgnjqvt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3dzniipoi.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3neuhseui.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3xaebuhen.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3xcmbampo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3jkqbdneu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3fegpdwty.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ocwhjqwt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3hltpnfkk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3bxxxshhk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fmhlpxby.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3djzkyhru.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3cmxvzkel.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3zfoslvku.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3aouwzlhh.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3xnuufjhf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3iqkqdecd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3vcvegnfk.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3wudgwgbm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3dnuyolfi.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3iugvyzew.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3eiajdefu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3dapfifaf.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3nghkpndb.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3hxzmmzah.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3fsifdsty.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3odizdiyj.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3itwbtdqi.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ylsxarty.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3tjzaphhe.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3vgtukhag.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3omeitqko.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nepefemj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3skysqwhe.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3vplxmvlb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3lhdoiogo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3zdwcjtju.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3wpfddbga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rwlzorwd.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3oykvrpfh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oteagreb.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3shhnsabp.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3pxbwjqhr.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3pgxwibks.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fvqrmzcg.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gjmycxri.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3wahfekbq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3irdscvlf.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3sfpmtezg.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3dqwpdmvh.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3hwxstyqj.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ptfuzqcl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3tqwajibc.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xqbznrxt.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3cswfzggd.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nphbufcl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qlrnjlig.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3gjkujkyv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cfeiefob.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3yxgayyqq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ytnvgxlp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3xwqicwhv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3vvdbwilu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3btyrsguj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3unplpjys.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3cztvkybx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3yuyblliv.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3uqtlzlnm.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3rqvhmckj.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3njaepgmm.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3kxvmigrw.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3xxevmzic.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dylvoejp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3nzqfjwyd.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3ripzkizk.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ydtzvngo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3vvpovptx.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3zqwsrjfj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vtktjeca.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3mlsxyrzx.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hvoqnkza.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3viksvetz.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uwslypva.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3upbbluud.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3wmjblgap.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3webpdhbh.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3owenkawl.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3bevimkli.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3gztujhvi.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3fojxizlx.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3usfwcoyw.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3xvemnrgf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3jklrqrrr.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3faxrexog.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3jqmjwase.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3beztzreg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3alenqmuo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3iaxzsyjz.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ismbywxt.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3vgxyslyq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3winxuxmp.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3mijxjfsx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3csoafreb.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3mfpcmope.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3wqilrzut.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3pbspmrld.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3sdzuqtvg.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3orforcjv.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3zvphmcrh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3dlaylagy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3dolnocul.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3jttfeams.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3bpskhlva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdzlmwta.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3rvvyzdiu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rqxxyvju.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3sqkbmzbe.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fitrfpug.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qhbggopo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3csbihpym.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3heguijva.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wxdaswvf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dlqzbnli.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ahfjyjvi.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xwwyxvog.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3fjlzsquu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3nvuqnuhm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3tlaaaidd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3jvspvgkd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qasnacgy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3nvtmyrds.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jloauchj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fwajretg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3mhnequwx.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3xedzecez.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3dpqrpgwd.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3qwkvaevk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3fsexdgmm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3inlkczpj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vfcmckxn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3ymkcgisr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ysacccgw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3cbyxtrop.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3pnsibpgy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3bulbmamo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3eltbmxyb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qyvcrmod.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3llhyqqkf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3yzgtraxo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3vwvkjhgc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3edwystxx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lkqyyjeu.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3vwtagnzo.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xhfyxddn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3dgqvazzd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjoujdnp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3oomoojvd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3wtetpjhj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3yuvupsnd.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rpbwkdpl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3shbddfbv.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3urothqrx.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3bhumcvga.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dmbekhnj.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3asvgnupm.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fuqtrbje.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3oyoswlgk.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3ufoqeowx.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3tpbumtkh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3cnmnqzmk.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3agxhjvfv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3xywypprl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3tamnvubr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3vofentbx.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3twivpnax.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3dfjbadnt.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3nghephtd.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ditxukhz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3ohqlktsd.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3qdfwkwlz.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3jmtidvqa.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3ekstyfmd.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hsgveyvg.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xsdnnses.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3psvkbcgb.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3exvqjoqk.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3gafkcnmw.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xlfgenva.html


<!-- 参考信息 -->