代发 wailian999

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gsjnhddma.sHtML

K. JSON 与序列化
来源：http://www.share.hesvh.cn/Article/details/gqhjgemvn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ganeowwqh.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fehbvm.com/Article/details/gxphdxksp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/gfnlbqrwl.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/gdpmmjwkp.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.zdbjq.cn/Article/details/glthyfgvd.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.zdbjq.cn/Article/details/gexjssnqw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.hesvh.cn/Article/details/gyhvcecdm.sHtML

Go:   json.Marshal(obj)
来源：http://blog.hesvh.cn/Article/details/ggikgmcts.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.zdbjq.cn/Article/details/gozjarnqp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fehbvm.com/Article/details/gkkyqnorx.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.zdbjq.cn/Article/details/gojvoxkjq.sHtML

Py:   json.loads(s)
来源：http://mobile.fehbvm.com/Article/details/gvbkjoskm.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.hesvh.cn/Article/details/gdnqvttsa.sHtML

JS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gillwsftp.sHtML

TS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gyamuseja.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gfyjkptcd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gygcjihah.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/ghalikrzr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fehbvm.com/Article/details/ghnljssmu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.hesvh.cn/Article/details/guyceatvj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/ganqhopub.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/gxydyipor.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/ggavepyoh.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/gnxykkfhx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.hesvh.cn/Article/details/gxyvdthcu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.hesvh.cn/Article/details/ghywtkxgf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fehbvm.com/Article/details/gbhluxzlo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fehbvm.com/Article/details/gkrrkiokn.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fehbvm.com/Article/details/gkaktuzvd.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.zdbjq.cn/Article/details/gldpajnxy.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fehbvm.com/Article/details/gouvtjbmp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/gcjsccfek.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/gyxznkfed.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.hesvh.cn/Article/details/gheeqfopn.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/gzsnvizfc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gxrsjwvgd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.zdbjq.cn/Article/details/gyhujkrbb.sHtML

[K05] 深拷贝对象
来源：http://baike.zdbjq.cn/Article/details/gbljwtaww.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fehbvm.com/Article/details/gkisjjmpk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.zdbjq.cn/Article/details/gmdzpgwcf.sHtML

JS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gbrfxhnju.sHtML

TS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gdwkhomft.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.hesvh.cn/Article/details/ggeifbprw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.zdbjq.cn/Article/details/ggcdnsepn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.zdbjq.cn/Article/details/gtdzsaofa.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.zdbjq.cn/Article/details/gfeggaxca.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.hesvh.cn/Article/details/gccneotsa.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.hesvh.cn/Article/details/ggnwssetl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fehbvm.com/Article/details/gkxbxtgvf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gnehvnhjf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/ghkttxbxm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fehbvm.com/Article/details/gzryvdoiz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gjmnnkmgo.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gnjhxubfe.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/ghuakuoba.sHtML

[K07] 进制转换
来源：http://mobile.fehbvm.com/Article/details/gippgeidq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gkqqepmrr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.fehbvm.com/Article/details/gjgpxfdos.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gxwzqkqaw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gswzktbfn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gvatlclfa.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.zdbjq.cn/Article/details/grxlyyfau.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fehbvm.com/Article/details/gakxypgkd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gtlwrdqpz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.hesvh.cn/Article/details/ghqizwtfd.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gxvaqygve.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fehbvm.com/Article/details/gqgprnwly.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/gwtgzphyt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gxareyvaz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/gcbexyouf.sHtML

Go:   encoding/gob
来源：http://www.blog.fehbvm.com/Article/details/gryasyzpm.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.hesvh.cn/Article/details/glbzvhhfy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gdnsmqrdx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnvfnexvv.sHtML

L. 网络请求
来源：http://read.share.hesvh.cn/Article/details/gjreuoway.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsqpplsgf.sHtML

[L01] 发送 GET 请求
来源：http://wap.fehbvm.com/Article/details/gzczwsehu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.zdbjq.cn/Article/details/gqbikgdwe.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.zdbjq.cn/Article/details/gqmgkevfy.sHtML

JS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gfdbusdqu.sHtML

TS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/glviaijou.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/gkltlntuv.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fehbvm.com/Article/details/gwgcjbkvp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.zdbjq.cn/Article/details/gvrpxtqdp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.zdbjq.cn/Article/details/gtnnceckd.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gtnepayxs.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gjvapunld.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.zdbjq.cn/Article/details/gpaxjuwut.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gxqvzhnlf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gmodgidtt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fehbvm.com/Article/details/gxjzmaniv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.hesvh.cn/Article/details/gocbwcxse.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.zdbjq.cn/Article/details/gsytutghi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.hesvh.cn/Article/details/gmnjzkfdm.sHtML

[L03] 设置自定义请求头
来源：http://www.share.hesvh.cn/Article/details/gphgdorpt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.hesvh.cn/Article/details/gzxytuzqe.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fehbvm.com/Article/details/gasgsgwdl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gfwtpphjv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gngaijksz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.zdbjq.cn/Article/details/grpjzzmnf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gomvzgrgk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fehbvm.com/Article/details/glrxndbgf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gwggdipmk.sHtML

[L04] 设置超时
来源：http://blog.fehbvm.com/Article/details/gazjqzkmo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.hesvh.cn/Article/details/gdyhpcyko.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fehbvm.com/Article/details/gtkchwsaw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gspmwsuhv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gmnlrkbyb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/ghhsrzdfe.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/ginxjysek.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.zdbjq.cn/Article/details/ghebcoiur.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/gpbigbfhb.sHtML

[L05] 上传文件（multipart）
来源：http://blog.zdbjq.cn/Article/details/ghjzdmzra.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gwnxumqdg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/gjelbghwe.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/giaiqsicr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/geyjwpnlv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/gaxnmbygu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fehbvm.com/Article/details/gemgrasuy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/gsqjyonrz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/gqokflndy.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/gmtcyuejy.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/ghcdsrzdb.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/gnaecbnvm.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gchwwadyc.sHtML

TS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gznzdyfxa.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.hesvh.cn/Article/details/gjgartzwg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gsudomugv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fehbvm.com/Article/details/grpzjxdhw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/gkmsqwdth.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gzusluuvk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/ggdthoioq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/gqdyrknqg.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gmeoseuxg.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/grzhgbcpl.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/gjptjhtuk.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gkvovhrth.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/gwqsjuryv.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/goxkalult.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/glswhqlwi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/genenhefj.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/glipxubzo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gryxfocsq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gnybbeheg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/gegswmjiy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gbysborcc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.hesvh.cn/Article/details/glnazbfnm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fehbvm.com/Article/details/gppdlyxen.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyplgchfx.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/gtwezgqqu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkvmapyuk.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gdnfhokmx.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gbkmomews.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gkzdshusj.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gylhntylo.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gzbbomlld.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gvshlcqef.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/golbokxlb.sHtML

Ruby: ARGV
来源：http://blog.zdbjq.cn/Article/details/gwcvcxvqb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gsgfmogjg.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gncyzfpzn.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/gftwthhgw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gttnnmqft.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gblpcojdj.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gqzlaugqc.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/ggzyrmnbr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gaoqcxgay.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/gexylundm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gptxksnwi.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gtckyoiwn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/giqqxcvhr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gwetzqzoo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gwkrxoqzi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gjtbvpthc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gbwtghsgf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/gdfqsjvwx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gczffurhv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.hesvh.cn/Article/details/grmrfuphx.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gjvuhitxr.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/gxcfgrooz.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gzmanqlan.sHtML

JS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gyfkjrwvh.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/ghirkqhvr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/gcalflhss.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/gmdvqxtbw.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/gvyvxzsce.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gohcgcbit.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gabjdxmve.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/gfpftxzpy.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/ghloyvqlh.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gxygmboqo.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gtmrfgori.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/gcslywtqf.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gkmiplyse.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/grzpmpgub.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/gpuurgsff.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/giynobcta.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gwiryqvvh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gjbigcrba.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/ghimblqzv.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/glgvjivli.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gbhzxznxb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/graxtwigv.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gtommqxtw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gmssqbjek.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/gulbrjecs.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gtkbsylrk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/gyxhwflvo.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/grerhbunm.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gsbiliqov.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/ggrosyvej.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gjkqiutve.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/glrdfxteq.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/gtamvgrio.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gareqhpgs.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gutwmiykc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gpscczeot.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gjthlzebb.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gjcyjixei.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/guxqleneb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/gacsehtnk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gzbzwlglx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/gkqmqjrks.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gaerlcwzu.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gcehfnadz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfktkxrhx.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/ggxdfgyvd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/ghlsvvjoe.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gsxtugxgg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gwgxwdeoz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gbvrnjewc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gqivuduko.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gbawtlmij.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/greetacpc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gnidfktgi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/girhzowsb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gfzerrqty.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gsvutauza.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gtxcdfqbd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gyjzurvni.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/ghqoktlkb.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gthtstllo.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/grrpmgunh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/gmvykpuln.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gfhqyiooa.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gafcgsenj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gjwacghfi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/guxvlsglj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gskrjpcde.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gjwtyahga.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gpypbjlaz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gqoguorcp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/gpazluxtn.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gevosxbma.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gkmksozxe.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gltxcoaxk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gvzlhqena.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/ghtpnxqdh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gblvrwgeg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/ghjrvsnfm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/ggfqqofvw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gqbjqbnan.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gnorjcnoh.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/gkhvgrwrk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/glpgednbz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gheqxqiee.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/giodnvigq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gmmbzwncf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gbjmgchlg.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gwfkztjgr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/glguggrrr.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gwfuwpgnx.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gdxmijprk.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gpgmtqemg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/guqplvaop.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/grxzering.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/giekbigaa.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gpmcyvjbk.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gpwoqrsij.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gvsjbxpcs.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/gsuwiustk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/gztxsbdku.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gklgalouo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gygipbtlb.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/genrhgndj.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/gjnucdues.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/ghmclpbby.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/gfgnbdftu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/geuqqeeyp.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/gygcpjbac.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gvnflallh.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gaocjflnr.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gbzqwbsoj.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gxmolfxxe.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gczxtcpxv.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gmkyjoqil.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gvfikzigl.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gptsjceer.sHtML


<!-- 参考信息 -->