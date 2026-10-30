代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/gkxmafgng.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/ggsbnqkjs.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.zdbjq.cn/Article/details/gzwidszxu.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gudyoqkic.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.hesvh.cn/Article/details/gdcivmxnr.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gwdmuivbc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.hesvh.cn/Article/details/gzzcegfvx.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.zdbjq.cn/Article/details/gyxdrobwg.sHtML

[K02] JSON 字符串转对象
来源：http://blog.zdbjq.cn/Article/details/gkxsmopro.sHtML

Py:   json.loads(s)
来源：http://www.share.zdbjq.cn/Article/details/gzgqrkbtg.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.hesvh.cn/Article/details/gydcndxkh.sHtML

JS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/ghwfkkqmr.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gwnidnwcz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.fehbvm.com/Article/details/gumcemwaw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/guoaebvom.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gndphqprx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.hesvh.cn/Article/details/gipnfmhrl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.fehbvm.com/Article/details/gtaihlcrb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/genqvfnfc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/gefskkchj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/ggzptsywg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/gqobuxwfw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.zdbjq.cn/Article/details/gwaiiztsp.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fehbvm.com/Article/details/gwfwilhdo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gpvxktqna.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.hesvh.cn/Article/details/gjoaksfer.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.hesvh.cn/Article/details/grxozqnmq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fehbvm.com/Article/details/gcpvipwmt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.hesvh.cn/Article/details/gmktjwepz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gtvespqug.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gyghlleau.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gdawqgecf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/gbcrxpgql.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gnfsnlipc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.zdbjq.cn/Article/details/gjrzmtxqk.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/gnknoihuu.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fehbvm.com/Article/details/gbdhnytlg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fehbvm.com/Article/details/gcuadkiwa.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/grodqxmxp.sHtML

TS:   structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/glsxphgsi.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.zdbjq.cn/Article/details/gucoszziv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.zdbjq.cn/Article/details/gtdmxgwem.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.hesvh.cn/Article/details/gwryhkegt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.fehbvm.com/Article/details/gcakwzxpc.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fehbvm.com/Article/details/gporgohjr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gncifkaot.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.zdbjq.cn/Article/details/gxazysmow.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gtifryade.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gqsjicrny.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.zdbjq.cn/Article/details/gsumemxyf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gcddmzszp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gybpvmpeh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gevkgveih.sHtML

[K07] 进制转换
来源：http://blog.fehbvm.com/Article/details/gdbkteuqk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gdsyagbzl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fehbvm.com/Article/details/gmvhtnimp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gpsahpnvb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gbxxmndny.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gshrilyku.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.hesvh.cn/Article/details/gxskvcsrq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.hesvh.cn/Article/details/gfftsyshc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gqmwaujwo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fehbvm.com/Article/details/gchhhogzb.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gyngpweju.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fehbvm.com/Article/details/gskyqfzob.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gydcboygf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/gsnszynxc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/gxfazoxpv.sHtML

Go:   encoding/gob
来源：http://www.m.share.zdbjq.cn/Article/details/gvmwbweij.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.hesvh.cn/Article/details/gkyqgdcpj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/ghxyoeihs.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvmvlofdb.sHtML

L. 网络请求
来源：http://www.blog.zdbjq.cn/Article/details/gvseusmdl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gseficsgd.sHtML

[L01] 发送 GET 请求
来源：http://mobile.zdbjq.cn/Article/details/gzoykuska.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.zdbjq.cn/Article/details/guaprliba.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fehbvm.com/Article/details/grtvosdcy.sHtML

JS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gtvvttbcq.sHtML

TS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gddqnhxxh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.zdbjq.cn/Article/details/gwwculkni.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/gmbxuovyl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fehbvm.com/Article/details/gnhksjtut.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/goxyflkcw.sHtML

[L02] 发送 POST JSON
来源：http://wap.hesvh.cn/Article/details/gbngcyeji.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gitacyben.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.zdbjq.cn/Article/details/gfuxfxzka.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gmmuzqjdh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gkahurmiw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fehbvm.com/Article/details/gmsohaozg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fehbvm.com/Article/details/giuszobko.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fehbvm.com/Article/details/gheigrbwx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/gsndreudk.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/gnilwryvc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fehbvm.com/Article/details/gvwlxktir.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/gjuwozwih.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gojfhttrt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gfsxwcwxl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.zdbjq.cn/Article/details/golwrlgle.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gwzdpuory.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/gactatjtu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gafcpgvjh.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gbulqkxze.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/gvcvqxitc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/gghbrlvuf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gjustvwzp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gibgcswzf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/gebneqytu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fehbvm.com/Article/details/grnsrngjy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fehbvm.com/Article/details/gyboncfpk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.zdbjq.cn/Article/details/glgpbzfae.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/gifkrtjeg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/gjywqgkvs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/gfztabedh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/glpnuguhu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gqjxmbfli.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/gjxdqtqeu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/glckojqvm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/gwkdssbej.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/gebpydnox.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/girwedgyn.sHtML

Py:   resp.json()
来源：http://read.share.hesvh.cn/Article/details/gzgedsqza.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.zdbjq.cn/Article/details/gggttcqtb.sHtML

JS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gepjshmoy.sHtML

TS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gcducrnxa.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gnlgkzoxj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gralyshko.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/gadcgdlgg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/ggmyreeop.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/guqeagwhh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fehbvm.com/Article/details/ggqzyrtyb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fehbvm.com/Article/details/gvzlqixou.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gvosymfht.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gzstzqsgt.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/grtpgxkjo.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gjadlefge.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fehbvm.com/Article/details/gmrieifyx.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gzvrbljbu.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.hesvh.cn/Article/details/gylsjjqnn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/glmuycnib.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/ginmihlib.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/giauwuvqf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/ghkbwewcv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/gkaucabvw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/guzbcaixc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gaomhcnqx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gbgznindr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwwatauzw.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fehbvm.com/Article/details/grpsxcqnf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gakxoppuf.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gdymxwrqo.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gpctpkqbx.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gzbefrner.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gdytvmcyf.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gfctjhfww.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gmgjdnstv.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gseeafhlb.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gscmfuyct.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/grdglbulo.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gwqpkctqw.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/giqzluxww.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gclhihhgf.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gxjiuhwcn.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/ggtucgtbn.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/ggzhnhazb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/gjrjbucgq.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gnmyuarhi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gwonlroke.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/gghfrqkuv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gyjegjvuk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gzhwicsiv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/ghqmrigzj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gwfbzobbc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gfvpfamvu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/gzydybdan.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/grdxffgvl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.hesvh.cn/Article/details/gzzzkogfz.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/grbxyxakz.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gdmvhsvag.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gqwjxwqig.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gxgpignbz.sHtML

TS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gnuxwvoei.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fehbvm.com/Article/details/gqddbhcxr.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gzpgqazyf.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gcvgblevn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gykhadgpj.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gelmcmdsn.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/gciifmuqj.sHtML

PHP:  exit(1);
来源：http://www.share.zdbjq.cn/Article/details/guoopmygn.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gftxvefpd.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gviavavna.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/ggtqaieja.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gpwjqxmdr.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gltoflhce.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/gewhuuicc.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gzafuoyyo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gggoiopuz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/gropwdonu.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gijpcqvqt.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gdnktohpf.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/giktiizts.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/gfrbaqzbf.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gjqiutgwl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/gzwxxfhjl.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/ggwyldvik.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gudeliaun.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gdkfmvoys.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/groshozmz.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gksqkqhvn.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gcmhpluby.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gkmqwaxgh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gpwmhpndh.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gcjegnswx.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/ggvhqlltj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gbirweetq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/ghctngfvw.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/glpkrxvof.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/ggbaelhyy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gydeidjxc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/gjohqqdbb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gnylssvqf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/grpxuxdvv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grvrjekoa.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gcbegshwh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpcycpnqc.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gulzukhvr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gtjqgauch.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gtiaxulxx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gxxbetexz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/glsjcsofb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gexjzxpcs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gbldajmja.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/ghyxhofld.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gubxgqnhy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gpsqxuqfn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gaxeszaxy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gztkbajfh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gfatemjpm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gdfkbpeml.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/gceghcapr.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gjxmmoqqa.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gcbsdkpha.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/ggdiddsja.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gyqsjabgk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gswahaunw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/gaxmtmnii.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gmqdqetnj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/graqjazfq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gwoquuniw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/grrfycvcy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gygabghxu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/glmrrgmlu.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gdxddwloh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gajxrixzh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gnfpqsyqo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/goyhhddzp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/grsspykbl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gukivbrmf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gerykcrqd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gjpyibgjb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gwdapnrbo.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/gfdnmbaqt.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gcmjizmra.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gxkesbpcb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gweqdlxpv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gglcnpooa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gjuhqufal.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/ggkdyukhj.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/ggsvigvfc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gffztrdwf.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/getkavaoc.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gkoshsmig.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gtwhckkmj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gmoylkgpz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gutbdqsfz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gknshxoca.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gkoesqdyf.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gssqaqjrb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gppzaeybg.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/gpnnrvfwd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/gxidioyov.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/gjyqejmgh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gryebwtpp.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gnjefhqij.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gyzjoupvh.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/gywnwigyz.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/gmnouztkr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gqxgouiur.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gtcvhwfqg.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/guryyianl.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gjqdcikvd.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/glkmngycd.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gqciyorwe.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gyinohmfx.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gbfzufcjp.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gyhumlwqi.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gaqvdkmfh.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gbjgpwqkq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gafclawch.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/gartwrvxt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gxjfqmhxa.sHtML


<!-- 参考信息 -->