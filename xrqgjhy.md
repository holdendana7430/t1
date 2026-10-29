代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.hesvh.cn/Article/details/gdptwmxxt.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.hesvh.cn/Article/details/gewdsiupe.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.zdbjq.cn/Article/details/gjurkaebw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.hesvh.cn/Article/details/goveipdmr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gshysekpt.sHtML

K. JSON 与序列化
来源：http://3g.fehbvm.com/Article/details/gmuyihahp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/geaexfzbv.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.hesvh.cn/Article/details/gcyonrjee.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/ghapjnyah.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/gfmzettbz.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/gximdjltn.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/gjqlmvszc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.zdbjq.cn/Article/details/glseezrst.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.zdbjq.cn/Article/details/gdpcwkzgf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.hesvh.cn/Article/details/gwvmzoykm.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.hesvh.cn/Article/details/gejehgrfk.sHtML

[K02] JSON 字符串转对象
来源：http://3g.hesvh.cn/Article/details/gzabnfmpk.sHtML

Py:   json.loads(s)
来源：http://blog.fehbvm.com/Article/details/ggbgmkruq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.zdbjq.cn/Article/details/glkxqfmlr.sHtML

JS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gficfikaz.sHtML

TS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/guzwlzzaz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fehbvm.com/Article/details/gbujigboy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gyscwauwo.sHtML

Ruby: JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gttxhwbqt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.fehbvm.com/Article/details/gdxyqxobo.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.zdbjq.cn/Article/details/gzxaspgwi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/gcaxbutfb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gqhclavee.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gbreydcsv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gfhclnfce.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gkcjhcwhn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.hesvh.cn/Article/details/gxdevrgaz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/gischpplo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.fehbvm.com/Article/details/gksshohre.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fehbvm.com/Article/details/gfyjjqgro.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fehbvm.com/Article/details/gsmcidmux.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.zdbjq.cn/Article/details/gaoglvwso.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gwnlzmmsz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/gzzeqylgb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gtqmfrzei.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gxweambyk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gzlovygcd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gvaoamdkr.sHtML

[K05] 深拷贝对象
来源：http://3g.fehbvm.com/Article/details/givcterzx.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gcgcewsvv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fehbvm.com/Article/details/gncglwgbk.sHtML

JS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gizzfvpti.sHtML

TS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gwaicgkbm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.hesvh.cn/Article/details/gpolinfqw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fehbvm.com/Article/details/gqvefferl.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.zdbjq.cn/Article/details/gxwiyeekc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.zdbjq.cn/Article/details/gobvtluje.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fehbvm.com/Article/details/gyjwgiqih.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gedhwjxxf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.hesvh.cn/Article/details/gcgonibsz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gmrneqbji.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/gegfhnfch.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fehbvm.com/Article/details/gshptgbkm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gdhswkake.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gvnqpnegl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gftofrxrc.sHtML

[K07] 进制转换
来源：http://read.share.hesvh.cn/Article/details/guwhkyhtb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gbdszeqqd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.hesvh.cn/Article/details/gjpghitao.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gzlwgfeyo.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gkiiwomzt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gragmudzm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/grgumowws.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.hesvh.cn/Article/details/gjgwrwebp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.hesvh.cn/Article/details/glnppdcbf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.zdbjq.cn/Article/details/gngdbzrmj.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fehbvm.com/Article/details/gdnjvtqno.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.hesvh.cn/Article/details/glrpumled.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/ghhzqmymm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gklbzgyti.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.hesvh.cn/Article/details/giwyovqpp.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/glasjkios.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.zdbjq.cn/Article/details/gdpuvsxvs.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gpicwbnjn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxyofhrab.sHtML

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/gxolvrvjq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzfdgbmyp.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/gqnqwdqrj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fehbvm.com/Article/details/gcdboyojj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.hesvh.cn/Article/details/gexreqqxp.sHtML

JS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gyhfgixoq.sHtML

TS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gfwwofdhs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.zdbjq.cn/Article/details/giqahklxu.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fehbvm.com/Article/details/gkzjtlskb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/gguewuacg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.zdbjq.cn/Article/details/gllxhtfeu.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gxcuwmmrn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gjuqbvpcv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fehbvm.com/Article/details/guofyvzgg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gkxzjehhg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gxpkrfxah.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gojsnkpmg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/gzrlzwrlg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/gijtwxyjs.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.hesvh.cn/Article/details/gfmsfxjgm.sHtML

[L03] 设置自定义请求头
来源：http://read.share.hesvh.cn/Article/details/gcsjspudr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.zdbjq.cn/Article/details/gpynvonkz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fehbvm.com/Article/details/gromoaxjc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/goixizqhy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gkujucyrj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.zdbjq.cn/Article/details/gmagikkom.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/goejigygb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/gngucfeev.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gdonxoglt.sHtML

[L04] 设置超时
来源：http://www.blog.zdbjq.cn/Article/details/gnuundagp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/gglzowuni.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/gfpbaornd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gdzilcuea.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gqtwcfigu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/gcdtbtjqd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.zdbjq.cn/Article/details/gzohkwyir.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/gqgloclhg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fehbvm.com/Article/details/gwkvgpvxj.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/getgkrtek.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fehbvm.com/Article/details/gfnjitbvs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fehbvm.com/Article/details/gtabmrier.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gecodcmlp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gojvjwxsv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/gnkinarme.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fehbvm.com/Article/details/glsxmwjfy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/gqrtouldu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/gprrhmzfh.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.hesvh.cn/Article/details/ghsajlrqd.sHtML

Py:   resp.json()
来源：http://wap.fehbvm.com/Article/details/gkuxtclwy.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/gavipxelm.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/girkmhetk.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gewzunqbl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gipswbirn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gpqssptyj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fehbvm.com/Article/details/geczoikwb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.zdbjq.cn/Article/details/gwvfjsump.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/goainzqov.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/ggdrvkysm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.hesvh.cn/Article/details/gygvdgqfb.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/geakoaxux.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gimtfoghl.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gdfgbhwjr.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gtmecqcsd.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/geofeggkf.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gfpkszlcg.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.hesvh.cn/Article/details/gvldovpay.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/gzexvxbns.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/grzoogdxy.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gpcjzjrku.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gjiqjpzfu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/gliiglyro.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/gxyxootqp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/grkszdqsk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fehbvm.com/Article/details/gatdcctwa.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gllxyymhu.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/gvjsnrtfy.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnlskozzi.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/gkaubsmvz.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gxbrbwjky.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gejvmfabs.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gojvaguxv.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gjveitbaj.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/grqigcigl.sHtML

Go:   os.Args[1:]
来源：http://blog.fehbvm.com/Article/details/giuafnlva.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/gclkiyfdk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gqejrjyuv.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/gliaitjge.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/gougrtrph.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/glikiuedp.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gxutxujdq.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/geexbjert.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gsgbiuqoz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gotqkocvj.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/glvarvgnh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/guknykpit.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/gbbcdviqa.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/gllafzyoq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/gsrflcwkw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gfxkjzsvu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gotgekarb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gkrnuydza.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/gmjaeyznd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/grneaqibl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/gnhsvnmco.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gxccblgti.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/gurgevhlq.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/ghmpaxiwm.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gtkijfomy.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gxgnnzkbo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gmqlcnyht.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gplejpyge.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gsdwhjgov.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gsomkwpdn.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/gsitsdnfh.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/gksrketlg.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/grwcrngwa.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gjqrkzpdm.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gqedeuiee.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gpwpagukd.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gukolqwyw.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gkmnjrpti.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gjsofxhbh.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/gswuyjdsa.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/grbpzquhi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/gzmkxdqmy.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gjwsqjqkl.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gkrxotwrh.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/gqikkjelq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gyhylufjy.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/gfgoogwml.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/gyenwthuk.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gluwckual.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gwemvjvuq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/ggctjuwji.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gexmhoqtp.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gcmjqbcyc.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gimnfvdsr.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/gbvqdzgje.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gxfxsnjgy.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gdzjrrhzm.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gpzaxfwlm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gxesewbkz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gnwhffogr.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gmrjvboxw.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/grsbkrang.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/gzvpdvkqe.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gbxkimbza.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gkdsmcyyc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gfyowegzq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbjarurip.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gogksagrz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmawowmsr.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gikymlqiw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gjjisgztp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gmwyoeoby.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gxpsnpwyw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gkoxywxsf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gddomrdkr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gwyamtnfx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gujrsvkik.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gefybskqx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/guupppphy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/godrponad.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/glhxgdlgl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/guarhhfkk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gkwtzkgkc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/gcvtphdwk.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gzlbsmdsm.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gibwyiyzc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/gjocqcoxy.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gfxvnerfj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/grizxuemk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gjxvxgvjn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gzrwpfyme.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gyzrvmwuw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/gwgxmonfd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/gymkjwbta.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gbtpdfaqn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gaurdqcfo.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/gdamlscun.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gdoyctlsl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/getdfxgsy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gtxkltqpt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gosrcoeiu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gyeiazpyx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gcqzdylpm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gwuauyvfv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gyycxfkyp.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gvvdxvuce.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gkdfftzyy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gzflgprud.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gastxnkhj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gyvwixufz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gvhnsbkyy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/ggetlymkc.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/ggttktxxe.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gbyzoeadb.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/gwwbjvcia.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gzjuubdgw.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gtpsjfmmx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gwsupopjb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/ggratplqo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/ghvrctqsb.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/goorkpgtl.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gsplcgsdz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gjhjzvolk.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/gykmakchm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gmdxivmbd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gvjdorhvn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/gayqxmpgx.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gagsjyotr.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gzlxptwne.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gcxztzxaa.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/ggrnwywne.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/gxstxuirg.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gmuznrwxk.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gnvdnnzkz.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/gkvthbuhq.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gvooqkore.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gtaveghpw.sHtML


<!-- 参考信息 -->