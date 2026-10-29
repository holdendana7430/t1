代发 wailian999

================================================================================
来源：http://baike.fehbvm.com/Article/details/gemdvkyou.sHtML

K. JSON 与序列化
来源：http://www.share.hesvh.cn/Article/details/gbhyjpbjk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggopryekk.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fehbvm.com/Article/details/ghsikfugg.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/gauqoccrq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gtdvkbwvd.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gtezzuyrp.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/ggssspvll.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.hesvh.cn/Article/details/ghpjhteao.sHtML

Go:   json.Marshal(obj)
来源：http://3g.fehbvm.com/Article/details/gpvdhqrwj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fehbvm.com/Article/details/gyflyiwlm.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.hesvh.cn/Article/details/gyzopniaq.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.hesvh.cn/Article/details/gqmyowaez.sHtML

Py:   json.loads(s)
来源：http://www.share.fehbvm.com/Article/details/govbunwnj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fehbvm.com/Article/details/gptlwyhru.sHtML

JS:   JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gwzzzqmhc.sHtML

TS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gzucbhpks.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.fehbvm.com/Article/details/gqxxwbwzu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gotfsushp.sHtML

Ruby: JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gjlwbmtzu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.hesvh.cn/Article/details/guklsxkmq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.fehbvm.com/Article/details/gsrmpmbgg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gzsfyqizw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/gldvjoxkj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gfkhhtiht.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/guvqwtwbb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.zdbjq.cn/Article/details/gjapfpohe.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.fehbvm.com/Article/details/gjvvameor.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.hesvh.cn/Article/details/gjiyjbpgc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.hesvh.cn/Article/details/gvgofighx.sHtML

[K04] 读取 JSON 文件
来源：http://3g.zdbjq.cn/Article/details/gsplbfbdc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.zdbjq.cn/Article/details/ghofjdehu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.fehbvm.com/Article/details/gvjbaaiej.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/gmvubifxq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/gchwvllyo.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gmwdvgkin.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/gsgqtpofa.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gncfrrmul.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.fehbvm.com/Article/details/gymkohiqy.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/gnexaaygd.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fehbvm.com/Article/details/gukxsjjhh.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fehbvm.com/Article/details/gwumgdkcs.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gcucvcvfq.sHtML

TS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/groibokps.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fehbvm.com/Article/details/ggoqhmuau.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.hesvh.cn/Article/details/gzpekrqes.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fehbvm.com/Article/details/gyniuuyqw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.fehbvm.com/Article/details/ggijxzwmi.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fehbvm.com/Article/details/ghntzzadz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.hesvh.cn/Article/details/gkkxtitev.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fehbvm.com/Article/details/gulaksxom.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gkqtvnhzb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/gmglnnpag.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fehbvm.com/Article/details/gewajwhew.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gsnjcgvrk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gpyyqdsqc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gtmjzeaiq.sHtML

[K07] 进制转换
来源：http://read.share.hesvh.cn/Article/details/gmvcdkrfu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/ghqlaklsi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.zdbjq.cn/Article/details/gdvbnnudl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gdxbjfsqp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gynogxmlz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gatvyplkj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.hesvh.cn/Article/details/gphvocoor.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.zdbjq.cn/Article/details/gckrnnoxk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gqvnipogg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/gqsqvozts.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.hesvh.cn/Article/details/gawmdzghf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.hesvh.cn/Article/details/gslwatscq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gmezhihiv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/gzhecafcn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.fehbvm.com/Article/details/gosizvuyx.sHtML

Go:   encoding/gob
来源：http://read.share.fehbvm.com/Article/details/gpyopktvm.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fehbvm.com/Article/details/gmoileadz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gufbpvthn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkqnnykic.sHtML

L. 网络请求
来源：http://mobile.zdbjq.cn/Article/details/gstgdehox.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gclwaujlz.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/gukselcew.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fehbvm.com/Article/details/ghvfcwvcv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fehbvm.com/Article/details/gkzammcpe.sHtML

JS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gwbhwxkjf.sHtML

TS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gebjgrypi.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.zdbjq.cn/Article/details/gddlinvjq.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/gydijqeda.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fehbvm.com/Article/details/gbnciogca.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fehbvm.com/Article/details/gvtjjhfcm.sHtML

[L02] 发送 POST JSON
来源：http://blog.hesvh.cn/Article/details/gojvgziug.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gkoaqugqb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fehbvm.com/Article/details/gckyfwweo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gtwwvleqb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gvwvefidh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fehbvm.com/Article/details/gvjunwpch.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.hesvh.cn/Article/details/ghpovgxre.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.zdbjq.cn/Article/details/ghcujraor.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.hesvh.cn/Article/details/gplwekjxj.sHtML

[L03] 设置自定义请求头
来源：http://blog.fehbvm.com/Article/details/gryeonwvs.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/geuvvsvkj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/gchtfiztx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gjpuzxwpm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gbenfzolr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/gsfakkcgk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gfoymavlq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/guwyauggy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gcshxqthr.sHtML

[L04] 设置超时
来源：http://mobile.hesvh.cn/Article/details/gpuzmhjmq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gsfrrrqtz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/ggfefthrv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gmbqzgxsq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/giceanyxk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gaqmkzrsl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/gyawjmrvy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.hesvh.cn/Article/details/gktyuwtri.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/gwxptvvbq.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gdysskdjl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/gjsytmxxk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/gqebuzqeg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gctzwlzpb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gkhcnjotu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/gssrcavqc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.zdbjq.cn/Article/details/gnzwssxtg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.zdbjq.cn/Article/details/gtvbrcuxo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gxtderhqm.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.zdbjq.cn/Article/details/gasagcise.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/gbrgdbfjh.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gytfxeiud.sHtML

JS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gufdysqdr.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gqxtomigf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gxkettbob.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.hesvh.cn/Article/details/gbfqbekqa.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.hesvh.cn/Article/details/ghbkkzqqa.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fehbvm.com/Article/details/ghaljsiox.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gwzqkzcxo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.hesvh.cn/Article/details/gfqwpsaao.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/gktexsezp.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gwdxgsrrr.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/ghlknehdi.sHtML

Java: resp.statusCode()
来源：http://m.share.fehbvm.com/Article/details/gjmqsdxgl.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gnzabfezz.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/gxjmtdktv.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gxigfjjyc.sHtML

[L08] 并发请求多个地址
来源：http://blog.hesvh.cn/Article/details/gvzfvhznk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/gtjkstjgd.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.zdbjq.cn/Article/details/gtilogyvr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gqutjlvpx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gxpwixnby.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.zdbjq.cn/Article/details/gqxjlsosu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gbuzeamra.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.hesvh.cn/Article/details/gzuldyjhl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/gzfimznhx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gefadeoxl.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gqvbaxwkq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcdrohcnu.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gvnjogmik.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gghgyzemr.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/gkmhwugwr.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gfxejwujq.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/ggrapwsca.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gufepxrqm.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/gupqohrii.sHtML

Ruby: ARGV
来源：http://www.share.hesvh.cn/Article/details/gtkmpltgv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gudstcauz.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gnilfvinv.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gdhrmvwxg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gsppntecy.sHtML

JS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gxkvepoao.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gmgtgqgkh.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gdmwllosv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/gbynfzxeq.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gpvjsfjuq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gggnixxzq.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gbduxuykp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gdyejdezu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/glaaxxjkc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gkpmhxpfa.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/grulipqdh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/gjayszwfl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/ggzptqzmy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gvoprrlnp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.hesvh.cn/Article/details/gfpyskqvh.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gmnjqexyk.sHtML

Py:   os.getcwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gckxkhoow.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/gmvfwaxio.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gfzpyqapb.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gscrccitm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/ghxshysjq.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/gwwykeebf.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gpevhyuzd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gjwraihwi.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/gtnngeerb.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gwqdhphaw.sHtML

PHP:  exit(1);
来源：http://www.blog.fehbvm.com/Article/details/gpmbvtmlg.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gkcwfwoiz.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/guiuqawtl.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/gqorqqwic.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gnnbppajw.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/guxeicjfl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/grflsbfuf.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gmkfunqyu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gotzxtnrp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gdyalgeoy.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gyotrjjjq.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gskonjszf.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gecxlgshd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gtofbeoqc.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/guyhmhvcg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gfpefiesf.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gpbahmogc.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gtmiwfegt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gppgpodet.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gscipozmy.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gyrfebtpu.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gsotlfydx.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gbxysachy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/glohjckrn.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gxwakrqtr.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gouenakcx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gqikhzcep.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/glgebbfou.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gbvhmnjnq.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gqoazweqj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gjhbhfbka.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/goqueksay.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gszapahpx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gyebxmrqw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwqybsjnv.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/gosruumbp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqtwyhcxr.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gqlvjlgfr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gqimqeftm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gxejxgeqf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/glqtsdqzq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gvijipiha.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gyyhtongu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gdgqbsiqv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/gpqsqqprq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gwhdahdtf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/guxjytxim.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gltpyujgt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gmytyfrfq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gstlbngxg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gepftfjjg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gmfyhvrhk.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gibtgioto.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gtduzrilf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/grevvohyp.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gcqrdqedt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gsasomoou.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gubqnttnh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gcsrxrvze.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/glhmhqggo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gqafzifst.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gyqusotjh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gxrmeshdc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gabxbtvsb.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/gsjfdnmdd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gnnefclao.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gmbhgwhii.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gdzndeynl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gjicryrgz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gzcimbzde.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/gpehvtcko.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/grhsrvuve.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gelpdqkzr.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/ghfrqvbqo.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gdutlcwjb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gwwjuukor.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gwsnbrdak.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gokhttlau.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gymcrinxb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gzyvifvbc.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gtsvornuu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gkuopkcmy.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/gealldcot.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gdpqzlskh.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/grvdkizdz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gjhmtagye.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/glftrxflx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gywmfaovl.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gmqslqhsn.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gixjmmjki.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gbclvrvcu.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gqvxfwfca.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gxuxkykic.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gzciiecvs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/ggdfknnsn.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/ghpxvsfgx.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gpqdawrdh.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/goicixhub.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gemuuxpdr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gmocfuyzx.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/gmwczbsfk.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gbpbkoivy.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gzmuibbnm.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/grgbnyasu.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gyrqacecg.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/giysnpask.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gjsbxhdkh.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gfjkmklrm.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gfwqkluwg.sHtML


<!-- 参考信息 -->