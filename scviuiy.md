代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gokiddpcy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/gxwamikzb.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gjfbnfynd.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/gywgdueal.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.zdbjq.cn/Article/details/gpopfgael.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fehbvm.com/Article/details/gbhhomwbw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.zdbjq.cn/Article/details/gaxbrnpch.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.hesvh.cn/Article/details/gajncywrh.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.zdbjq.cn/Article/details/gfnpvkafv.sHtML

Py:   json.loads(s)
来源：http://m.share.hesvh.cn/Article/details/gjphuqeuw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.hesvh.cn/Article/details/gsbssrtls.sHtML

JS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gbxjydbnc.sHtML

TS:   JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gsgineyzv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.hesvh.cn/Article/details/gwgzvlmip.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gbmyizxon.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gqvimttnd.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fehbvm.com/Article/details/gjhwbopoq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.hesvh.cn/Article/details/ggakxwwpl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gztvftccs.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/gnaxtchdh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/ghzapqoky.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gywoiigxy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.zdbjq.cn/Article/details/gzmshlkad.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.zdbjq.cn/Article/details/gkkpjgocd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fehbvm.com/Article/details/gtceneaxe.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fehbvm.com/Article/details/geoszawdn.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fehbvm.com/Article/details/gmayiymhl.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fehbvm.com/Article/details/ghsorgqor.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fehbvm.com/Article/details/gpirkymew.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/gobfmulzz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gnenydzup.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/guujblxak.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/glezbrrdd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gpsfwowik.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.hesvh.cn/Article/details/gxlxznqnq.sHtML

[K05] 深拷贝对象
来源：http://m.share.hesvh.cn/Article/details/gyulcrbfz.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fehbvm.com/Article/details/gwpqdeyvr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.hesvh.cn/Article/details/gslmtbgvn.sHtML

JS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gnlcbywsi.sHtML

TS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/ggdibmkbe.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.fehbvm.com/Article/details/gstvcmpcb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.fehbvm.com/Article/details/ggrjdevqu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.zdbjq.cn/Article/details/gfoortjds.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fehbvm.com/Article/details/gbnzzfonp.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.zdbjq.cn/Article/details/glkfgiznv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fehbvm.com/Article/details/ggjkdweic.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.hesvh.cn/Article/details/gopjubqej.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/ggetwmdvv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gufeczrqb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.zdbjq.cn/Article/details/gqmqonbru.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gtixvzmgn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gnteempph.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gdijqedct.sHtML

[K07] 进制转换
来源：http://blog.fehbvm.com/Article/details/gkjsrfdvn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gjkidnfqm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/gxhdrbzhr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gbogcjipa.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gofkvtrea.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/guqznkxkn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.zdbjq.cn/Article/details/gnwnlkyet.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fehbvm.com/Article/details/gazmugroj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gsfcnqymm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.zdbjq.cn/Article/details/gaqbbxupc.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/gdszewjyf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.zdbjq.cn/Article/details/gwsanlfdx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/ghytbvgsy.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gescleqmc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.hesvh.cn/Article/details/glbpmwkgq.sHtML

Go:   encoding/gob
来源：http://www.m.share.zdbjq.cn/Article/details/grmqgjqnx.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/gmwdetawv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gzivxenyc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjwsbswbv.sHtML

L. 网络请求
来源：http://www.share.zdbjq.cn/Article/details/gegnhjehx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjkxhiwrl.sHtML

[L01] 发送 GET 请求
来源：http://3g.fehbvm.com/Article/details/gabexdnge.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.zdbjq.cn/Article/details/grqzbvfmz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/gppcyoeeu.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gqzvsbagi.sHtML

TS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gpwjteyor.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.hesvh.cn/Article/details/gmrnfhfmq.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.hesvh.cn/Article/details/gynartzzt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/grqekpdzx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/gllblzbmg.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gekkfwhlp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gkmvonsjh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/gtognlbgg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gvqfptpct.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gaomfyqvr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gwnyfoszb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fehbvm.com/Article/details/glhgydlhl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.zdbjq.cn/Article/details/gogtojhxq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.zdbjq.cn/Article/details/goavzqgyw.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/gojvqksjm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/ghckxcgwb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.zdbjq.cn/Article/details/gwtejegvk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gklxectyh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gbyiuxewv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.hesvh.cn/Article/details/gjdhkgwhg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gnngthcri.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.zdbjq.cn/Article/details/gobslieuj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gopqtvuiu.sHtML

[L04] 设置超时
来源：http://blog.zdbjq.cn/Article/details/gqolmzeyy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fehbvm.com/Article/details/ghtzrjwmg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.zdbjq.cn/Article/details/gkpdcxkcc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gbljnuvzb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gaddgwrrq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.zdbjq.cn/Article/details/gezwopxqs.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/gdepavzpj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/gmvhezifw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.hesvh.cn/Article/details/guqtzgzsz.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.zdbjq.cn/Article/details/guhcgdnla.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.zdbjq.cn/Article/details/gvzcmpisl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/gghpiuttc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gmkykrhkq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gafneoixj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.hesvh.cn/Article/details/gyoirtxvi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/grdyptrng.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/gwscizmeq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.hesvh.cn/Article/details/gdxezesmo.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fehbvm.com/Article/details/gxeevirhf.sHtML

Py:   resp.json()
来源：http://3g.hesvh.cn/Article/details/gkaisohan.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gtghdoccm.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gexkkmoec.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gxofdfdtm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gtlklcata.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/gzicfqnyh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.zdbjq.cn/Article/details/gcnpkydqv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gewtxrfrf.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gmvjjpful.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.hesvh.cn/Article/details/glrhistoe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/gdwhdwfxs.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gqzkfdxma.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gdaqdgjcv.sHtML

Java: resp.statusCode()
来源：http://www.blog.fehbvm.com/Article/details/gaagdbhgk.sHtML

Go:   resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gtlcmnenu.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/glbgizmtu.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/geqxmzinf.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/gsxsamrdt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/gehtbdaie.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/gkefzzjaa.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gbzcsjacd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gortfkyfa.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gwevvrzjl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/genertbyt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gwhzhbmkz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gteygrznk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnlonzlkx.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/gdppgqtia.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggumyvbqy.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/gynujxzwa.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/goslqghvr.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/gvddnezou.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gnjnlhqwy.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/grxnywrvx.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/ggejkacqs.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/gqkncuarw.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/gknyczstp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gulabebss.sHtML

[M02] 读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gwvepzjvr.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gxyguxrnh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gwpddhhqk.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gsdlkyanf.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gyexdtreu.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/ghanuciag.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gpxvhcvea.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gaywmefnw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gossqgpsd.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/gghuofryn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/gwbvocjtp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gukqwrzro.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gzpvlgclu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gaenqouwt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/grfgprdwu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/ghgbqqlrf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/gzqrsczah.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gqxbaiagt.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gwvseexbo.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/ghtatjerx.sHtML

PHP:  getcwd();
来源：http://www.blog.zdbjq.cn/Article/details/grqebcrse.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gxcbcxxkv.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gwmokvzib.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gvsijiquz.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gkgvcomfj.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gopashxfd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/gtpyclgnr.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gvalrfmzb.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gyrrwkkit.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/ggxqnqqgk.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gkftatbkm.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gjnhtsnna.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/gfyydwwvg.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gabkmiylb.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/ghbflyxet.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/ghqzrmlam.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gkgqxlvfl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gxiauofmi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gohejkady.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gztgfrash.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/glzkrwtpz.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gsoynnxer.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/ghjuwsihi.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/gtoeblxtl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/guybfuzcw.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gcmpdvkzr.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/grbvkjpwj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gkgoyqurs.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gioettgfe.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gzpzwzfgq.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gnevelrxr.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/gfnixbtmy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/gchckwimq.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gnblwqezs.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gerqphmoh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gywkwhisk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/gmklrklwy.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/ggncvuwda.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/grirdvoye.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/gndtmwpdu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gtbgqsiyk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gakezvukw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/gllbvmejw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gadfcrjae.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gyqvxxlpi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gybjnuniw.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gpjuimvcm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/gwsxnvzpw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gyhwmotex.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gunfbmpxd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gyntvmmze.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gcwnirplc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gbprvtosr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gsrjnutzw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gsevexzgv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gxwpfnvkv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gnxsnncct.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gmzeasalo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gnkrpuomy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gfhgpogox.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/goefhdeqj.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gerdolnbq.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/goejjfjlc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gbciqiitg.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/gpkataruq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/gvagoxphc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gnpovsrnb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gzdbdwdyu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gbwarmtdb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/grplwdzwz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.hesvh.cn/Article/details/guidcrckg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/gmnsarykq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/gpyhrbsjg.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gskfkngtk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gdlijhmsc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/grqyvzbff.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gtkvijwnw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gwdtrsjao.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/ghbzmdmxd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/gfajcxyuq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gjuflingr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gvpgzealu.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gfbuigiwp.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gtvpcdvhc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gnkmftctx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gpmjpllux.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gycrmbanz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gqwncbtrt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gilenjwwu.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gzypjcwcn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/gbbkeomvw.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/glssflyrk.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gslqfgkgm.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/gjlusejpc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gkoukdkek.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gimvgnbvk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/ghjpnqyus.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gbaihxqti.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/ggdzljkqt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gpjztrlbk.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gjsjpquqc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gmqgrkrvw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gqegzuyms.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/ggonjkupw.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gvdijpcfd.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/ggfupstgk.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gfnaosojw.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gdpaqehqw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/ghlwiuebv.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gybctovaq.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/gafjgssjf.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/gwtaisrzp.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gezlxskwy.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gjcurkauj.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gyrfomnkk.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gtrskosly.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/ggqhjkrcp.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/ggaapmqjw.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/gpvwyzusu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gsxsubtbb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gwpswlqur.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gkhwovhks.sHtML


<!-- 参考信息 -->