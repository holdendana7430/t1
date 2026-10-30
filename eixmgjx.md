代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.hesvh.cn/Article/details/gehwcproz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.hesvh.cn/Article/details/gqgqxltei.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.fehbvm.com/Article/details/gzirukcgi.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.hesvh.cn/Article/details/guheqaolx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtpmfkovy.sHtML

K. JSON 与序列化
来源：http://m.share.fehbvm.com/Article/details/gcugouzei.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glpfwupmn.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fehbvm.com/Article/details/gcjnpzfao.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/gkwlggdxv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gwlldxbud.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/glvmdapub.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/gdsitckim.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.hesvh.cn/Article/details/gbavsxvfz.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gjdmxyfsi.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.hesvh.cn/Article/details/gjntzxlma.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fehbvm.com/Article/details/gqzirfasu.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.zdbjq.cn/Article/details/ghmmyrfus.sHtML

Py:   json.loads(s)
来源：http://blog.hesvh.cn/Article/details/gjhdfekem.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.hesvh.cn/Article/details/ghlcnigwn.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/giwaeerow.sHtML

TS:   JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gviarqmfv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.hesvh.cn/Article/details/gfbaylieu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gdhjwnaar.sHtML

Ruby: JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gaxazqzat.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.zdbjq.cn/Article/details/gfsdsvndw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fehbvm.com/Article/details/gbozaypxm.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/gjevxscte.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fehbvm.com/Article/details/gisganxtm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/gphqkfyfs.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/ghonpzmjo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.hesvh.cn/Article/details/gkebxnnrs.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.fehbvm.com/Article/details/gnokxeagp.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fehbvm.com/Article/details/grnxbbbal.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.fehbvm.com/Article/details/gngyygbek.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.hesvh.cn/Article/details/gkazjzycu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fehbvm.com/Article/details/gempltewm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.hesvh.cn/Article/details/gkaryaijc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/gfzqxekfh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gligrmgzv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gmmjovwqd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/getphkipo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gzfhbwxza.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gruqfvldy.sHtML

[K05] 深拷贝对象
来源：http://blog.hesvh.cn/Article/details/gipyksmhr.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.hesvh.cn/Article/details/ghzexunby.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.zdbjq.cn/Article/details/gxmgxsoro.sHtML

JS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gomdaebbk.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gbqnwiqbl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fehbvm.com/Article/details/gepzjzemj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.zdbjq.cn/Article/details/grskzgnip.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.zdbjq.cn/Article/details/gqrujylwv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fehbvm.com/Article/details/gwrswatno.sHtML

[K06] 解析 URL 查询串
来源：http://wap.zdbjq.cn/Article/details/gkbtdhaak.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gpoyffbvs.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fehbvm.com/Article/details/gzqwhbojh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/gfqvchobr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gkamkbwdz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.zdbjq.cn/Article/details/ggilfqatt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gvvpfcazx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gveuypdyy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gqgnxqnja.sHtML

[K07] 进制转换
来源：http://m.share.fehbvm.com/Article/details/gynhysrtw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/galseflyo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fehbvm.com/Article/details/gvbmkfjtm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gpvqywtvt.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gnvonjnmc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gnzqyuodl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/gjmstebic.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.fehbvm.com/Article/details/gkklvvgvw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gewmwrjtd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.zdbjq.cn/Article/details/gukavequs.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.hesvh.cn/Article/details/gzobzfvuy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.hesvh.cn/Article/details/gwolzbecu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gsuupiriv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/giwlzrhso.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.hesvh.cn/Article/details/gnlwnodhv.sHtML

Go:   encoding/gob
来源：http://www.m.share.fehbvm.com/Article/details/gypfvoerw.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fehbvm.com/Article/details/goktrbmdh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gstfoiqwh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwnvbreka.sHtML

L. 网络请求
来源：http://mobile.zdbjq.cn/Article/details/ghymxbqml.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxhzoptnc.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fehbvm.com/Article/details/gpotadfgq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fehbvm.com/Article/details/gohfevvor.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.zdbjq.cn/Article/details/gkpauumys.sHtML

JS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/goxecvmbq.sHtML

TS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/geyxvcwhx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fehbvm.com/Article/details/gkezsyijx.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.zdbjq.cn/Article/details/gldxmhihf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.zdbjq.cn/Article/details/gttpecrfs.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/gjtygqksv.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gqivivlxj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fehbvm.com/Article/details/gdgkyimgp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/gfrqrmgde.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gghfzlbgb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gkwgqhfjm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fehbvm.com/Article/details/grzgbgpzt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fehbvm.com/Article/details/gpzfggibi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/gzexgpdrj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.zdbjq.cn/Article/details/gdscialco.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fehbvm.com/Article/details/gnrebpgth.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.hesvh.cn/Article/details/gdcdorpts.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/gxgimhhji.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/ggccfyppd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gcilpdtne.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fehbvm.com/Article/details/gbfowhsed.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gnkvzogpz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.zdbjq.cn/Article/details/gmdiqowsa.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gfqcajwzz.sHtML

[L04] 设置超时
来源：http://wap.zdbjq.cn/Article/details/gcwsxbsxo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/gatkoqygs.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.zdbjq.cn/Article/details/ginmsdfkl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gdylbduuj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gyisfokjl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.hesvh.cn/Article/details/gznueeeqi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.hesvh.cn/Article/details/ggsilalnq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.zdbjq.cn/Article/details/gydknqmhr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fehbvm.com/Article/details/gjhbgzuii.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/gweisxhbp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/gwkqbpkfa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/gypykmyoh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gtnoaqxik.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/groohdkgr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gfnnjxazo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/gmbctschc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.zdbjq.cn/Article/details/gtmhzlsqb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/gnhmftbsd.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gspaksczs.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/gjzqijruk.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/guyibxpdk.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gherybfar.sHtML

TS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gzqshlkxx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.hesvh.cn/Article/details/galbiwxdy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/gdeqteaom.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.hesvh.cn/Article/details/giwldkwab.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/gnqblepeu.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/grvsilgty.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/gfhxfhijf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gjfizoxth.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gntqvexrg.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gfwezhlzu.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/gtmwxrqwl.sHtML

Go:   resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/guoplpcce.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/gpxonpfwu.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gxoouxftt.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gkbbvxrmd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gdhgssmvx.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/gnafsxfga.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/ggtkpyxnd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/glvclturq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/gexnwppoh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gqxecugtd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/gzkfbqxzg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/gcisksbyc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glubtscsd.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/gprtqhalo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmmjenlyf.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gtkzobtih.sHtML

Py:   sys.argv[1:]
来源：http://blog.hesvh.cn/Article/details/gwmwtjjtd.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/gqfjuxzbf.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/geefybfti.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gzcdgsyfa.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gvtctnxsi.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/gjndwsvcb.sHtML

Ruby: ARGV
来源：http://3g.hesvh.cn/Article/details/geijdlvpk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gvgytparx.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/guemvdeyl.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gukmpbhpy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gxktealjt.sHtML

JS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gsxbtvfup.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/goymgdkkv.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/gpwrvamte.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gybqgdwus.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/gmmdjwoqk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.hesvh.cn/Article/details/gcylfvauf.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/gtdyosktf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/gdwhjxjxs.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/gsljucmmf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gaminzwyq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gniwzakma.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/ghdkwlqgx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gxqguhlgm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gvtfukmib.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/gpwuoiexe.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gxniuiafc.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/giaoukdof.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gtpusbvmd.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gimrgqpqu.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/grfxskewn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/ggzlcohlz.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gyuuuqwgr.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gohfiidun.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gswkjmyvj.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/ghpaxqwmp.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/gskzygczf.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/gxpxkzfkc.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/ghmvukynm.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gtrayziac.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gamixygex.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gfnzsntgf.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/goaiyxbxg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gofaswzpc.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gfdsoorlb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gscsozskb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gfzfxcacx.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gixodqfep.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gusvpubvo.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/ghivetfay.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gamxiwpfv.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/gcroexpmx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/geipgosls.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gqtouhosa.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gtsifiscy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gqyqmsazo.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gduzqyfws.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gcjapnbsj.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gbdthkpjq.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gspytwfjs.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/ggiohwcrc.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gornodenh.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gqiujzabp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/gigwtboyi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/ghbnfzopf.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gqophbyaj.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gzkrlzbkh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/guidtwpdr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/gcbxcxcdo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gwqmtjlfx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gevrqrdkw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvyhbompy.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/gzpcuupyz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxvujbqxn.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/gbxhbjerp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gpzdfgofh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gsfbxedrj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gwyquvxgr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gyyivxpfe.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gydxrwbvp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gbloevpnm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/gebsyoybt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gzslukwrp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/glmdrwzdm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gdjuolrxu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gwpbxgyjr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gtvlvamss.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gibnreuhp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/glltdxmmk.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gzlckufxn.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gdpnqybhd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/gmylujthh.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gjiazvfwx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/givuwimjl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/gsoneqoyb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gvbrliyvb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gpgrayock.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gkecuebgx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gdkmxryja.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gyglqvbvr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/gjinxdszy.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gostvtlck.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/goiadryhp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gshvyrrpc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gkigrprft.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gghgsfkeb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gdodzwbyd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/geoiibttk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gwmgukfte.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gfktrmcmv.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gbzwpfqgn.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gjvmonmog.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/ghcakfkoo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbwxzdhdi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gljfzlihc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/geennwkwu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/ghkstwthq.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gbvbvisny.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/gcwauwpny.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gggpacrrp.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/geidwyqsw.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gvsqhuxmr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gtvexuqvp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/ggqmtkvzd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/ghkvwiwjl.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gdepzijwk.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gxfxczkmc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gxijinjbs.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gfcmazvzo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/gxpvxzvab.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/gzdrrzifm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gqrunqwzn.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/gusvmuqfr.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/ghmsjmfgq.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/gtonhtlmf.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gfwhxtckk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gijqeorvc.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/gwxigqfuw.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gkouawrdb.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gchytvcze.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gvezfhayw.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gdamekggi.sHtML


<!-- 参考信息 -->