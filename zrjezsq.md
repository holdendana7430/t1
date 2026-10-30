代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fanxiaobao.xyz/Article/details/gomqqbvaw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.fanxiaobao.xyz/Article/details/ghgxkfgou.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/ggymnplal.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/geeuksloh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.fanxiaobao.xyz/Article/details/guqvsebvz.sHtML

Go:   json.Marshal(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gbcseowtz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.fanxiaobao.xyz/Article/details/gvbxobowr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gljkfawks.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fanxiaobao.xyz/Article/details/guxifjart.sHtML

Py:   json.loads(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gzvngrugl.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsbxvdek.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpbjkssf.sHtML

TS:   JSON.parse(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwfiiucj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvzqhbjn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxpoirjv.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gioccnbnp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gggeuhync.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grudtxrgd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuqrrwgj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fanxiaobao.xyz/Article/details/gbbyxqwrw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gfxowsqrt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gruklofpy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gnrtcjmlw.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fanxiaobao.xyz/Article/details/gvhmtjzyw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/glfyjpzbn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsreplnnt.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqnnnrew.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtkscfqr.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmelmhvhn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugsskezu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fanxiaobao.xyz/Article/details/gasjzqnhj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fanxiaobao.xyz/Article/details/gacaxwaba.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fanxiaobao.xyz/Article/details/gseknymve.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gczxkhlnc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmrumaji.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjyyvweu.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsctdpabz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fanxiaobao.xyz/Article/details/gkvkmciuk.sHtML

JS:   structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfakmqfc.sHtML

TS:   structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gawoyhedt.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmlgmwde.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.fanxiaobao.xyz/Article/details/gdwohwluw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmqmbgew.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrcuqgye.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fanxiaobao.xyz/Article/details/getzeusmc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fanxiaobao.xyz/Article/details/gftamiqff.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gstczvgtv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fanxiaobao.xyz/Article/details/gozokoezx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fanxiaobao.xyz/Article/details/gzxjxatel.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzssztfd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fanxiaobao.xyz/Article/details/gwhxtboqs.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsskfuxe.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpgfcbrw.sHtML

[K07] 进制转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gzytbtjqs.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/goahnooxx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fanxiaobao.xyz/Article/details/groaziilc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gyqliuxmx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gnwscphyw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/glsjjhzkw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkaitlddj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fanxiaobao.xyz/Article/details/gayzlqapx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtshtohtd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fanxiaobao.xyz/Article/details/gllmrlkgw.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gembnrcbg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrjownfc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fanxiaobao.xyz/Article/details/gvykhiuvk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fanxiaobao.xyz/Article/details/givwgsgav.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fanxiaobao.xyz/Article/details/gbvfnrjjd.sHtML

Go:   encoding/gob
来源：http://baike.fanxiaobao.xyz/Article/details/gljppnyqq.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gsrwsmkrm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsbrgfhv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/guqgfrjme.sHtML

L. 网络请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gasrcpqwv.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/goiratflg.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknxnppbh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fanxiaobao.xyz/Article/details/gvsitcodn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fanxiaobao.xyz/Article/details/ghvattikw.sHtML

JS:   await fetch(url)
来源：http://wap.fanxiaobao.xyz/Article/details/glpniorpk.sHtML

TS:   await fetch(url)
来源：http://read.share.fanxiaobao.xyz/Article/details/glhvqjmsd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fanxiaobao.xyz/Article/details/ginnowsaj.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpofpnoj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fanxiaobao.xyz/Article/details/grigzened.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fanxiaobao.xyz/Article/details/gdlccjtlp.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqgfwlhq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fanxiaobao.xyz/Article/details/gshclzydd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwvttspr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fanxiaobao.xyz/Article/details/guznsspak.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fanxiaobao.xyz/Article/details/gbhedjegw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fanxiaobao.xyz/Article/details/glpogohhn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fanxiaobao.xyz/Article/details/gudfjhvvg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmguavgws.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fanxiaobao.xyz/Article/details/guhdkertn.sHtML

[L03] 设置自定义请求头
来源：http://blog.fanxiaobao.xyz/Article/details/gycgzxpuu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fanxiaobao.xyz/Article/details/gqgjslvxa.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgzqyqsr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsneflyh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fanxiaobao.xyz/Article/details/gonyxhtou.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzocormv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqspxfri.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fanxiaobao.xyz/Article/details/gjbdspbrm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbndfopp.sHtML

[L04] 设置超时
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwcrrelm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fanxiaobao.xyz/Article/details/gjqeoodxh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbntjqbh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmrgfomk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gvujgldyv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fanxiaobao.xyz/Article/details/gakhvktsj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fanxiaobao.xyz/Article/details/gdwmyqqip.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngmdbhio.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzagxvsx.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fanxiaobao.xyz/Article/details/gzicrhhrm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fanxiaobao.xyz/Article/details/gprufnimi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfnvsokc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fanxiaobao.xyz/Article/details/ganuvrknq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fanxiaobao.xyz/Article/details/gxomrlbxw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fanxiaobao.xyz/Article/details/gajzlmven.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fanxiaobao.xyz/Article/details/gelwrzfwi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvbgjugx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnmyfxie.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getmsdrsh.sHtML

Py:   resp.json()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrizopbu.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gbyectkdo.sHtML

JS:   await resp.json()
来源：http://baike.fanxiaobao.xyz/Article/details/grocirqox.sHtML

TS:   await resp.json()
来源：http://wap.fanxiaobao.xyz/Article/details/gostqdpbu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvqxxieg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdnyywdr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfqbmuiq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fanxiaobao.xyz/Article/details/glifrcgdi.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwackxgh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fanxiaobao.xyz/Article/details/gcxxhydkz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fanxiaobao.xyz/Article/details/gmjispfbl.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fanxiaobao.xyz/Article/details/gudhoqsdf.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fanxiaobao.xyz/Article/details/ghoqdvmif.sHtML

Java: resp.statusCode()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqknpcrpt.sHtML

Go:   resp.StatusCode
来源：http://3g.fanxiaobao.xyz/Article/details/gcrfnbllj.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fanxiaobao.xyz/Article/details/gzixjlyzc.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwjmbnhj.sHtML

[L08] 并发请求多个地址
来源：http://wap.fanxiaobao.xyz/Article/details/grrbrssfr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhauauxl.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fanxiaobao.xyz/Article/details/gcxldqdhs.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gccipkpru.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gyyjcsiif.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyviabbwr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fanxiaobao.xyz/Article/details/ghklulyan.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzrxaela.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gxtaowmru.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gdodgeyjf.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptwmibdr.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhlvssuc.sHtML

[M01] 读取命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/grvgcqwdk.sHtML

Py:   sys.argv[1:]
来源：http://wap.fanxiaobao.xyz/Article/details/gxojuqqcw.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghravbfbw.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwknfjbji.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnofostt.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fanxiaobao.xyz/Article/details/gooxymoeb.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdwgptok.sHtML

Ruby: ARGV
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgaxcaxm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhcelgxl.sHtML

[M02] 读取环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsdaatfj.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoueudit.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fanxiaobao.xyz/Article/details/gqrbahhel.sHtML

JS:   process.env.HOME
来源：http://mobile.fanxiaobao.xyz/Article/details/gikeywjji.sHtML

TS:   process.env.HOME
来源：http://blog.fanxiaobao.xyz/Article/details/gaqvyplgv.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvjphtrk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fanxiaobao.xyz/Article/details/gssfxyjgd.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fanxiaobao.xyz/Article/details/gtyemxufh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fanxiaobao.xyz/Article/details/gisgtdadh.sHtML

[M03] 执行外部命令
来源：http://3g.fanxiaobao.xyz/Article/details/grzxytgzq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggxspmnb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fanxiaobao.xyz/Article/details/giplnoztt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqbeefox.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fanxiaobao.xyz/Article/details/gxytnsoyn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmafvmpop.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzajgncnl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyksclha.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdbfnfqv.sHtML

[M04] 获取当前工作目录
来源：http://blog.fanxiaobao.xyz/Article/details/goejxncvn.sHtML

Py:   os.getcwd()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjqroibp.sHtML

PHP:  getcwd();
来源：http://baike.fanxiaobao.xyz/Article/details/gbysonwgf.sHtML

JS:   process.cwd()
来源：http://read.share.fanxiaobao.xyz/Article/details/grgvvlesn.sHtML

TS:   process.cwd()
来源：http://baike.fanxiaobao.xyz/Article/details/guiaucyzs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girwluspa.sHtML

Go:   os.Getwd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvrjcgop.sHtML

Ruby: Dir.pwd
来源：http://3g.fanxiaobao.xyz/Article/details/gietatzof.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fanxiaobao.xyz/Article/details/gichxrfon.sHtML

[M05] 设置退出码
来源：http://wap.fanxiaobao.xyz/Article/details/gmdocxwwi.sHtML

Py:   sys.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gtusatmps.sHtML

PHP:  exit(1);
来源：http://3g.fanxiaobao.xyz/Article/details/gnrdyfhxj.sHtML

JS:   process.exit(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gakbaqspv.sHtML

TS:   process.exit(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gecnbifhu.sHtML

Java: System.exit(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gacjeprff.sHtML

Go:   os.Exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjhtoygi.sHtML

Ruby: exit 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gritabbei.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcegtwbl.sHtML

[M06] 向标准错误输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gckxxvehq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gftgojlgx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtamiczvp.sHtML

JS:   console.error("err")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbniriqls.sHtML

TS:   console.error("err")
来源：http://blog.fanxiaobao.xyz/Article/details/gzqelxeuk.sHtML

Java: System.err.println("err")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzhpsdrd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fanxiaobao.xyz/Article/details/gooufeuww.sHtML

Ruby: warn "err"
来源：http://blog.fanxiaobao.xyz/Article/details/grpbuzand.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdrskqzn.sHtML

[M07] 判断是否为主入口
来源：http://blog.fanxiaobao.xyz/Article/details/gpawssiej.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdbpjxfz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fanxiaobao.xyz/Article/details/getdhyjbl.sHtML

JS:   require.main === module
来源：http://blog.fanxiaobao.xyz/Article/details/gfapckuwa.sHtML

TS:   require.main === module
来源：http://wap.fanxiaobao.xyz/Article/details/gtqiapoac.sHtML

Java: public static void main(String[] args)
来源：http://wap.fanxiaobao.xyz/Article/details/gpauzobrv.sHtML

Go:   func main()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqdbwknp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fanxiaobao.xyz/Article/details/gsgltsovu.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fanxiaobao.xyz/Article/details/gkyiudihu.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fanxiaobao.xyz/Article/details/grnhlvwvt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnljxvteq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnufoxti.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcuhbcyc.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzxtuzqv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfvwxwuv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fanxiaobao.xyz/Article/details/gknvbksbx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fanxiaobao.xyz/Article/details/gddmwmdhw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqiiqymc.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/grxrijvjk.sHtML

N. 数据结构与算法
来源：http://wap.fanxiaobao.xyz/Article/details/gornbsxoz.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ganowdong.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsfaubyx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gumbxfocf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fanxiaobao.xyz/Article/details/gzkkmcpjs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukidqvfo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzjvmapd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goplkorry.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gdbttlhtg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajumlpcr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyeklwgq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fanxiaobao.xyz/Article/details/gvpnlbfyn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fanxiaobao.xyz/Article/details/gmturplar.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhyhtvkz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwikcumxm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggghwcbom.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpnqjhrv.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlqxaveq.sHtML

Ruby: arr.sort
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgqzpsji.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfiijvznp.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fanxiaobao.xyz/Article/details/gwqxnowtt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fanxiaobao.xyz/Article/details/guqoyzkob.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogknxhlx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fanxiaobao.xyz/Article/details/ggjkelqyo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtspydgg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fanxiaobao.xyz/Article/details/gpmkrcuxo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fanxiaobao.xyz/Article/details/gfghahatl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fanxiaobao.xyz/Article/details/gdygdqkms.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwzxtmhc.sHtML

[N04] 斐波那契数列
来源：http://blog.fanxiaobao.xyz/Article/details/gydpbehhh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsajquty.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunkjyulr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxfoxbbh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gxpgxrovs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fanxiaobao.xyz/Article/details/gqcejglss.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatnozpls.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxotierzc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gmckroxdu.sHtML

[N05] 最大公约数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqypjhexk.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fanxiaobao.xyz/Article/details/geubzxvng.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fanxiaobao.xyz/Article/details/greznufbf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghkfmnnqr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfabsnlxn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnlpsjhm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guujprccg.sHtML

Ruby: a.gcd(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gusxdcuia.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvryeomvt.sHtML

[N06] 判断回文字符串
来源：http://wap.fanxiaobao.xyz/Article/details/ggvrqbofa.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grflyjtoj.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fanxiaobao.xyz/Article/details/gfyrgmgla.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkcztial.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fanxiaobao.xyz/Article/details/ggrvgtowo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fanxiaobao.xyz/Article/details/gxmnqkilq.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fanxiaobao.xyz/Article/details/guklxsrtz.sHtML

Ruby: s == s.reverse
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqjwyhco.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fanxiaobao.xyz/Article/details/ghugfzpyz.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshxhxwsi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fanxiaobao.xyz/Article/details/gdedkqlgw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fanxiaobao.xyz/Article/details/ggivbmigl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fanxiaobao.xyz/Article/details/gztxtedki.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fanxiaobao.xyz/Article/details/geoacduns.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggypaxuby.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fanxiaobao.xyz/Article/details/gsywpzlnn.sHtML

Ruby: // 手写 Hash
来源：http://baike.fanxiaobao.xyz/Article/details/gokycqvmn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fanxiaobao.xyz/Article/details/gegffrfgo.sHtML

[N08] 生成全排列
来源：http://www.share.fanxiaobao.xyz/Article/details/giuozjzgc.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gocdibwys.sHtML

PHP:  // 手写递归交换
来源：http://blog.fanxiaobao.xyz/Article/details/gatmxlccm.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnkwqvcu.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyrkencd.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsaavmbrl.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxwlhknf.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuspgeio.sHtML

C#:   // 手写回溯递归
来源：http://wap.fanxiaobao.xyz/Article/details/gdjehpokf.sHtML

[N09] 栈与队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkewyrbob.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fanxiaobao.xyz/Article/details/gsxqxfcdg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrjegqrd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmlmfpfc.sHtML


<!-- 参考信息 -->