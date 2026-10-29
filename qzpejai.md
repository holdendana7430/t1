代发 wailian999

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnvzmnmyr.sHtML

K. JSON 与序列化
来源：http://3g.hesvh.cn/Article/details/gborbarqn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcqzmkgam.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.hesvh.cn/Article/details/gvvigtqyx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/gfqlnegyu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/geccftift.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gdtswyctw.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/gnjslcweu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fehbvm.com/Article/details/gxefxogko.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.zdbjq.cn/Article/details/gmsktechn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.fehbvm.com/Article/details/gsiuqogec.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fehbvm.com/Article/details/gaecwcdqy.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fehbvm.com/Article/details/grplxiamx.sHtML

Py:   json.loads(s)
来源：http://wap.zdbjq.cn/Article/details/gijjqboqo.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fehbvm.com/Article/details/geevsfogo.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gvxnupohl.sHtML

TS:   JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gjzyopeuw.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.fehbvm.com/Article/details/gzdfexzau.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/gzqkicbpv.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/guxjgwdrv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fehbvm.com/Article/details/gtchelxnm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fehbvm.com/Article/details/gnfhpwprd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/gswmddzth.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/gxoxfnmvp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gjgtbcrmw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/gfktgpvrm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.hesvh.cn/Article/details/gnwwifyqd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fehbvm.com/Article/details/gkdsnpjal.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fehbvm.com/Article/details/gihodjajv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fehbvm.com/Article/details/gjwxxrysw.sHtML

[K04] 读取 JSON 文件
来源：http://wap.fehbvm.com/Article/details/gwbkjiadj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.zdbjq.cn/Article/details/guwarsxna.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.zdbjq.cn/Article/details/guovavrps.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/grvbhpmao.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gxbipkfia.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fehbvm.com/Article/details/grjfzmmua.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gljhphlyh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.hesvh.cn/Article/details/gddpaitwa.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gtoofffvr.sHtML

[K05] 深拷贝对象
来源：http://www.blog.zdbjq.cn/Article/details/gkowicxic.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.fehbvm.com/Article/details/gizvmklgy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.zdbjq.cn/Article/details/ggmqtkvox.sHtML

JS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/ghtadpwzz.sHtML

TS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gxgheyuwv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.hesvh.cn/Article/details/gsqpwqvqn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.zdbjq.cn/Article/details/gbzhjbuak.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/gvutqexml.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.hesvh.cn/Article/details/gowdkidfw.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.hesvh.cn/Article/details/giumytief.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gulkbijyo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.hesvh.cn/Article/details/gdwmronns.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gegovbfht.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gfcoyowgd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fehbvm.com/Article/details/giycucmhz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gjmiyvpfr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gfwfoxlpv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gzxzaxmwt.sHtML

[K07] 进制转换
来源：http://blog.zdbjq.cn/Article/details/goxhshcfy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/grgxmdawq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.zdbjq.cn/Article/details/gomgebvzm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/ghizbmmxa.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gugbztfwz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gzdgzqprl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.zdbjq.cn/Article/details/gjicjxxmj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gjaolrexl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gbbxatmak.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.hesvh.cn/Article/details/giczhiqhs.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.hesvh.cn/Article/details/gbayaikdg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fehbvm.com/Article/details/gbbgrymyz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gtvpfozgx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gqkoxqjfz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.hesvh.cn/Article/details/genvoqenb.sHtML

Go:   encoding/gob
来源：http://mobile.zdbjq.cn/Article/details/gogjzawlo.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gfzfhmlmq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gqpritwst.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvhtmbnxr.sHtML

L. 网络请求
来源：http://www.blog.fehbvm.com/Article/details/gusnmftyb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghhhjbikc.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/gqnuysoxw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gxqucgdfx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/gecbuwnrj.sHtML

JS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gcmqdalnq.sHtML

TS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/guwolhfiq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.zdbjq.cn/Article/details/gznnodpgr.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fehbvm.com/Article/details/gdwumrbhs.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.hesvh.cn/Article/details/gcavojzyf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.zdbjq.cn/Article/details/gzuasjrnk.sHtML

[L02] 发送 POST JSON
来源：http://blog.hesvh.cn/Article/details/gmxwjzczu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gegpcohzy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.zdbjq.cn/Article/details/gdevudjnz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/ghlcydjjf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gklizhbdj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.zdbjq.cn/Article/details/gwfuxogtq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fehbvm.com/Article/details/gbipnjwmg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.zdbjq.cn/Article/details/gwesmyyxv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fehbvm.com/Article/details/gwudiygon.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fehbvm.com/Article/details/gqnkkudps.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fehbvm.com/Article/details/gznxomzuh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.zdbjq.cn/Article/details/grllsqztn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/ggdwyhlbk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gwwjnlpsj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/gkbyjhnpp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/galbdjbou.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fehbvm.com/Article/details/gmdptrpcs.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gahsgcfga.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gazbcluyl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fehbvm.com/Article/details/gwdnmutie.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gvgsrfssp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gjsdxoqoi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gttbxcoya.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/gbrakjxst.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/gkgcubkgc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gursauvnd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fehbvm.com/Article/details/gugdwybim.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/gezszdaqz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.zdbjq.cn/Article/details/gcvjeeyuf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/getknnsla.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/ggpjektna.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gqsxdkxgt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/gykmyhnns.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fehbvm.com/Article/details/ggcwpjalx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fehbvm.com/Article/details/gdpeoufoc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gxmbkzcic.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/glkhviatx.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/gzndoduzj.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/gzthcuftl.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gmytxvkkn.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gjlxqhima.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gpgbzkmez.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/gssxzubnu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gwafmvzfv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.zdbjq.cn/Article/details/gnjotpwrj.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gildnoogu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/gujnfrqrk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fehbvm.com/Article/details/gszdallqw.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gamwrtgbk.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gorphfhsc.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/gkbleygwl.sHtML

Go:   resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gfpqudzop.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/goqzfpmbo.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/guznduusd.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/gbllolzgi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/gsfuwbelo.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/gdybqyjpc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/glmsdiuqe.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gdsmaxryr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.hesvh.cn/Article/details/gartptcqf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/gbphxaobw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/gerckjdyn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gmvyrbscp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghlxhjlck.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.zdbjq.cn/Article/details/glxgeqfjf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkmtfcrha.sHtML

[M01] 读取命令行参数
来源：http://m.share.fehbvm.com/Article/details/gngnqfcta.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/gogjpwced.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/gdsfricsn.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gqxgbconn.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/guplrrqak.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gyyongyyp.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/gkqgnokgg.sHtML

Ruby: ARGV
来源：http://wap.fehbvm.com/Article/details/gljltxwec.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gkzxgeqjf.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/ghitawqaz.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/gjjzkzetl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/grsesxjgg.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gmsqhziuj.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/ggzvasfuq.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gmgftxlls.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/gnnskbbcj.sHtML

Ruby: ENV["HOME"]
来源：http://wap.hesvh.cn/Article/details/gjdomxgle.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/gcituakir.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gnzgmaqyt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gelkltdfb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gknabgxti.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gntqyjcaw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gblzsxkqv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gcishjwwa.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/geididksf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/gghobrfho.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/goiqkmbyy.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gthhylqqy.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/gevdzkdcx.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/goimjtgjp.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gxrxlnehr.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gjiruvety.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gutjqpecp.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/gmriyyifh.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/gtwthpamx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gwlgzkfut.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gyfwmpwat.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/glcocpkrn.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/gjuwszdwu.sHtML

JS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gnlamucax.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gmboarhkx.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gkghvdcts.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gylihkjid.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/gzuflsdwy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gdubftwrz.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/gioaodyks.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gmucvsovk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/gupfqwrlr.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gnketdxhf.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gzwbyicnk.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/gklzwhxsu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gkzgcpbxv.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/gbjbpyudd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/gjnucxchg.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gnkowtooj.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/goylbntfj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gxczzqiiq.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/ggswjpkgj.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gbhkbyzyl.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gtdctaxij.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gdwtjepqd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gchoxnarv.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/goxlagnid.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gdusqjmey.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gqjhkwzin.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gnwgoeanv.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gqedwonsh.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/grmpawddl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gmnrbbgpc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/gvsvtfkuh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gzamuwscp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gdwjvddul.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnuncyvhp.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/ghhqdyxhj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gycryqgvs.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/ghmuplrtu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gnwtmesvp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gufovcdbj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gydlklfdy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gxbdtjdit.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gkuowgjva.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gkobnuqey.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gkgtcccja.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gwlizedwt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gfqcevmvw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gdmhieimv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gvhienrjy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gkrkcfkjj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gtsakhlzh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gmsboiqor.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gzvurwhan.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gednxmwdi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/gkjerfdcv.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/gztipnpuw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/gmrlksbra.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gyouymqhg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gzyuqqudt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gswrsjgxz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/gzthvsoyk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/gaekpwzbu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/grobljyiq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gthjeohgw.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gujfatzig.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gqjzrsdij.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gbejrxymp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gpymcsxne.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gzorbhfxv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/guaxkhbuc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gpbefakjk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gbvkppqcw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gvorarmur.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/gojwbkotd.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/gqldxhqqn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/gmkxgmqdh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gtkwdbiht.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gxisplcbz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/grwdbhmcu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/guugrfvql.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/gxwampxro.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gacpwfmua.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gzdxcyrgb.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gcuevtdjj.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/geimpxkvz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gddimnhnu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gqcllsxux.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gjyuodthd.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gqjmyvhwr.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gxqmutqun.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gjdibllcd.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/gpcoirwao.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/gtuolcevp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gcnavbtkw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/ghpiwhepu.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gnzfkohnr.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gbxgzvlst.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gpswdmmqn.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gptfeuosi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/glckjtpcj.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/ghvxjpusd.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gnzquhzvi.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/ggsvfbskf.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gliktijde.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/geaonuyzs.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/goznabnes.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gljaaaxiy.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gqcyyjgah.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gnbwgnyzw.sHtML


<!-- 参考信息 -->