代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.hesvh.cn/Article/details/guegphsxx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.hesvh.cn/Article/details/guvoqfyiu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fehbvm.com/Article/details/gsapcgixw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.hesvh.cn/Article/details/gfznjpmrb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gniwfxoqn.sHtML

K. JSON 与序列化
来源：http://blog.fehbvm.com/Article/details/gxihjibnu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcyqmgddw.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.zdbjq.cn/Article/details/gschcrkgd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/gxcwwwcog.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gqdlccele.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/ggllbppdg.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/galzqcbzm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fehbvm.com/Article/details/gjiopexwy.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fehbvm.com/Article/details/gdjronedc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.zdbjq.cn/Article/details/gtjlltelz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.hesvh.cn/Article/details/gwecunweq.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.zdbjq.cn/Article/details/gvzdivkbw.sHtML

Py:   json.loads(s)
来源：http://www.share.fehbvm.com/Article/details/gxflrfgjn.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.fehbvm.com/Article/details/gqspmpqhg.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gcmtzgdrs.sHtML

TS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/ganeqqlcv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fehbvm.com/Article/details/gsfrvuwek.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gmcfzwjxm.sHtML

Ruby: JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gdgznfkwo.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.zdbjq.cn/Article/details/gjiitwucz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.zdbjq.cn/Article/details/gxxnzvmza.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gyctjxfpc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/gtxsrkmqr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gbhcfolmh.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/gdfnbkxob.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gvmcnrtlt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.zdbjq.cn/Article/details/gdnesyfnw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.zdbjq.cn/Article/details/gerzqadff.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.zdbjq.cn/Article/details/gnidhmgex.sHtML

[K04] 读取 JSON 文件
来源：http://wap.hesvh.cn/Article/details/gucjjuemz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.hesvh.cn/Article/details/gwwdirmlw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.hesvh.cn/Article/details/gbdfyihos.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/gvdkwahrg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gbnmhhjql.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.hesvh.cn/Article/details/gqthklwsx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gsyjxgpxo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.hesvh.cn/Article/details/gundwkoru.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/ghsakdgfg.sHtML

[K05] 深拷贝对象
来源：http://www.share.zdbjq.cn/Article/details/gqeaggigm.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fehbvm.com/Article/details/gwzsssxxj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fehbvm.com/Article/details/gxgrqlbca.sHtML

JS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gcbkrtpfn.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gacvtltuh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.hesvh.cn/Article/details/gvdhzzkwh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.hesvh.cn/Article/details/gcqqbdsnd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.hesvh.cn/Article/details/gxhmyurwy.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.zdbjq.cn/Article/details/gpwkkzcdt.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.zdbjq.cn/Article/details/gsjpdyqmv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fehbvm.com/Article/details/gipucgxba.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.hesvh.cn/Article/details/gtlwxxwcr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gvdmczunh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gldvdpltg.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.fehbvm.com/Article/details/gsjlsmyad.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gcetlvkkc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gavlrwysw.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gtlxwrvcn.sHtML

[K07] 进制转换
来源：http://blog.hesvh.cn/Article/details/gpyqmmxcn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gjtuivrev.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.zdbjq.cn/Article/details/gbhqzezrb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gstgqsaec.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gpxrihbqr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gnromipyb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fehbvm.com/Article/details/gfxvrwlag.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fehbvm.com/Article/details/ghggojpzd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gtqfsrryv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.hesvh.cn/Article/details/gocakpgfb.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fehbvm.com/Article/details/gqtxljkvs.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/gzratbxsd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gtyyrsakp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/gcfqzsbgw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.zdbjq.cn/Article/details/glaqllxwy.sHtML

Go:   encoding/gob
来源：http://www.share.hesvh.cn/Article/details/guodsimmy.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/guummfdwd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gqonyuqiv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdlvuryqm.sHtML

L. 网络请求
来源：http://blog.hesvh.cn/Article/details/gphasyxsn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggziaeacu.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/gyhyghxdj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.zdbjq.cn/Article/details/gnxnmonge.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/gtntajusq.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gkjyvevdy.sHtML

TS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gsovhijmc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/gggbsvlqw.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.zdbjq.cn/Article/details/gvltebsha.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/gtnxtwakg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/gkzsnahtg.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/gporvkoda.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.hesvh.cn/Article/details/gdcnrgefm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.hesvh.cn/Article/details/gdnaoyqdm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gpxpllpmx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/glvvtuhxp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fehbvm.com/Article/details/gscuowjoh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.zdbjq.cn/Article/details/gdbcemdqe.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fehbvm.com/Article/details/gvibvpejc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/gjxxhizao.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.hesvh.cn/Article/details/gdrgpodba.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.zdbjq.cn/Article/details/gwbkssfqz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.hesvh.cn/Article/details/ggrsjyiru.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/grewqdnsw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gaqchdkbw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.hesvh.cn/Article/details/godlgmtbb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gixdvzgxy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/gmgitfmce.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gxqvwmvej.sHtML

[L04] 设置超时
来源：http://wap.hesvh.cn/Article/details/gikvshocu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/gziqtulba.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.hesvh.cn/Article/details/ggrbwmqlv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gusvdflkc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/glehuqpiv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/gxpasxiuv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/glkgyvely.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.hesvh.cn/Article/details/gvhseouyp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.hesvh.cn/Article/details/gynrqsiyy.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.zdbjq.cn/Article/details/gppeslnzg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gafgbyzbn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/goikngxkm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gzoryjckj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/ghcwnfzer.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.hesvh.cn/Article/details/gomsquprk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gedrbains.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/gwwdjxlgt.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/gajhcxinh.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/gkzbhnqfv.sHtML

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/gxawwdeip.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/gstwtfhgz.sHtML

JS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gnhrjxedx.sHtML

TS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gknzrqncp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gnbquecuh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/ghgnldlin.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/gpojgcqxv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gwfvzfkjt.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gktyibszi.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gfbmiecei.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gzjelkicg.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/ghueatcjf.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/glwnvctgr.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/gimbglsmv.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gxpjwiyql.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/gkaqkbwgm.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/giaqkkrbw.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/ghybtjrir.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gzhdngobx.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fehbvm.com/Article/details/gofdwfsod.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/ghurfeucw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gehfcseqr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/gjvuxfzom.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.hesvh.cn/Article/details/gooeeawhd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/gmvekimtx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gidrmwoyq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmdsaqnkb.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gtroxbedm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghwsyjwfl.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gcqecaytr.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gdyddlazq.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/gqpyyvmuq.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gmosfxowf.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gqgknkmqi.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gpccpaumv.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/gdvlgabqt.sHtML

Ruby: ARGV
来源：http://blog.zdbjq.cn/Article/details/gexypnqyq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/goltaiuwj.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gnhlkoddm.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/gpwzotyxy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gttydepkc.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/grhgrwrwa.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/glmljnstl.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gjjjxpuxc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gfrxqjdrs.sHtML

Ruby: ENV["HOME"]
来源：http://wap.hesvh.cn/Article/details/gyjmnaprz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/guhwdgncg.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/ggwpckooj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/gkwsgrssj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gasyqdnno.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gnskewpmb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gjlcgijjv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/goczomvpx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/givonzrtm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gscpeigbd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/grgdjrixn.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gbgowxmvz.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gklntnwnj.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/gzxpeakpg.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gzhoionjq.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gpjwvyrvu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gldrnooqv.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gxxbukyjs.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/geipinoty.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/ggnfrhvzw.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/giflnfwut.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/ggjivktjp.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gtovtwhpp.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gykcdyzei.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gdhdrdbyx.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gerozrrth.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gagcqmich.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gxpezpntw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gegeegsrz.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gvpovtjeb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gqsvnpcee.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/giretadgg.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gqfhvndxn.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gotdqzsod.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/grgbhpowj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/ghhvwxcub.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gpxlhubma.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/gqzdnfwel.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/gjufmcvvn.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gwyljybpi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gugvpadlx.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gnsrntixb.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gluxyehdq.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/ghqultmpq.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/giojigyhf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gpywsgney.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gyuocqsop.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gndentyac.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/ghywiheyb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/gqwlvgoyk.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gamypxvrx.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gngmvzdcz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/glvfgazqw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gnqosvspi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gldlllnet.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gtvdhnviv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnwdfvuvn.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/gvcsmfdzb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghdpeflrj.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gniuwtbng.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gwcmktkgi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/goyavmudk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gredxiief.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gqnrlsmux.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gtfwltuyc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gxekedqdv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/gtkocwhfe.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gqerdttec.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gqjxzgxma.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gwkbqkoqo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gggbpejeh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gdrjfzbmc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/glqlrhsey.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/gdikvfnuw.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/grbqhqfbo.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gpicslyye.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/gcphjoege.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gwplsjiqo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gspwnnort.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gdwepbgly.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gpexdsxmt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/guckzmdra.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/gajkhxgwx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gaosbdwdj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/grbwxahgx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/gqpcmyzuq.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/gmrbptwsp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/ghtduezrg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gmgtkdjyd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gbdkekjik.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gktoymtdb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gksauerxu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/goawzftqs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gjyuukxxc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/guthyvuqg.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gaunkcmtd.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/gelsqrnfo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gxbteouhw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gxltyurjz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/guhuratoe.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gwwnghsiz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/gdvuvwcyo.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gmumijczd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gtbqgsawx.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/galkrdmpy.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gjlppzddo.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gjimrwqxa.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gfqeypnro.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gtveemqxo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fehbvm.com/Article/details/gdhjyxgrd.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/gkzdgmduq.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/gnwswtjtp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gugxpurgh.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/gzidujgvq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gjifiedfe.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gwvvtpqqc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/gjvsnxzoz.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gbxzcwvat.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/gebwwwqoi.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/gyjmpofwl.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/gimpqpeyv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gigraswkw.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/ggvupfeip.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gcuvbtiop.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/gugyvnthb.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gxemdjfmu.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gtigepjhv.sHtML


<!-- 参考信息 -->