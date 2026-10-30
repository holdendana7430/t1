代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/gcpeprpej.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.zdbjq.cn/Article/details/ghfcqvgij.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/grgfdfmhr.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gtxytzvzk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.zdbjq.cn/Article/details/gvrdtzuaj.sHtML

Go:   json.Marshal(obj)
来源：http://wap.hesvh.cn/Article/details/gkcsgyksx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.fehbvm.com/Article/details/gofmjifhf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.hesvh.cn/Article/details/gxgvefsnq.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.fehbvm.com/Article/details/gcbgjtbpc.sHtML

Py:   json.loads(s)
来源：http://www.m.share.hesvh.cn/Article/details/gwabhleab.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.zdbjq.cn/Article/details/gpsrtolwy.sHtML

JS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/ghlnfiuyg.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gbeabyyoj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gcgmceraw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gakltanzw.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gwnlkwqii.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.zdbjq.cn/Article/details/giyxccgbv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.zdbjq.cn/Article/details/gsvtlncfj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.fehbvm.com/Article/details/gnygteqim.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/gqtpuprjf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/gmtsvfesm.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gifrdrjwu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gfsiiltax.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.fehbvm.com/Article/details/ggcosqxds.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.fehbvm.com/Article/details/grtlnwcsz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.hesvh.cn/Article/details/gsyldzrdh.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.zdbjq.cn/Article/details/gsgmwnkss.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.zdbjq.cn/Article/details/gakyzhnvb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.hesvh.cn/Article/details/gkwmloago.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/ghxcdjwku.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gzfxhcjiu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.hesvh.cn/Article/details/gmxxtzwec.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gsvnsljnw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gsfmzgify.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fehbvm.com/Article/details/gholesuob.sHtML

[K05] 深拷贝对象
来源：http://www.share.zdbjq.cn/Article/details/gbcytjsit.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.hesvh.cn/Article/details/gryioirph.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.hesvh.cn/Article/details/giwqfedeb.sHtML

JS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/ggkylzdsl.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gbxfpljsl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.zdbjq.cn/Article/details/gjysfabfv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fehbvm.com/Article/details/gqflqvuub.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.zdbjq.cn/Article/details/ggxdiirro.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/gjfrekkoc.sHtML

[K06] 解析 URL 查询串
来源：http://baike.zdbjq.cn/Article/details/gifscgamr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gosnnynsg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.hesvh.cn/Article/details/gxlekueet.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gcaahcemc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gzvlgqljo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.zdbjq.cn/Article/details/gpsltynby.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gofmbufqf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gbmkfdgoj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gtsnddges.sHtML

[K07] 进制转换
来源：http://mobile.fehbvm.com/Article/details/grcabqabm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gymzqlqfh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/gwxmifujt.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gwagtlbmg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/guywhqakv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gdzdrgkfn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.hesvh.cn/Article/details/ggcqkcjnu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fehbvm.com/Article/details/gxpuhwnqf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gbyahbleu.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.zdbjq.cn/Article/details/ghwzjkjbd.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.zdbjq.cn/Article/details/gzxomvfse.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.zdbjq.cn/Article/details/gssyiekee.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gaktxykpm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/glxkgpcan.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fehbvm.com/Article/details/gprjxptnd.sHtML

Go:   encoding/gob
来源：http://mobile.hesvh.cn/Article/details/gvyiablma.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.hesvh.cn/Article/details/giwlfgaut.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gxtexvcec.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gktqezwqr.sHtML

L. 网络请求
来源：http://www.blog.fehbvm.com/Article/details/gdsbvxfaz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gachqhlkq.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/gptodfqbu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.hesvh.cn/Article/details/gnahajxjc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/gvuzrlrpu.sHtML

JS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gatliimzn.sHtML

TS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gauafhlit.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.zdbjq.cn/Article/details/gcwlhgjof.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/gckmgdgix.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.zdbjq.cn/Article/details/gmxvszmmx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fehbvm.com/Article/details/grkngwuzz.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/ghvhwkrbp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gmbxxjhsh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.zdbjq.cn/Article/details/gvbmzjnit.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/grtryqnnr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gaxrtfsag.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gdnbbnric.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/gyrwyhdty.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fehbvm.com/Article/details/guyhfuyjv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/girrpkkha.sHtML

[L03] 设置自定义请求头
来源：http://wap.hesvh.cn/Article/details/gsxrleqlt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fehbvm.com/Article/details/gqlpijkkf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fehbvm.com/Article/details/gszsigawd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gzfpvamjc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gxtleeyry.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.zdbjq.cn/Article/details/gsnmcqtpn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gwmvmpulk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/gagpqhnos.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gvohmdwlt.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/gkbcrlrwd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gipzufjey.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/gocrriquo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gtuzgdbse.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/glaharxut.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/gidjgmcet.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fehbvm.com/Article/details/gwdzjfgca.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/gwgvkbsnq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.zdbjq.cn/Article/details/gfpqgfhgd.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.zdbjq.cn/Article/details/gkaviuekh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/ganeyyltb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/gkarjjjcz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gnzycphui.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gmvlwczfe.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/gemzjcwiv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fehbvm.com/Article/details/gpursjcnd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gzaynxxpt.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.zdbjq.cn/Article/details/ggnydafzn.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/glvvuojqu.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/gzimpytdq.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fehbvm.com/Article/details/grjvvroky.sHtML

JS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/ggwizfqwx.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gnhgnbtbm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/guryrhktd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/gtefujjoi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.hesvh.cn/Article/details/gtdkputsv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/gkzaubrtn.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gzxqaajas.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/gmakdhimp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/gvrhnllof.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gbaicvlcf.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gmzukqpeg.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/gjgmbtqeb.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gugdgmtep.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/gqtrmvkoi.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gsdtwrexp.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/gwjxtgaym.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/gexlrpxnc.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/grixmacrf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/giiyvxzpn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gbguqihbf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/gxncggxqm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.zdbjq.cn/Article/details/gsrycqoss.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/gxihaycvb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.hesvh.cn/Article/details/gvbvnowqw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmdrstbya.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/geehqmcjz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glyyhpoon.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gwvaskfyo.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gkbtydcub.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/glrhrwpik.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gdwiwqxdu.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/ghsiojiqc.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gjrnlnmxc.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/gqugjqioj.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/gntpteuki.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gqcufojna.sHtML

[M02] 读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/glzpfpzpv.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/gcxfidldp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/ggemybgbf.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gezlqkqiv.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gaecatafi.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/goqdbzdbw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gulrhszll.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/gamoxxgky.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gbtzpnrug.sHtML

[M03] 执行外部命令
来源：http://baike.zdbjq.cn/Article/details/gpfpbbeqx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gxdjunenx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gmevwkjdx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gsmnetckp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gvzovkedt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gvfktkjkd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gjbrzhmut.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/gdtygisiz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gdoowdhkn.sHtML

[M04] 获取当前工作目录
来源：http://blog.hesvh.cn/Article/details/gibqxbslg.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/gxbluwjhq.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gspkythap.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/ghqtexyrh.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gyxdavxia.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gzvapsnhd.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/griekvskv.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/gmxswrtid.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/grhkhcqsn.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/ghttnsesa.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gmrnlmxfe.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gusgaqcfs.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gehtxbpoh.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gmspqmgig.sHtML

Java: System.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gbkbccwdf.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gcpwuzxbd.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/ggnsewacv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gkxqjrtyh.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gualsgorz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gnyuabsgp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gysfeaqpf.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gbjhmczqg.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gzthrxpbi.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/ghrqlzqak.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gqnwedjam.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/gtenrzxhy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/ghkoqfius.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/gmqughcca.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/gkasmayjl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/gqbfwkfck.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/ghdakfvmg.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gonjgxrtr.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/gmhrtuckm.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gbcxngnkt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/gmkbmumzt.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/gczexhrmo.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gpeglnbjf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gmuvondvr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/guuihxewp.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/guwixqiex.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gxwwifltp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/gakrsncpt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gbbhlsuzd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fehbvm.com/Article/details/grniahaps.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gesavbuev.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvtclajck.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/graewnjcr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyxwwnguw.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/gorjhhdpx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/gnubipsbh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gxtulxxix.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gldonkvaa.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/girldutes.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/givralrux.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/grxfrxugf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/gquytskjf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gtgybleup.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gbropqfii.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gxyrktixj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gfkdhifzr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gbhnwhjcg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gahvrepxo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/guujffzvm.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gbcfeaygp.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gywwqjmnf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gsqslmbwq.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/ggdarlqdz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/guhqhhfux.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gmjuajtqu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gkdtxgqsy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/glbyaxsuf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gbgqlvaiv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gvkyhjnpo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/ghujoyywu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/gdqrdawhw.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gkybebvcl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gevsaulgu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gvuysbsyt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gfmarohyg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/geasogxrw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/ghajzmjtz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/ggyeqadaq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gxeakswfm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gikpwipux.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gaajiffxe.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gthapphkc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gsnuzkklk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gbmrfpzyv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/grpubdwve.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gjwnzdjcv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gxwexwdra.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gwdujmxji.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gytyamyar.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/gvbldwkzq.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gavrwtsmu.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gmbhfxntj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/ghjzbcsza.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gtgxzbtzn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gwrmyyssb.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/gmpaydato.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gpewkmyzj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gnyjhkfbd.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gtfkybcbq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/ggctsousf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.hesvh.cn/Article/details/gpxvhlzjq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gpiikfywg.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gwohcktoh.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gbatxjeyo.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/glesutjrp.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/gjfvbmqxv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/glyakgzih.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/gimzjzhfj.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gwygxvriu.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gpogtcykn.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gtfrzujyx.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gkndptkdw.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gsjrumrgv.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gpubbfwes.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/givvwdorb.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gxbqdftbl.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/guwwissff.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/gveogcdrs.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/grnizaihz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gtirrxbtc.sHtML


<!-- 参考信息 -->