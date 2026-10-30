代发 wailian999

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghjtwlmwu.sHtML

K. JSON 与序列化
来源：http://m.share.fehbvm.com/Article/details/gqwgxqfvf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggslthdgb.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.fehbvm.com/Article/details/ggosafnfw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.hesvh.cn/Article/details/gxnnlcrha.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.zdbjq.cn/Article/details/gdrjyzovh.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/gwhqtgzvc.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/goyuqnjia.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.hesvh.cn/Article/details/gzhkxakjl.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fehbvm.com/Article/details/gltmsrfpa.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fehbvm.com/Article/details/giocbufrh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fehbvm.com/Article/details/gjputlere.sHtML

[K02] JSON 字符串转对象
来源：http://3g.hesvh.cn/Article/details/gurklsdhn.sHtML

Py:   json.loads(s)
来源：http://mobile.hesvh.cn/Article/details/ggtnnpnvw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fehbvm.com/Article/details/glymxjian.sHtML

JS:   JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gbwsvpxga.sHtML

TS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gpsxenayi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.zdbjq.cn/Article/details/gsysxwoay.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gxhvqwwjt.sHtML

Ruby: JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gercdkfni.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fehbvm.com/Article/details/gmdkkyojw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.hesvh.cn/Article/details/gqskyabmm.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/gnnpyzruu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/gubppkjgr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/glorvtppk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gqexcgcdf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.hesvh.cn/Article/details/gcxclqtef.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.hesvh.cn/Article/details/gtwqmxdqw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.hesvh.cn/Article/details/gudjiunzs.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.hesvh.cn/Article/details/gcdyrbnuj.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.hesvh.cn/Article/details/gjszwwimj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fehbvm.com/Article/details/gnxwsqygr.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.zdbjq.cn/Article/details/gesrsgmdd.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/gqamesgpj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/ghznhdjcp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.hesvh.cn/Article/details/gtgpmurrt.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gukudrmno.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.zdbjq.cn/Article/details/grahxkckz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/geryjfbms.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/gfbvlxxrq.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.hesvh.cn/Article/details/gepimafbi.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.hesvh.cn/Article/details/gmyvguxpr.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gpqjgqskd.sHtML

TS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gjeqzjjqu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.zdbjq.cn/Article/details/gxkhpdgnp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.hesvh.cn/Article/details/gaqjqpjop.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.zdbjq.cn/Article/details/giybeclxf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.zdbjq.cn/Article/details/gsoxpqsge.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fehbvm.com/Article/details/gttobvgqn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gpnfarnaq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fehbvm.com/Article/details/gymtquxhu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gkbuagqnr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gwuguuivd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.hesvh.cn/Article/details/gvlbybczs.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gjadaqhya.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gwckzjzof.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gtppqvqqn.sHtML

[K07] 进制转换
来源：http://www.m.share.hesvh.cn/Article/details/gbbgkipxv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gberaassn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fehbvm.com/Article/details/geekbzaun.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gomyedgbr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/glhwcgpds.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/ggejwioqj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.zdbjq.cn/Article/details/glfgcrkzl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/gbiqoiuio.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gtmpnwlbj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.hesvh.cn/Article/details/gymhlzcuv.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fehbvm.com/Article/details/gqhuhazso.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.hesvh.cn/Article/details/gjcpaelvs.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gdrspydxc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gamynntxo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fehbvm.com/Article/details/gmkzpmrrz.sHtML

Go:   encoding/gob
来源：http://www.share.fehbvm.com/Article/details/gdeigqvuq.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.hesvh.cn/Article/details/gbkzzgndg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/giwffpqpg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwvybyfza.sHtML

L. 网络请求
来源：http://wap.zdbjq.cn/Article/details/glvivvzrn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/geulipwfy.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fehbvm.com/Article/details/gfholywty.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.hesvh.cn/Article/details/gkyvjafzf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/gtkobkuwz.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gremwfbqq.sHtML

TS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gxrljwubi.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.hesvh.cn/Article/details/gboimysvt.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.hesvh.cn/Article/details/gitkjghap.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.hesvh.cn/Article/details/gtalozcni.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.hesvh.cn/Article/details/gagjxldcw.sHtML

[L02] 发送 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/geuvhvzrw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gxrfyhjvt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/gcgiznwrp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gpagllpuy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gsroljmte.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.zdbjq.cn/Article/details/gtwamkuoj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.hesvh.cn/Article/details/gwablgwhw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.hesvh.cn/Article/details/giexknpgu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/gzccghcka.sHtML

[L03] 设置自定义请求头
来源：http://read.share.hesvh.cn/Article/details/gxtfjbqsn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.fehbvm.com/Article/details/gtvbliqst.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.hesvh.cn/Article/details/gnxdzikdm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/glnhnyaio.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/glccmdcwa.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.zdbjq.cn/Article/details/gwpynrbwg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gxkbiwfwn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.zdbjq.cn/Article/details/gxgaamiid.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gfoovdzwd.sHtML

[L04] 设置超时
来源：http://wap.fehbvm.com/Article/details/gcbkgwrjj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/gdjlamrpe.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fehbvm.com/Article/details/gdjtmbems.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gasnqtgjo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gebxykfxk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fehbvm.com/Article/details/gpkocimul.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.hesvh.cn/Article/details/gzqmhrmab.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fehbvm.com/Article/details/gdxlokvhv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/gtcuzramd.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/glubtnxbc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/gievecibh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.hesvh.cn/Article/details/gjlwsdnef.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gvgsmycnl.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gafbaisge.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gjilkixrd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gyyjgisxb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.hesvh.cn/Article/details/gfkeprvmt.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/glcmwbvkn.sHtML

[L06] 解析响应为 JSON
来源：http://wap.zdbjq.cn/Article/details/gigodheqy.sHtML

Py:   resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gxvstncfh.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.hesvh.cn/Article/details/gbuxqlztm.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/giquhfdkq.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gfkwobtcw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gwsaxqvyg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.hesvh.cn/Article/details/glwzwbkvr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.zdbjq.cn/Article/details/ghvjiodmr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.hesvh.cn/Article/details/gyutoaulg.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gedmgtmbz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.hesvh.cn/Article/details/gvqukodfe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.hesvh.cn/Article/details/gzoisjqsf.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gorunmvqu.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gplgdvaou.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gmiiartzd.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gsigdtcvf.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/gxsgmsxtk.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gfgkmkxtx.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gdcfbcfba.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.hesvh.cn/Article/details/gmejzxazj.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gsquskgqg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gjihiwyws.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gkkjxlung.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/glvhntpib.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/grzapytrm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gipajtdso.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gwxepktzl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtbldxpie.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/ggfqvquuv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyrlipiyz.sHtML

[M01] 读取命令行参数
来源：http://baike.zdbjq.cn/Article/details/ggodhxuyb.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/gxusihgsl.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/gydmttrii.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gecnvocjn.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gqjqhyuqn.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gsvobfuxa.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gsbniwxkx.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/gdlikiuvm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gguunazih.sHtML

[M02] 读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gzcoqqets.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gwqdvvyje.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gzpdxmepr.sHtML

JS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gpkpktwha.sHtML

TS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gfxtzohmt.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gckczwkca.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gnjndeoty.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/gskwovhka.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gweyufqiq.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gnbwdzpps.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/guunkegnd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/gqkzkrygs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gvgvdzhbl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gwzsddltx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gybaeotvi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gqqzdywen.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gczwspubf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gnpzoqngj.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.zdbjq.cn/Article/details/gjcjmhenq.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gcpaiimcd.sHtML

PHP:  getcwd();
来源：http://www.blog.zdbjq.cn/Article/details/gpoyxzcas.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gpfhjlszw.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gamsueftk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/gceldoahm.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gciqwnrcr.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/gzmqpjssc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/glqmfpaua.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gwewzxmxg.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gixahuudb.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/gjxmcufxa.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gplqlewqd.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gebivhddv.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gkmmjltiw.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gzgkiblkm.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gmptzhpaj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gxwnzshcj.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gkwpyjeft.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gkfbetsqm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/giqzmhppw.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gveugivoj.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/guvezjqtd.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gyuyowtgv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/gluxfsrwf.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gkbwplfjd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gkdusovam.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/gnvqfkgty.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gggrrzbgr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/guflecoxk.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gpdpyudyw.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gllocjlkx.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gmouxrbxv.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gjvsxksqv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/glqxckwvi.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/ghlkylsfu.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/gswxgjutr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gcwztpsdt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gwuprdivy.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/guutqmyyw.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gduhrydqr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gkqwfhvhi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/gpznzoogm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gmuimebpq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/gocyusakj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnxyxnwsu.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/geeoxjent.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjnigkuky.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/gvjfxnmfb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gkwlelhcb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gmywmhuze.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gtpedgync.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gwmrufzhc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gvtayggnu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gmeeennvu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gvzoyhizx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/garjxfjlr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gilcbnawi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gkounnnsj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gkiabdyco.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gsiksdwnx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/geylynscj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gcxleizpp.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/ggjcjzncd.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gkxrycuyp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/gcnghzxxu.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/ggjodvcpk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/gjlcelxef.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/gwzwjpmhr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gizufovqg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gydlmlinp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gkqpcxdgw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gkxfhqvqj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gsecsalck.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/guwvvwtgu.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gtochfxfe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gstqmmeeq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gvepbzrdc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gjacrkcdd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gytqlpjcu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gyjyivsqw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/gnbacwvjc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gzuobwmoq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gjuumhocg.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/ggtxtitrg.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/genbqffya.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gxgywprgc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gtlbgenbz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/ghobbqvxg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gxvtwnqyl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/gxdnrdprs.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gsdjujpgz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/gkjnvpcyo.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gmnbqruit.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/glgcotuwf.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/ghdgchudh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gioucfmjh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gqbyktlkv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gtlcindfz.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/gwshoaihh.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/gehceqhil.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gebylmwel.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gxmprfxlr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/gntzyrzew.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gnmmuhdjg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/giivmlofo.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.zdbjq.cn/Article/details/gmyifezmt.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gwsvwanfo.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gjjcalshw.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gjnsrtswi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.zdbjq.cn/Article/details/gcixfzpid.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gukdrggsz.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/gxqkbgwaf.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gekqclqfe.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/ggvxdvjpa.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gkrpgkriq.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/grkzztfvg.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/glumgkqou.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/ggubwlddu.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gnxfenzqd.sHtML


<!-- 参考信息 -->