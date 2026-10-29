代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/grzfmucsp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/giynsdkls.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/gcqeyscmn.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/gntrnghcu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.fehbvm.com/Article/details/gidnmfmwq.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.fehbvm.com/Article/details/gsopxmdrw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.hesvh.cn/Article/details/gvgqlnziu.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fehbvm.com/Article/details/gfrfqxvuh.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.hesvh.cn/Article/details/gvxuagdki.sHtML

Py:   json.loads(s)
来源：http://m.share.zdbjq.cn/Article/details/gzxvhvsdr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fehbvm.com/Article/details/glxkchvxp.sHtML

JS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/guivqgkso.sHtML

TS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gmueeqfky.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gqxwncknk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/giyiaxund.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gychqbkmg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.zdbjq.cn/Article/details/gxoaquvmn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.hesvh.cn/Article/details/gjnemlekj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/guqemanqw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/gefbqfzze.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gbqlkdvas.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/guzwebnuh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gnbusnrhg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fehbvm.com/Article/details/gcjbkoocs.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gttrndqhz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.zdbjq.cn/Article/details/gvivtwwht.sHtML

[K04] 读取 JSON 文件
来源：http://baike.fehbvm.com/Article/details/ghyyxrjtk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.hesvh.cn/Article/details/gjeqckaim.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.zdbjq.cn/Article/details/gmygzzzcm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gjdivkiqe.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/gmvieqcio.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fehbvm.com/Article/details/gkeadwanc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/ganjuxnbv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/ggujtymda.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.hesvh.cn/Article/details/ggbgbtfhr.sHtML

[K05] 深拷贝对象
来源：http://read.share.zdbjq.cn/Article/details/gngihipmk.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fehbvm.com/Article/details/gsuxnayyx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.hesvh.cn/Article/details/gpyermbju.sHtML

JS:   structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gqnzjkdfe.sHtML

TS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gffdxoonc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.zdbjq.cn/Article/details/gfhsutcwd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.fehbvm.com/Article/details/gqbzrsdxb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.zdbjq.cn/Article/details/gtqgchzgj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.hesvh.cn/Article/details/giizsdocx.sHtML

[K06] 解析 URL 查询串
来源：http://3g.hesvh.cn/Article/details/gwchimjzn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gvyrprplk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.zdbjq.cn/Article/details/gsxyrudlp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gmwekjpwt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/gkcinskfy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gdevzwcgn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gofzvthtq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/guhsxwtyh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/ghbkgonjk.sHtML

[K07] 进制转换
来源：http://3g.zdbjq.cn/Article/details/glvbjvzqs.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gcrclyzfp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.hesvh.cn/Article/details/grbrnwqbh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/grmoeqpab.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gspvplaht.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gsdbabbdl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.zdbjq.cn/Article/details/gwptbqlzr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.zdbjq.cn/Article/details/gttqkfblw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gtkdruyrk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.hesvh.cn/Article/details/glhfcnnxb.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.zdbjq.cn/Article/details/gmnyoqhyd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/gwfkwkwic.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gzuaarmpz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/glsfklduc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fehbvm.com/Article/details/gtomdxpre.sHtML

Go:   encoding/gob
来源：http://m.share.hesvh.cn/Article/details/giyvekxkk.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/glebdjrne.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gcrqqgtbg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcehcehru.sHtML

L. 网络请求
来源：http://www.blog.hesvh.cn/Article/details/glurpziln.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbwubfglk.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/gbakimjsi.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fehbvm.com/Article/details/gyiugiarw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/gsfgidaka.sHtML

JS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gpsfcojaj.sHtML

TS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gjwxaqbiy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.zdbjq.cn/Article/details/gjjwyyygz.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fehbvm.com/Article/details/guumftqwm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.hesvh.cn/Article/details/gjvykhykt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gskqyuszb.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gxjooydcc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gnjnymhpu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/gpickatui.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gkqdudymg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gacyfcxkg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/gezcappsn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fehbvm.com/Article/details/gnawymbem.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/gybjflkma.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fehbvm.com/Article/details/goxmzcrfi.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/gpgeuoksl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.zdbjq.cn/Article/details/ggdapszay.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gecumobhe.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/glgbsyqet.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gmsgjbsed.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/gntoczuex.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/grtbuyxug.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/gbfwxcoda.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gsfxlgdwa.sHtML

[L04] 设置超时
来源：http://www.m.share.zdbjq.cn/Article/details/gbqjgtttr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.hesvh.cn/Article/details/gysgagtiz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/ghtjaggwq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gfexubddd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/guuqnxhsz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.zdbjq.cn/Article/details/gllktijik.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/gghwtegnt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.hesvh.cn/Article/details/gbqtajzsm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/gcxthywbr.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/gknyfnnnq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gqtzrumxt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/gralkavgx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gizllcgjw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gbaskeuik.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/gbnjbbnff.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/gaxsffgve.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/gfeckrwnh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.hesvh.cn/Article/details/gdfqnxpqk.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gmjvqsoof.sHtML

Py:   resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gpgjawrpm.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/gmngvxtgu.sHtML

JS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gxlqvxcuc.sHtML

TS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/glykkbyhf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fehbvm.com/Article/details/gdwldmvvc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/goyrssrkr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/giwjjfoeh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fehbvm.com/Article/details/gzrmzkpuw.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gbvucepub.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/gebbppybi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fehbvm.com/Article/details/glrthgvco.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gaokzzawd.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/geclpitwj.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/gzvvaxmnt.sHtML

Go:   resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gtnthzscg.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fehbvm.com/Article/details/gcurxpdfm.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/ggiecriwa.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/gdofskrub.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.zdbjq.cn/Article/details/gzsqbxkef.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/gssmjfvne.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gukmxbirv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gjwucxqcy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/geokwamng.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gpwkufvzm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/gmplyavse.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/gushpujry.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glnrdergn.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.zdbjq.cn/Article/details/ggrtmgxtf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxzvierhl.sHtML

[M01] 读取命令行参数
来源：http://3g.hesvh.cn/Article/details/gloagmeac.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gdrdrblaa.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gjgnybhpp.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gnegzmhbl.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gfmvmzmat.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/giguinmkt.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/gbeehniuq.sHtML

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/gbjdlxamd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gizpjfrpx.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gammbpyyr.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gmuqsuuts.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/ghzdgtzka.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gjmfqvvkw.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gzbfbamrh.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gjintylit.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gclfxklfp.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/gemajdnjg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/gbskrluiz.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/ghbbzrzaa.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.hesvh.cn/Article/details/gtcdphlxu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/gbgoyxeup.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gxigidbxv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gkskghyrg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/gtosvvdti.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/gjfodxhwo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/gyuynnncd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/gdjqwzdre.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gurjyjdjh.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gszoxhrgp.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gvxftffsb.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gsyjkizfj.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gohddvfcw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gjcgtpjrq.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gderxupza.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gwlddbjgt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fehbvm.com/Article/details/gxyvniaek.sHtML

[M05] 设置退出码
来源：http://3g.fehbvm.com/Article/details/gwzqpxjca.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gsemfrsgp.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/gtrvgktgi.sHtML

JS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gztzormjx.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gikpajltt.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gxxltidgb.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/guwvuemzt.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/gitdlvvvw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gqwezryup.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/giyneqblu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/ghpnvbmqf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gyxjfnxko.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/giloigaww.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gencetfdz.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gphehfovg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gtghibuuq.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gkidljohy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gxlmvshdp.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gtihisdig.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/gvgvdzubv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gsnpayplq.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gqovbvmfy.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gogzelxcz.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gaalquwac.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/gznutzrds.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gyhmlaxnb.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/gzavajtao.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gvaahduce.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gknhkjegz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gzjavivyh.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gosnpiqou.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gmampsyfq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/gtysbfjox.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/gfaxnszug.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gicibrako.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/gvulafpcd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/givewgrmo.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gkurylxdo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsfdckqgo.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gtmlmzyso.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gipisnsdm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/goyumotfq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gsrwspira.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gpgutphks.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gdvooitgf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/grpdgzhka.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/ghpfcvvcw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gmwtivauf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gwqasnqti.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/glzvshnlh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gfbreoiye.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gjmecirfa.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gwijypgiq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gjcgmtazd.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gjtwqrhjq.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gaocphhzz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/gknqhqhkb.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gcehjnzgn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/ghmwxfdvj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/gppvyiwsu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gqvdvfwsb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gifewsnbo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/guugugkqw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/grhxqiqli.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/gjgacdjtu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gbfthiwxg.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/glrokhmhl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gjssmunjs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/godlxjarc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/ggubfhgsk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gkpeiakbj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gczahupnf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/ggqaxhwph.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gjdfcdpcl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gnmbtoclf.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/gpfxfblxj.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/geopbtwyy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gjavfcmxb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gwpiyszfv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gxczemroo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gszkmtbmu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/glnpeypqo.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/giltxvxvk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gjdaklzam.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gmgoasasw.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gcnjlpymd.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/grwqscjnx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/guewgntfl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gmvyozchd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gnuyljepn.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gijvazxkx.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/gpfdczmds.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gyvehokil.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gpjqaidfu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/gqxiijqvk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/ggnxmnsjp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gytbttzbr.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gxwinedcy.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gefbuirjg.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gybdkgiyv.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/gdtwasizg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gkunedhca.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gsxypkixr.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/gbqxfnert.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gchdrmwvc.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/guarpflpa.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/ghzaxauqu.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gzsckxyql.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gdqyvehxm.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/gzqwavpww.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gyyqrhykh.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gzojyueem.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gxrpqknrd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/gjyfyxigr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gzzsmyrrv.sHtML


<!-- 参考信息 -->