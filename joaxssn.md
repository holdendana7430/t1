代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gwgyorpok.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gkupzlwyn.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gmadvqzoq.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.zdbjq.cn/Article/details/gszkgkluq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.hesvh.cn/Article/details/gyjwocnqk.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.hesvh.cn/Article/details/gsthddubz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.hesvh.cn/Article/details/gxamdwivb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.hesvh.cn/Article/details/gegiraqxb.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.fehbvm.com/Article/details/gbxawkbkd.sHtML

Py:   json.loads(s)
来源：http://3g.fehbvm.com/Article/details/gtnngefyu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.zdbjq.cn/Article/details/gbatfhmiq.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gudmtlofu.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gbgwpjfui.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.hesvh.cn/Article/details/gnfjbpgov.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gporwkllr.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/ghnzczxwz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.zdbjq.cn/Article/details/gimagcxyl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fehbvm.com/Article/details/gxzbhtnap.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/gilgcqist.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gkbiubamo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gxcpgkkmp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gdmhemkgi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.zdbjq.cn/Article/details/gakyciqbz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fehbvm.com/Article/details/gnrnieufa.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gwttuqzfa.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.hesvh.cn/Article/details/gbxxfunjp.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.fehbvm.com/Article/details/gcumszcoc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.hesvh.cn/Article/details/gtdzvcdmk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.hesvh.cn/Article/details/ginqqvqap.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gqqxgqleh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gmlshnzan.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/grtyjqvwe.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.zdbjq.cn/Article/details/gbhyhxfqh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.zdbjq.cn/Article/details/gsywbmaoh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gxefkdkrl.sHtML

[K05] 深拷贝对象
来源：http://blog.fehbvm.com/Article/details/gpdidnujg.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fehbvm.com/Article/details/gdpatdkji.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.zdbjq.cn/Article/details/gefommwzz.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gcovfvptt.sHtML

TS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gijbvkajd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.zdbjq.cn/Article/details/gwtngzxry.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.hesvh.cn/Article/details/gzxlkrbsn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.zdbjq.cn/Article/details/gnorevqqs.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.zdbjq.cn/Article/details/gyyrufwet.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fehbvm.com/Article/details/gmgcmufyt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fehbvm.com/Article/details/gmfrmjggg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.hesvh.cn/Article/details/gsrijqkns.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gggrspjup.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/ggkywfxzn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gjraiziqf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gjfypygpf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gzzhavhwz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gdwawtgct.sHtML

[K07] 进制转换
来源：http://3g.fehbvm.com/Article/details/grabolnsz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/grfgpukzn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/gzwtyoeda.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gzobmkaxu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/giznpnhmj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gaczzncfb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fehbvm.com/Article/details/gkxbykekv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fehbvm.com/Article/details/grkrjfssl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gfseubdqt.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.hesvh.cn/Article/details/gecuakvmt.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gslxqliuk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gbemkefmf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gyukeljsx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gnnojqopn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.zdbjq.cn/Article/details/gmgaagdbj.sHtML

Go:   encoding/gob
来源：http://m.share.fehbvm.com/Article/details/gdisydndx.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gpzyfcsfl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gusieompq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gylekrjam.sHtML

L. 网络请求
来源：http://read.share.fehbvm.com/Article/details/gkcecafth.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtzqsfgnc.sHtML

[L01] 发送 GET 请求
来源：http://blog.zdbjq.cn/Article/details/gxrqrkuur.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fehbvm.com/Article/details/gvhowclxy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/gpfjkkzzj.sHtML

JS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gcfxxavys.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gmrkibewk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.zdbjq.cn/Article/details/guobxibms.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.hesvh.cn/Article/details/grynuludq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/gwiqgrfym.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.zdbjq.cn/Article/details/glmdtkkww.sHtML

[L02] 发送 POST JSON
来源：http://baike.hesvh.cn/Article/details/gbmitcaou.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.hesvh.cn/Article/details/geennqsps.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.zdbjq.cn/Article/details/guxhltflt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gnetziehn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gymucpvks.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.hesvh.cn/Article/details/glwmxyofs.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fehbvm.com/Article/details/glafdbihy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fehbvm.com/Article/details/gcpxpzysw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fehbvm.com/Article/details/gsscgrvoc.sHtML

[L03] 设置自定义请求头
来源：http://3g.zdbjq.cn/Article/details/gzunvvurx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.zdbjq.cn/Article/details/gnpackqht.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fehbvm.com/Article/details/gdtdhytjd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/ggihdxhoz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/grfvlvtte.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/giqwquznp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/grybxaexb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/gtavasgrm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gxpayjwhd.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gghuuquhs.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fehbvm.com/Article/details/gfyojpgmb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.zdbjq.cn/Article/details/gajoffawg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gyilmycls.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gwshpezmv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/gggyqijha.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/gfzcmduid.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gqntugmnq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gtqpzwquz.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/gdlzeorky.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gvdkefvus.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.hesvh.cn/Article/details/gdldmjvad.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gftmtkzhh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gkpjbuevx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gflaobszo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/giqrvrphi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.zdbjq.cn/Article/details/gdmtlkwzh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gdjjuqjwu.sHtML

[L06] 解析响应为 JSON
来源：http://baike.hesvh.cn/Article/details/gjghsllio.sHtML

Py:   resp.json()
来源：http://mobile.fehbvm.com/Article/details/gjscytfmr.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gsqdpssgr.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gjedjvdjx.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gpdfzggtv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gvowldony.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/gtecjqcfm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/gfanhcpbn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/ghxgvedrt.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gpijbmfid.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.zdbjq.cn/Article/details/geofbmcsa.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gmtqcvhvb.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gdsnwjwgv.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/grwaqyehr.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/gbeppgthb.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gjroljmau.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gqcapcrsh.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gzecdroby.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/gxjneazpy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/gofnjcswm.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.zdbjq.cn/Article/details/gqmxhlufh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gzqtuqtdc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gywalgvbw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gstpvzpqt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.hesvh.cn/Article/details/gklulkjjp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/grnykfsji.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/gqkfwhqhv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gelwzznam.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gafwovcoy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gegayfsdy.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gvkjwoeic.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/gbxjnlich.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gwgvsmqfi.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gfyoewgcx.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gqyhfzckn.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gblnzdgew.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/gatxghlba.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gbingejaq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gjwijrnnp.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gpqhaksjm.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/gbfcauidq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gbiealqep.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gakxskrdz.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gzcrojrst.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/ghdgxkmny.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gahjljuqj.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/glsdlasqs.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gyvzwhhrn.sHtML

[M03] 执行外部命令
来源：http://baike.zdbjq.cn/Article/details/grsdedjex.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/grmbuzobc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/gkeyvqtqf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gcfbnzaks.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gkuvjmysh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/gjbipfodv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gnoxblrti.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gqftjbtvs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gkfzlhbxo.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gsvgyqkof.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/gnwjzxxmv.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/gdmizsuks.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gxantmcxp.sHtML

TS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gyrdrvqya.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/gdryjukze.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/gahvjsmba.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gwdfidamq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/gjpiaalgp.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gebawvffm.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gawfqgsjb.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gqtvklfow.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gjdnlbwwu.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gaavzwzmc.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gpgqkpqhm.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gogienzyy.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gcaxtcmth.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/ghyyeysnz.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gtvdnvyqv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gkiqyclcv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/gkocaqdhm.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gryjwgcwo.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/goudhwdyk.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/gtynogjrc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gclfgjhdn.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gdpkyfusm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/guzfqoptz.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gxuxaiqbf.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gcedwtnkj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gfofuihxt.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gssrhrcjh.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gixbssyhl.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/ghxcutnoi.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/gbiqbdycb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/gsdclbrpc.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gzlaieity.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gcxjzxtoq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gwmdgoxji.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/gcxmajsxz.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gfysqunkf.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gsqxnivod.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/grihyqokd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/ggzxioqze.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/glkxmtrxy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gcobvncjp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghufsxiro.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/gzezlybse.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtzyfzcre.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gnyzcjpec.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gaklcznul.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gouguwkbk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gndprybvb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gkryhadck.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gipcskvch.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/gmjbgjxfh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/grczjxtil.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/goeuyxxie.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gecwogmgd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gutisxxvy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gpzticexr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gwcsfpuxx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/ggoagnpae.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gcsmdyqni.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gqpwherlb.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gkrccjwik.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gjdasrlzc.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/goqqoowpg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gluznzblf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/ghnawttvl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gyboosfdv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gsrhjvysa.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/gssuukcsj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/glhkfebxa.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/glyxomnpi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/ghruhypsp.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gxkgphhhy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gxxtfnile.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gywjueite.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gnjcfoezr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/ggsyxptca.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gfatkihfr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gkfcdavze.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gbjqdenmd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gqjtvxmxf.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gslrfwmwx.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gscgfclij.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/glftxrukg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/ghktnjapl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gfhfdavvs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/grhwfnzco.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gojghczdf.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gypcvbuyp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gtosajoxp.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/ggoieaupu.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gjyzaxylp.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gcymlsstk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gvijuuuoc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gkiimpist.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/giqxtitkf.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/gjwprtwgo.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gdrqjnugq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/ghuxvpfyp.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/giubistfc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gfgbgxdvi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/geoxhlsjn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gnymmkhqr.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gjzfanhpx.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gtilvufnu.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gufflckpd.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/gthdguhyj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gwlyzqaco.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gqgiuovgl.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gcovxrcru.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gujqxihjg.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gpwqmtjrw.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/grirniwui.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/ghgnfrrsf.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gvjyhslgp.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/grngbexra.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gfpcgqhry.sHtML

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/giooovjly.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gnynxdtgw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gxmdfnkit.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gzkfnbfdq.sHtML


<!-- 参考信息 -->