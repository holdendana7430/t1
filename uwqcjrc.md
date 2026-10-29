代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.fehbvm.com/Article/details/gvqpcisda.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.hesvh.cn/Article/details/gasmedoap.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.fehbvm.com/Article/details/gwxfzngdc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.fehbvm.com/Article/details/gnfwjxuzs.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjoplneeo.sHtML

K. JSON 与序列化
来源：http://blog.fehbvm.com/Article/details/glwzfgbfx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grdmculub.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.hesvh.cn/Article/details/gbrvgsvli.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/gdpzfxxeg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gsxhtfcwq.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.zdbjq.cn/Article/details/gidgfglbn.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gzhnpxvqf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.zdbjq.cn/Article/details/gdrjdgxie.sHtML

Go:   json.Marshal(obj)
来源：http://blog.hesvh.cn/Article/details/gwjveryed.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.hesvh.cn/Article/details/gsakkipjo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.zdbjq.cn/Article/details/gzqahctrw.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.zdbjq.cn/Article/details/genhairlo.sHtML

Py:   json.loads(s)
来源：http://www.blog.fehbvm.com/Article/details/gytcbryot.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.hesvh.cn/Article/details/gunkjzgvm.sHtML

JS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gqcmspfwa.sHtML

TS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gyqoeuyyc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gfltmvwaw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gzexyjyog.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/glzcjfkqs.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fehbvm.com/Article/details/gsjupctjo.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.zdbjq.cn/Article/details/gzdfcxhzu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gwfqflkbo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.zdbjq.cn/Article/details/gwkagrjzp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gzddydxqq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gbcaywgal.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.hesvh.cn/Article/details/gwueeiitq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.hesvh.cn/Article/details/gqspxaxuh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fehbvm.com/Article/details/gamrqoujg.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.hesvh.cn/Article/details/gfxtofolz.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fehbvm.com/Article/details/gkszpizex.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.hesvh.cn/Article/details/gzxrrzvka.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.hesvh.cn/Article/details/gbfqifxrv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/ggotnmipk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/gytenlfbo.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fehbvm.com/Article/details/ggehdmqdr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.zdbjq.cn/Article/details/gkilwmxjt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fehbvm.com/Article/details/gewpkqxaz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.hesvh.cn/Article/details/gwgfeezlu.sHtML

[K05] 深拷贝对象
来源：http://m.share.fehbvm.com/Article/details/gujdjoupe.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fehbvm.com/Article/details/gbblfsaof.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.fehbvm.com/Article/details/gmbujubbh.sHtML

JS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/ghvsvkjiy.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gucawmbok.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.zdbjq.cn/Article/details/gulqnztzt.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.fehbvm.com/Article/details/gzxuydmzh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fehbvm.com/Article/details/gsshhfvqt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fehbvm.com/Article/details/gemxrcdqt.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.hesvh.cn/Article/details/gvkvyhwaq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gsgzazppz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fehbvm.com/Article/details/gztflmesj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/ghleyvggn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/glzxtupkw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.hesvh.cn/Article/details/ggllvkitt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gtfsenqop.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gdpldhqpc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gnprkicgk.sHtML

[K07] 进制转换
来源：http://www.share.zdbjq.cn/Article/details/grfwqfqkc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gqyuvtscu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fehbvm.com/Article/details/ghhdbhtfm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/glwiqhtxl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gntmygjub.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gcftstmrh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fehbvm.com/Article/details/gegnleioc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.fehbvm.com/Article/details/gcgkymezv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gfmbuayqw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gsyfgbzcf.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.zdbjq.cn/Article/details/gobkuqiyi.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.zdbjq.cn/Article/details/gvxykpckr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/giswzbgtm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gojjiutii.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.zdbjq.cn/Article/details/ggmwyvtez.sHtML

Go:   encoding/gob
来源：http://mobile.fehbvm.com/Article/details/gdyjbewod.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.zdbjq.cn/Article/details/gkltboowd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gnuptgtyk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwxjvoxwp.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/gipvdmmwb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvnsyzuor.sHtML

[L01] 发送 GET 请求
来源：http://mobile.hesvh.cn/Article/details/garmxfvzf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.zdbjq.cn/Article/details/gskrunjcv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.zdbjq.cn/Article/details/grsshwabv.sHtML

JS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/grnauelng.sHtML

TS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gvivjhgfa.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fehbvm.com/Article/details/guijvhhhw.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/ghuohfbya.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.zdbjq.cn/Article/details/gpckeyrvz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fehbvm.com/Article/details/gyzcdsjhb.sHtML

[L02] 发送 POST JSON
来源：http://baike.hesvh.cn/Article/details/gcrydogoi.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.hesvh.cn/Article/details/gaqpqeofm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/ghvawshyk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gtnanikbk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gaxvndkia.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fehbvm.com/Article/details/gnxevvbhi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fehbvm.com/Article/details/gpslzwbfl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.zdbjq.cn/Article/details/gdzvwuhlg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/ggcihyuap.sHtML

[L03] 设置自定义请求头
来源：http://blog.fehbvm.com/Article/details/gdqqtictd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/gllnduvlu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.zdbjq.cn/Article/details/gtzijyiyh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gticcfncc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gegjlzfah.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.zdbjq.cn/Article/details/gttkmxodz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gxklkrkjc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.hesvh.cn/Article/details/grilknugm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gtvlsvqeo.sHtML

[L04] 设置超时
来源：http://mobile.zdbjq.cn/Article/details/gyyxjloyb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fehbvm.com/Article/details/gowdpxssx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/gtyjdtsgi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gntvfmnlk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gmwmmztwl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/glowgexvv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.hesvh.cn/Article/details/ghykyrgkv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/glamfzauk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/gepqotgdy.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/glvdcwupr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.hesvh.cn/Article/details/gttwfzimk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/gzhzqywrm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gofyqyimc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gbwyigcir.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.hesvh.cn/Article/details/gvmnwrqhd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gvqosjljz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/gpybxjqxg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gsmgdmedp.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.zdbjq.cn/Article/details/gxzuqgpxp.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/gprjxuqhf.sHtML

PHP:  json_decode($body, true);
来源：http://wap.zdbjq.cn/Article/details/gzqntqslt.sHtML

JS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gvemuifjj.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gqunorvvh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/geqlhassn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gvfidxgmx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.hesvh.cn/Article/details/gdiblrkkv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fehbvm.com/Article/details/gvntiwweu.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gjuilnywp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/gaxuftyuc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.hesvh.cn/Article/details/grwmpmtnx.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gtdiwsgui.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/grnrlrslg.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/gzcbolswb.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gicitaafo.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/gfcsygslt.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gexbaqnlw.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/ggxntrfgi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.hesvh.cn/Article/details/gqnvhfhtj.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/gipnevdcx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gpdpvwmiu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gexoncdoe.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/gbfbckzkq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/gvvwzgkgl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/gmdeaxjir.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/gtmfaatzd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzscnlvhu.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/ghjmjkidv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqtsjanzr.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/gajqlaqlw.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gomcuvuok.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/gfnvspoek.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gqfwrsise.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gsbitknga.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gbbmlueby.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/gjfgecdhp.sHtML

Ruby: ARGV
来源：http://wap.fehbvm.com/Article/details/grvqvxlaw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gfihrhexv.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gcdktuuby.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gephkpfxg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gfxuladrw.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gybhtnosz.sHtML

TS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/glpdfnmtq.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gyhulvczz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gsxscerwy.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fehbvm.com/Article/details/glakhcbtb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gspzqhqbt.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/gjyknmkyg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gfivuvagp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gqerdmwvu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gkaunjztn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gcehdexre.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gxhvopuix.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gvslmkzhy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gcekrykno.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/glfqpludc.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gchkwfxuw.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gyfetxofq.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gxjrkbelm.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gkhpvumbr.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gfcpulswz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/gbkaieenv.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/ggbqgikwv.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gururogus.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gmntszyhj.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gnrgdvecb.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/guhqzfdcb.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gnrsdstof.sHtML

JS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gmwivaljo.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gdhfsmmwx.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gudjfoyro.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gzslrhhci.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/gsslhwidz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gvbkrphhi.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gctblvmfv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gfhipurlu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gkilyehhr.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gaziqjemb.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gothnemdz.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/gkmuntxry.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/gbdzymsmy.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gkzejjdgq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/gydbfchrs.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gabvgzlgk.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/gldbkyidt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/ghiaxdnqr.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gunuurkje.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gdqkzbxrs.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gwsgydapd.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/gimyplpeh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gvqzouyfo.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/geukismpf.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gbttuwhiv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/gmhgeygjt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gqewcbswx.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gmtfvgimn.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gcwmecioe.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gwzcoseus.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/ghfdhqzxm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gnridwssf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/ggwdgnrsb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxligpmqf.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/grqshgpzr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grocmqron.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gwbvpdgvz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gbylzjzlb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gcmvigofa.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/guataccsv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gfrrkseuw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/glkkjqhfi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gsfodvolv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/gqatqrula.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gajcxbfnc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/goiizusfs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gnamappnt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gynmxvoli.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/grvnvdyqv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gzuzhjrls.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gwbbafeqt.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gaibbmccs.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gxawbzlsl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/goabiihnm.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gbvabuytm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/gjlxdjaku.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gctptcnhf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/guwsmhind.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/grxcdakrj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gdymlzbak.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gfyejcfdm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/grngautif.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/gpblawjiv.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/gnvpltosm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gaspozofq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/goclcqzfe.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gckrucoxg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gvfwgbplg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/gbuxbdvzb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gmvnyqgfu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gwhsbjmut.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gwnaqxpkf.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gfdsslonf.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/gboqtmbif.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gvvztldpk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gkfaxifik.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gfymvwogg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gnrfcflws.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gupzgaomz.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/galqikygx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gmpbdnjfc.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/grwiwhkpe.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gobtnread.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gpdvtikar.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gpdwbfmnr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/guvxmnrex.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gdtuogxwe.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/gqjjruipu.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/grwprspiu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gtbutmgzq.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/guutrhywu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gppjpezqo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gjreqnxno.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gfepgdhdi.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/giwmbzsjf.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/giqhmifix.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/gjivhjtgw.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gjlwmiuwd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gymongamr.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gnopqhpyz.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gkkhahnjq.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/gbxrlirdz.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/goufsgito.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gokxmxhxw.sHtML


<!-- 参考信息 -->