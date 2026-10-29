代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/gilamnbgy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/geyabixha.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/gvuumyggv.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.fehbvm.com/Article/details/getjaxeul.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.zdbjq.cn/Article/details/gyzxfxtoj.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fehbvm.com/Article/details/gviloxtbb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.zdbjq.cn/Article/details/gcdkasmyp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.zdbjq.cn/Article/details/gjhjenvew.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.fehbvm.com/Article/details/gfyiqhlhs.sHtML

Py:   json.loads(s)
来源：http://wap.fehbvm.com/Article/details/gcmhdpkdg.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.hesvh.cn/Article/details/guptkskxz.sHtML

JS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gmtgsoayf.sHtML

TS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gcphvfvuf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fehbvm.com/Article/details/gamwsctta.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/gzxzsoxlo.sHtML

Ruby: JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/glrfozxcf.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.hesvh.cn/Article/details/gzmnbtcis.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.hesvh.cn/Article/details/gjksoxyhw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gfqxoaphk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/gcdsedwzg.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/gwefrksfu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gkomlocbs.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.hesvh.cn/Article/details/gkfbezbad.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.zdbjq.cn/Article/details/gmioertfw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.zdbjq.cn/Article/details/gfvnlorgt.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fehbvm.com/Article/details/gmbqetvyx.sHtML

[K04] 读取 JSON 文件
来源：http://baike.zdbjq.cn/Article/details/gecyeeuxx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fehbvm.com/Article/details/gdwwfkqhh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.zdbjq.cn/Article/details/gnzyspwxf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gpkkyomtg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gmwtybsqo.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gsahxxkoy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/ghykgnmyy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fehbvm.com/Article/details/gajkxafuh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fehbvm.com/Article/details/gdcioyvor.sHtML

[K05] 深拷贝对象
来源：http://mobile.fehbvm.com/Article/details/gmcubdbto.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.hesvh.cn/Article/details/glwcqrpgy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.zdbjq.cn/Article/details/gscebdujh.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/guhcjypen.sHtML

TS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/grhwreddl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fehbvm.com/Article/details/gpfactwei.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fehbvm.com/Article/details/guxyfhtvy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.zdbjq.cn/Article/details/gqlpcyiuz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.zdbjq.cn/Article/details/gagrspuuv.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.zdbjq.cn/Article/details/gvoshyksi.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fehbvm.com/Article/details/gokitgzph.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.zdbjq.cn/Article/details/grpenmqxr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/giwxnqepb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gtgwhzmxk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.zdbjq.cn/Article/details/gwobabxtj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gwamcrdxb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gnvhqzrre.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gjulejwma.sHtML

[K07] 进制转换
来源：http://mobile.fehbvm.com/Article/details/gwzduuogb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gvhvmamop.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fehbvm.com/Article/details/gkppytbee.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gzaslwnxc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gifgvnwvd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gthlmwtan.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.hesvh.cn/Article/details/gcyeswpuj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.zdbjq.cn/Article/details/gzirzpeqn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gzglkbwik.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fehbvm.com/Article/details/gnnsqnnlc.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.zdbjq.cn/Article/details/gywrvjxzg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.zdbjq.cn/Article/details/ggtellfbb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gtuqsuxyl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/goeakbnna.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.zdbjq.cn/Article/details/gwuppeqjw.sHtML

Go:   encoding/gob
来源：http://read.share.fehbvm.com/Article/details/ghrwufehh.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/gcwkajgkx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gkezvnehz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/guspvyrbh.sHtML

L. 网络请求
来源：http://www.blog.zdbjq.cn/Article/details/gunljiiyq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpcbpzmby.sHtML

[L01] 发送 GET 请求
来源：http://m.share.hesvh.cn/Article/details/grrjzwhef.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fehbvm.com/Article/details/gaihpevyu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/gnjpekphf.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gywobwbgu.sHtML

TS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gicbfhhby.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fehbvm.com/Article/details/gvxzkqcrs.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gzrdchxhi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/gsbcndaxo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fehbvm.com/Article/details/gntyodlqt.sHtML

[L02] 发送 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gcvkymoxz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.hesvh.cn/Article/details/gaqmsfvrt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.zdbjq.cn/Article/details/galgmvqcl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gczfsebiz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gkoypdhop.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fehbvm.com/Article/details/gkwcvzjzv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.hesvh.cn/Article/details/gbpltuzjk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fehbvm.com/Article/details/gwyxfpber.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.zdbjq.cn/Article/details/geqntgifi.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gwuxfmhdz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fehbvm.com/Article/details/gucnmhrzh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.zdbjq.cn/Article/details/gptgghvfi.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gfhtvfwpu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gisdwftdi.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.hesvh.cn/Article/details/gicfbwvwj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gxsdpvbdo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.zdbjq.cn/Article/details/gxvndfbqh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gfgcnfmno.sHtML

[L04] 设置超时
来源：http://mobile.zdbjq.cn/Article/details/gmeepbmme.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fehbvm.com/Article/details/gwcviohsp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fehbvm.com/Article/details/gelhrdops.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/ggucvzooy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gyopkndpg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/gwurmbfkc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.zdbjq.cn/Article/details/goltmqitv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.zdbjq.cn/Article/details/ggawmoqta.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.zdbjq.cn/Article/details/goggkzihl.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/gkgaioqhv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fehbvm.com/Article/details/gxzuxzdoe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.hesvh.cn/Article/details/gyzvxavqe.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gzkldlxlq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gqpkvedwh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gdkbwmzpz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.hesvh.cn/Article/details/gnehklloq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/ggkmorobq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/gjwrqlvzh.sHtML

[L06] 解析响应为 JSON
来源：http://blog.hesvh.cn/Article/details/gybkncnqz.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/gkrbhkath.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/gkwxubnen.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gadzreluw.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gzubzweph.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gegywoxki.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fehbvm.com/Article/details/gqlvvhvhy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gahllymka.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/gnqlfwegl.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gfafycqlg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/gatnksqpt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fehbvm.com/Article/details/gcteuixrd.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gukpehrvb.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gtercxppk.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/gextvlrgi.sHtML

Go:   resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gxvlzjfoc.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/gymhaftiw.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/ghrxjhcvv.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/gvbcpofiq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gadrbyonk.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.hesvh.cn/Article/details/gxwluteeq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gdnbfmfcm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gxppjzhuu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gxutmsrpk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/gavcckcrf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gbbquxsss.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.hesvh.cn/Article/details/gxqubpmhs.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqyjzbdub.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gfoynwfsj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqrufepeq.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gzclezqbv.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gzainycwl.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/gpgombqkd.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/ggzaywvqn.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/ghgyfxadp.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gksqgknux.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/gnecaopvw.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/gpxqmsmbg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gxoqkvxqp.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gatwbewzb.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/gklveqzkg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gogkgeobl.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/ginjzlloe.sHtML

TS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gylttoahc.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gnpwxgbto.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gmfczizuq.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/gzcaavgwu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/gachcacsr.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/gmjhdpjik.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gxblvazon.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/gdpfpvltq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gysgbagyc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gjguizfho.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/ganczpfcg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/gpfjjwold.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/gxylsulbx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gcqlplwfp.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/gtitmyhzh.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gpyzhsyoa.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/grizyrdwy.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/ghhqccsgt.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gmozlrfxc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gdiyazpqj.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/goqytiebq.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/ggjysrsgb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gigfmieml.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/gjhfnmkpu.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gtqlfupfg.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/gmfdawzpc.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gpzudyekf.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gfzlaqwwu.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gvwlrlcbh.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gzyozjmox.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/gapztvwnj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/gwrtwnjur.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/giclmzccs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gcmrwoyua.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gbjlbyyiv.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/grfkufjbv.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gqxoyjezk.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gpnxebwqt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gsgfjkpxc.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gknmdqslb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gjkwqqwld.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/glpuavgfb.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gbifmxghq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/gsdlwmqwy.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/glmrlnrgf.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gpcdnfsvg.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gwombbtdb.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/godyxffhc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gzlfazpgh.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gpoourgyb.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gzuvbovln.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gsmdljzfv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gdssmwnqr.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gfmdufeog.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gpwsinsfv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/gwufnxfsr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gigmzgazj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.hesvh.cn/Article/details/ganzxuykj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gexjmumpl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/giovojmip.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gmtxlmfii.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjaxczayf.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gvyrbsagt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/giwenevej.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gzvbtwegn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gjorsgaqx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gxoouyawl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gnlyrwmzx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/ghyygyptf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/glhrloqis.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gddwwueee.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gmfkcichm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gjmwrtgfy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/ggcjwsdby.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gnwyueyip.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/giomtwngu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/gsadqsyhi.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gtcufbaeh.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gdegogbmt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/ginxjfuvf.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gtqhjasdy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gulriaxyc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/ggfegytjr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gdvlcgbrd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/glyrqmajj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/grrjwuylb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/gsmxivlra.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/gvoypnhmz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gtjxqsjtq.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/giecwxsmp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gpccdswfs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/goiavjqqw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gbzhvsolz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gdnpaxumv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/geoypoqnn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/glonozoul.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gbprtidbn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gzmumdxky.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/gyrcqxusy.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gixikmnbq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gjxcgwlpe.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gstvzufth.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/ghcmqumze.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gbgpqybnm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gmejqelmf.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/gltwjvjqi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/ghzvezwbb.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gpzuirtcc.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gujgwsdld.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/guzfatpzi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/giyvprond.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gwecihhyj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gmrhixdcy.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gdnicviyn.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/globrsnug.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/grjnxtnxh.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gdqhnjazz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gvwpmqrym.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/goifosmyw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/gbyaxuksx.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gnwfknkhb.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gyldfqjge.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/gixfdrtnm.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/ghxytitlj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/goqizchsb.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/grukffefe.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gubnjazgy.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/gwfwdpkhu.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gjotkcvhd.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gklwtcsqg.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/grplbveup.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gkyyaqyhb.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gvvzebjeh.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gpmclwacq.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/giyfvxdhi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/geghfcbcb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gatbhxlip.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gqwaedsjo.sHtML


<!-- 参考信息 -->