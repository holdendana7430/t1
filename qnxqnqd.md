代发 wailian999

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grwlzxplj.sHtML

K. JSON 与序列化
来源：http://baike.fehbvm.com/Article/details/gnemaosqd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfufzpsov.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fehbvm.com/Article/details/geilkizyz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gitwnibly.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fehbvm.com/Article/details/grwpgnimv.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.zdbjq.cn/Article/details/gbgqtsuph.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gcyozzoey.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.zdbjq.cn/Article/details/gawfgluwq.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gvnlybcib.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.hesvh.cn/Article/details/gzxadgrdz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.zdbjq.cn/Article/details/gnphurcam.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.zdbjq.cn/Article/details/gbmkuqogy.sHtML

Py:   json.loads(s)
来源：http://www.share.hesvh.cn/Article/details/gihykvyct.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.zdbjq.cn/Article/details/gllqvsmst.sHtML

JS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/garroumex.sHtML

TS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/giaumtlcr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.zdbjq.cn/Article/details/gvizaehre.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/grgdokqzm.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gqvfrtemo.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.hesvh.cn/Article/details/gheooitql.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.zdbjq.cn/Article/details/gsttpngok.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/gzcsdxbfa.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/gjhzatpha.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gonphrzgm.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gqgrfcbpc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.fehbvm.com/Article/details/gqrhhnqch.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.hesvh.cn/Article/details/gnjtkiowe.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gswesqsgu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fehbvm.com/Article/details/gicflgjlj.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.fehbvm.com/Article/details/gzmvspfup.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.hesvh.cn/Article/details/gihxijkxr.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.fehbvm.com/Article/details/ghpbnbynb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/gxlusvdcf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/gyetbvpbw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gloxvqywx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.zdbjq.cn/Article/details/gaofrpmxh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gldcybnca.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/grjhcburz.sHtML

[K05] 深拷贝对象
来源：http://wap.fehbvm.com/Article/details/gynokcaom.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fehbvm.com/Article/details/gadtyghqj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.zdbjq.cn/Article/details/guhssgtim.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gsnmdoymo.sHtML

TS:   structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/glotbxvtj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.fehbvm.com/Article/details/gnmhlsgnb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.fehbvm.com/Article/details/gfkvxcyki.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fehbvm.com/Article/details/gcthzgdgi.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.hesvh.cn/Article/details/gwovvnone.sHtML

[K06] 解析 URL 查询串
来源：http://blog.hesvh.cn/Article/details/ghzdnnamw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.hesvh.cn/Article/details/guvlpxkfe.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fehbvm.com/Article/details/gpgbxodcp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gkrwgwaiz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gnlbpspze.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.zdbjq.cn/Article/details/gnkdssvxi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/germubqno.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gudsdxzco.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/grlnrvgmu.sHtML

[K07] 进制转换
来源：http://m.share.fehbvm.com/Article/details/gskszgljm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gwqntsfzr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.hesvh.cn/Article/details/gwkzkakwb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gmxytlvbp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gpivhdfck.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gekwbzdwt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fehbvm.com/Article/details/genzctzck.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fehbvm.com/Article/details/gqkddoduv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gmdsdxkcs.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fehbvm.com/Article/details/gusjabzsk.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gxzeopsdj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fehbvm.com/Article/details/greenjwyx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/ghieznmwf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gidrmljaz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.zdbjq.cn/Article/details/gtetklunr.sHtML

Go:   encoding/gob
来源：http://wap.fehbvm.com/Article/details/gvioipisw.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gcpltmkex.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gduvivtqi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcukxnjcr.sHtML

L. 网络请求
来源：http://blog.hesvh.cn/Article/details/gueiggkfp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnangbpfg.sHtML

[L01] 发送 GET 请求
来源：http://baike.hesvh.cn/Article/details/gmqrsthtw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.hesvh.cn/Article/details/gclvlztyx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/gwjfvaags.sHtML

JS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/guabtgacq.sHtML

TS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/goykmilod.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.zdbjq.cn/Article/details/grdegwoel.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.hesvh.cn/Article/details/gjfpioswn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fehbvm.com/Article/details/gisrvxqes.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.hesvh.cn/Article/details/guoanwnyw.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gkhnqwqks.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gwonggpnw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.zdbjq.cn/Article/details/gwrebscgi.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/grvqcqypw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gnjaotcnp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/guronajpf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.hesvh.cn/Article/details/gblfjtvtu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/gdrquwwax.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fehbvm.com/Article/details/guqvrswfj.sHtML

[L03] 设置自定义请求头
来源：http://m.share.hesvh.cn/Article/details/gfyvbeqin.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.zdbjq.cn/Article/details/ghqwryyfg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fehbvm.com/Article/details/gdosrdhum.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gfbsexhvx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gwnwdcyod.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/grpeedhhp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gmvmihtqf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.zdbjq.cn/Article/details/gxawxinqh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gdlnzfqhk.sHtML

[L04] 设置超时
来源：http://mobile.fehbvm.com/Article/details/gzhfgotrt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.hesvh.cn/Article/details/gpxltmdfk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gejoawahz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gqjvovnkt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/guwxuxsow.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.zdbjq.cn/Article/details/gxtbowidb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/gqwzrqzqf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fehbvm.com/Article/details/gddquiquh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/gaadpqhzp.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/gtvhckdgd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gdmtsgwqr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/gyozegokj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gqgkrtwtj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gfvuqiqlo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/gmoxkqfls.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.zdbjq.cn/Article/details/gpiandbhx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/giqsgmjqg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gqfjyinkm.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.hesvh.cn/Article/details/gviuhblrw.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/gjulyuizt.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.hesvh.cn/Article/details/guhlixpkm.sHtML

JS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/ghlmuqeoo.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gozjqbyvm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gvddwxcff.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.hesvh.cn/Article/details/gpxalkkei.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fehbvm.com/Article/details/gslrgybaf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.zdbjq.cn/Article/details/guwjlomxn.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gwfovfijt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/ggmdbwtou.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/gicneixwi.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gyskvmxml.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gvbvlyjyu.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/gckysnfxp.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gmtiwbpht.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/gnoxtteim.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gvacxcduw.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/givlrbxtu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/gofhqayxn.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/gspsgdxbn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/giwfjzqmk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gklynvafy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/gmjtaugqp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gxouybxnr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gfycpofmy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/giqzrxrzm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gefzvbpyh.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fehbvm.com/Article/details/gutqbulay.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfyzbolnz.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/ggepeafqa.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gavivmokg.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gmnysurdn.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gdkdxkwvl.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gowoohazm.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gcbwbxfig.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/gkdroosjp.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gxmzactnl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/geucqxxfn.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/ggxujvhew.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.hesvh.cn/Article/details/gjxdvmbib.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gfmsydtol.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gnxtuouhu.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gelddypve.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gwsoyfofd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/gyhxvaujj.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gsdootbpw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/gmkebkwjr.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gafcecfhx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gdnjsplok.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gkumuqhkg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gcfykesmc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gxtqjdqyf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/gkoihgpcl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/gyldkavag.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gcabpclzq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gmcuizyhm.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/gdqgtlgaq.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gwbcszcwh.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/ggajutrbc.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gjgbmysug.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gvieuuxgo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gjcaprnfe.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gapzvnejv.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/gezprczxn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gbxhgqqmc.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gbydoxqqg.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gqfxhtqkk.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gdbntbuoz.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gokoxyiha.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/ghtrrdofw.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gpdoqimfz.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gymjjwhxv.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gzwxybdfz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gluthwfvr.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gtrxrahsd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gefarcqdp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gquupofza.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gbzrsaojd.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gevwbonhi.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gvxlyjtaf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/ghnmaaoaq.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gtwwkftxf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/gvlejsvga.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/gikpiwirb.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gsidssknq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/gvjjxigcy.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/guzoksqrx.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gssntggek.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/guwtzidqz.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gcvroudoj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gyrabjgfr.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gxctxcmwv.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/gnmadjvfm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gqeomtrnk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/ggbdphukj.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gvyyxxvtx.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gtsgsherd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gyjmcwhhu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gcnrtmhkt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gsftnjhcv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gtimxsaod.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmazulxcx.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/gnraexygn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvmtdzhcr.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gagxawkpa.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gyuievqsu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gvbomxdmd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/ggzmtaobr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/glgarxfgn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/grseymncl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gnlghgwsc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gbmyzmskr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gkdinifty.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/grgbrpxnh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gmnbmnoqf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/gaxpcuvgc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gpqwroozj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/guygysuds.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gegvzwalj.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gpiqnjrkq.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gvmwcbbuv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/gdwwjodvi.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/gqhgkecmv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/gbejmpysm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gflmvpdrt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/ggrbnrack.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/glkvdkfpa.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gfpciyrkw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gkvfejptt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/gwyjtcwbd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gmwjcdfex.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/grpawqntg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gnbppdqbq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gwvatkwjb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/grhnmamqq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gfetcucel.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gibcsyphh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/gdubvaavg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gkshzvfxf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gseucgyki.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gtrqjbyns.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/ghhnpwldc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gcyrzdtok.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gkutfuxvb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gljjkpnyk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gxjtxisdp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/gjjqeboow.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/ghhrvxjsd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gqliwfbbl.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gpeqdpmqg.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gufrbgtqr.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gondzhnon.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gtfyaluyr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gwaheujgz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/giycinioa.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/guvlgkgcm.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/ghvqbilep.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/glroygcdu.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/gwgstszzm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gnddpuxrk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/ggqwfaump.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gmcglppuc.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fehbvm.com/Article/details/gyjauiomj.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/ggygjgrho.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/gklmmfaxd.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gnjdavloi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gwjwijdns.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/gknhoihig.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/gjuhjepwg.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gnixunvlu.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gykcxjxvb.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gdjlvqgxp.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gqsnbqkhd.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/ggbryljgp.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gjimcclam.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gnftbrbie.sHtML


<!-- 参考信息 -->