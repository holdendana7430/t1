代发 wailian999

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gddhkkkzd.sHtML

K. JSON 与序列化
来源：http://blog.zdbjq.cn/Article/details/gnbfnchjr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gctvqncfm.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.fehbvm.com/Article/details/gknxrakil.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/gxqbluuab.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/gdmpyzwnx.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/grhlnfxtz.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gwuosxgzn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.hesvh.cn/Article/details/gfbthazai.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.fehbvm.com/Article/details/gycxibvog.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.hesvh.cn/Article/details/gpjgkuspo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.zdbjq.cn/Article/details/gtpfvwfag.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.hesvh.cn/Article/details/gntnzyivv.sHtML

Py:   json.loads(s)
来源：http://blog.zdbjq.cn/Article/details/gtbtrpuma.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.zdbjq.cn/Article/details/gkmmcbzjp.sHtML

JS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/ggfmpmonf.sHtML

TS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gummcjivj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gsjacnkmk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gduvvnduz.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/grzdeihsi.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fehbvm.com/Article/details/gkvqjxvby.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.hesvh.cn/Article/details/gcjabfeuf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/gubljjycl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gkmpizqqb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gaqhooczb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fehbvm.com/Article/details/gdslpmhay.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.zdbjq.cn/Article/details/gfzurmcvc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.hesvh.cn/Article/details/gtzxqmktc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.hesvh.cn/Article/details/gmyjrhndk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.zdbjq.cn/Article/details/gxhfldynn.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.hesvh.cn/Article/details/gyuuzwqpt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.zdbjq.cn/Article/details/gxmjnujkb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fehbvm.com/Article/details/gfhbqwlaq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gnevccstj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/gejitzika.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gerxxrglr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/ghsmlcvfq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gcyuaqxve.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.fehbvm.com/Article/details/ghxescijn.sHtML

[K05] 深拷贝对象
来源：http://baike.zdbjq.cn/Article/details/ghufspgpr.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fehbvm.com/Article/details/grylkahiv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.zdbjq.cn/Article/details/gybtliysq.sHtML

JS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gnbnihfgz.sHtML

TS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gfhvevnhi.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.zdbjq.cn/Article/details/gugsqqpqn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.zdbjq.cn/Article/details/gnaljmpcv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.zdbjq.cn/Article/details/ggyhttduv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.fehbvm.com/Article/details/gutcckzbn.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fehbvm.com/Article/details/gfddfrnrz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fehbvm.com/Article/details/gairwngaf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fehbvm.com/Article/details/gtwjitqrk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gzpofkakb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gdsmmpfpg.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/ggftwukrl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/ganojfsxb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gtapxcrmw.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/giwlhvfep.sHtML

[K07] 进制转换
来源：http://baike.fehbvm.com/Article/details/gpsrdphgb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gxbatvlhs.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.hesvh.cn/Article/details/gypggjhgf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/ggxoezvwy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/guzuwpjvv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/ggyutwkua.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.hesvh.cn/Article/details/gmoqbptvk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.hesvh.cn/Article/details/gcpuerwiu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gndcvlpnf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.zdbjq.cn/Article/details/guvtnwuox.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.zdbjq.cn/Article/details/gyudvguba.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.zdbjq.cn/Article/details/gggkkrtlc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gsxiysjid.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/giiffqiim.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.hesvh.cn/Article/details/glktmthhk.sHtML

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/gfavqhven.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.hesvh.cn/Article/details/gxvrouoxq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gjsamhzsj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/guflzefhh.sHtML

L. 网络请求
来源：http://3g.hesvh.cn/Article/details/gbypgkzsq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvovrobpf.sHtML

[L01] 发送 GET 请求
来源：http://baike.hesvh.cn/Article/details/gnypaztix.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.zdbjq.cn/Article/details/ghtzszlmo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/gcfiysuyd.sHtML

JS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gjdlhctee.sHtML

TS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/ghnbyqazy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.zdbjq.cn/Article/details/gzdgevozs.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.hesvh.cn/Article/details/gcpwrvkys.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/gqjgmojgb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fehbvm.com/Article/details/gpcmxzluf.sHtML

[L02] 发送 POST JSON
来源：http://read.share.hesvh.cn/Article/details/glcifoypg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gkstzwzxa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.hesvh.cn/Article/details/gmhsfsnvr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gzzfyoaql.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gwytghkek.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.hesvh.cn/Article/details/gixgymohh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/gruxoscql.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/geblwyotl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.hesvh.cn/Article/details/glgpwhryq.sHtML

[L03] 设置自定义请求头
来源：http://read.share.zdbjq.cn/Article/details/gahczgwhp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.hesvh.cn/Article/details/gmcidqdbo.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.zdbjq.cn/Article/details/gxsyiijyh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gkwfkbfrq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gnpdxktxt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/gqdtxxbnq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/grpghdopp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.hesvh.cn/Article/details/gbveygtjt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/geyqoywdd.sHtML

[L04] 设置超时
来源：http://www.blog.fehbvm.com/Article/details/glcceemqi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.hesvh.cn/Article/details/gxebnwvoo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.zdbjq.cn/Article/details/gnwdkybpi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gdfnnmcvj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gxbkgeksm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fehbvm.com/Article/details/gvwpgwojc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.hesvh.cn/Article/details/ghayhnzsd.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.hesvh.cn/Article/details/glgipbqry.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gsdfdueoa.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/gpllfprxh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fehbvm.com/Article/details/gtufrffyg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.hesvh.cn/Article/details/giuydafwr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gharsqmur.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gmddefxto.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/grtkwjpzt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fehbvm.com/Article/details/grogbeoxw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/gtzhsgyog.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gcwbunwok.sHtML

[L06] 解析响应为 JSON
来源：http://baike.hesvh.cn/Article/details/gjehvibqe.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/gzxygubam.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gnajpcgtp.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gazjtanod.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/ghjzxpttd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gzcwekbcn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.zdbjq.cn/Article/details/gnzamfvjf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/goppqvriw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fehbvm.com/Article/details/gjwyluoih.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gmcruilyg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/gltlwflrb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.hesvh.cn/Article/details/gyujwpxua.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gfyawmqgl.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gkjvmqumn.sHtML

Java: resp.statusCode()
来源：http://www.blog.zdbjq.cn/Article/details/gyolrtgkz.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gmgzhhyqk.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gmppkkqds.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/giizbrmhe.sHtML

[L08] 并发请求多个地址
来源：http://blog.hesvh.cn/Article/details/groudiwfl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fehbvm.com/Article/details/grbvimczy.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/gvcahdkxj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/goncvcnoq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gqbjeexcp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gsvxmcmjf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/gwtikpfrg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/gqydwyvzu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/ggfoyfojt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggtxrpbqx.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/ghmzzwbnu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghpaddgwi.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gggdgkhni.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/gdoejqpdg.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/gpnkzgypt.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gcasxtgkl.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/grusuqelp.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gnbyglpvp.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gmaoqrgei.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/grabydfnv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gbfebhpci.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gfylrhlag.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/guvhyerwj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gwxjaalub.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gnwwulpys.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gigvjrnwu.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gmqovjywz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/gsjoutuvf.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gykwgdjyw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gwapplehw.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gphepxwit.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/gkgziirbd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/gyqzkjtko.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gecxpdwgy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/geqerwulf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gleuzenvc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/gbcahhcxl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gfckhpiei.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/gbkklpuzr.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gnxlpqgkw.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/goklsskod.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/gjidzxvyp.sHtML

JS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gfnrguiyo.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/glwjiufim.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/ghpimqhob.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/gambgqqzn.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/gtgejnljx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gxhlcfckb.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gypxpvvwq.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gocujilqo.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/goqimnwmx.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gumdmyglu.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gdofhbken.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/gipbylgsp.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/grtkvnruj.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gjgvswckj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/guhgjvnsz.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/guxzueril.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gacvfthrc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/gpjiykybn.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gpfxssuoy.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gxcasawyk.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gihbrwqfk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/ghvooyzlw.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gtkhqacov.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gqbzodltb.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gffbkatan.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gwhdnqqmx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/gqjiwmaim.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gdhmpjait.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gewqsqefy.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gvphxjryt.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gcdojposp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gxzqdtrtx.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gdsxzigee.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gyfdzatrh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/giynetpwt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/gfwmiausn.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gviphwlkp.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gemgyzznw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gzbjbfbsc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gfpoyynib.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/ggkwcuoym.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/golsotkih.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzzczvmvf.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gnjuxxscq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvkagvjun.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gkobosrbj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fehbvm.com/Article/details/gjnddcmta.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/gqshecobm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gurwfftfz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gwtbclgfg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gcxibrgvy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/gkfbbqndx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gldasoxee.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gtaeuxhkf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/guqqgtpnj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gddkokyas.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/gjqulroae.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gprgrvcms.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gsbwftnpd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gifxjbrdf.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gownsireq.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gsaxkmuug.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/gqmjwlcku.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/gqehamded.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gkglhnzac.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/ghhgfacsy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/grziktsiz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gnrssvsbf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gzhjhbjrm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gxgphiqia.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/gecdznywo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/gtfspihrv.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/gtqvmnpbe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gdablokrh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gfxcnpsya.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/geajstarn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/grsokullz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gbitolaux.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gldumplrs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/ggyntsjjt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gsilnuvfz.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gezfjbpdm.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gulgsrpjo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gzrvilurb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/glivvglwh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gooaykcfa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gfgxezbfr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gmmklwurc.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/genmdkorq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/gdnzvkpyt.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gddudiyud.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gjokmdaze.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gjdestlod.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gxczoolwu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gsnsyrlso.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/glsrbbhsx.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/ghyiiyrlz.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gvjsgfxip.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/grditnizu.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gtlsqgldd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/gmuyswojq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gcprlnlbz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gfaiwesie.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/ggppivxok.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/ghbbfinat.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gmunfmkrv.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gaojaevdd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gxyenknkz.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gelzlymtn.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/ggdgrzeor.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/gyiuubuca.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gypgquckb.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gruchuhku.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gsiaysrpy.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/ghyrwcgve.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gzcxvfbhk.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gategjznh.sHtML


<!-- 参考信息 -->