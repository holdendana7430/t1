代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fanxiaobao.xyz/Article/details/gwtexryof.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fanxiaobao.xyz/Article/details/goznkwlem.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpzunqbg.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmaoqfic.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fanxiaobao.xyz/Article/details/giayealyw.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gneoovlgu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fanxiaobao.xyz/Article/details/gxitwykda.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/ggsvqxtyt.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjdvbonr.sHtML

Py:   json.loads(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gggeepgjb.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fanxiaobao.xyz/Article/details/gbdoxlapk.sHtML

JS:   JSON.parse(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzguvivkl.sHtML

TS:   JSON.parse(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gbdnuykvb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fanxiaobao.xyz/Article/details/gcwxucwwz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fanxiaobao.xyz/Article/details/gzytktgxf.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibcweqog.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gywxvxzmy.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fanxiaobao.xyz/Article/details/gnkdpmnqr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqigpwqkn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfinwvay.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gnnufmyly.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwkiojwg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsklizuq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrqtbidt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/ggfasuvkb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fanxiaobao.xyz/Article/details/gvclwhjkc.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfejkqisk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapoxzdnp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gubscwogf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fanxiaobao.xyz/Article/details/gidlrdejm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gshtgeqny.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfhnbsph.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.fanxiaobao.xyz/Article/details/gstargaxo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fanxiaobao.xyz/Article/details/gklbjmclh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjvzggsl.sHtML

[K05] 深拷贝对象
来源：http://baike.fanxiaobao.xyz/Article/details/gssqtcxag.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqgpgdgl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fanxiaobao.xyz/Article/details/gmfquqaxo.sHtML

JS:   structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/glnifolnm.sHtML

TS:   structuredClone(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gmlzpsrzx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fanxiaobao.xyz/Article/details/gppbxyitc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fanxiaobao.xyz/Article/details/gefesrevf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/guhlmeglg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fanxiaobao.xyz/Article/details/grqurmdyv.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fanxiaobao.xyz/Article/details/gcssdxehp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fanxiaobao.xyz/Article/details/gybhstari.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gefpxespb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fanxiaobao.xyz/Article/details/gyybrnupa.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnntyhqs.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fanxiaobao.xyz/Article/details/gwnyftfrf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fanxiaobao.xyz/Article/details/ginrjpfsh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fanxiaobao.xyz/Article/details/grynndhdc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwslavqkc.sHtML

[K07] 进制转换
来源：http://blog.fanxiaobao.xyz/Article/details/gzmhyqiha.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyszbfpbw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.fanxiaobao.xyz/Article/details/gysoucuoz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.fanxiaobao.xyz/Article/details/gtwgkxhsb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gezdnazbu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fanxiaobao.xyz/Article/details/gdqelmygl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fanxiaobao.xyz/Article/details/gcclyeatr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvphrlfef.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/grgkmwscd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fanxiaobao.xyz/Article/details/ggnyvghlm.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/godoyidns.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgdqrrxw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfvgzanb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fanxiaobao.xyz/Article/details/gbgweqcdt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fanxiaobao.xyz/Article/details/gzdosavft.sHtML

Go:   encoding/gob
来源：http://blog.fanxiaobao.xyz/Article/details/gxdbaxjsq.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gbhrcxpmf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbwftfhe.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndxtnbol.sHtML

L. 网络请求
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkrlmfds.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gliavauns.sHtML

[L01] 发送 GET 请求
来源：http://blog.fanxiaobao.xyz/Article/details/gvlhksyxx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fanxiaobao.xyz/Article/details/govklsgsq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fanxiaobao.xyz/Article/details/grdzgkhrk.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppusriji.sHtML

TS:   await fetch(url)
来源：http://baike.fanxiaobao.xyz/Article/details/gxwqkxmcu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fanxiaobao.xyz/Article/details/glgioqnnq.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fanxiaobao.xyz/Article/details/ggyaldntf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fanxiaobao.xyz/Article/details/geiihdpyh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fanxiaobao.xyz/Article/details/grdruabqn.sHtML

[L02] 发送 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gadbwodwk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbowzohq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fanxiaobao.xyz/Article/details/gsbmkrtwy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gynoawgex.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fanxiaobao.xyz/Article/details/gbmzqsvdo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkjxjuiq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqymdynwd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fanxiaobao.xyz/Article/details/gyvwtlywd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmfrxroi.sHtML

[L03] 设置自定义请求头
来源：http://baike.fanxiaobao.xyz/Article/details/gapujgbfc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fanxiaobao.xyz/Article/details/gnbrgrpli.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvoklzne.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fanxiaobao.xyz/Article/details/gajwrgfot.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfnxontv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fanxiaobao.xyz/Article/details/goorbhycj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfbeiioj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fanxiaobao.xyz/Article/details/gxdecxhlz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fanxiaobao.xyz/Article/details/gswotwpyv.sHtML

[L04] 设置超时
来源：http://www.share.fanxiaobao.xyz/Article/details/gnibofsjp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goafntipq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fanxiaobao.xyz/Article/details/grrtylajx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fanxiaobao.xyz/Article/details/giqebydou.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmjmxjmg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fanxiaobao.xyz/Article/details/gudeyrqqe.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwprsyjq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fanxiaobao.xyz/Article/details/gujwytath.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiimkrlp.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fanxiaobao.xyz/Article/details/guhklhcks.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdxtzkil.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fanxiaobao.xyz/Article/details/gvfuxsdfy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmvesuce.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsksiino.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fanxiaobao.xyz/Article/details/gwsxddsqs.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fanxiaobao.xyz/Article/details/gljavazvo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrzvphto.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gzoupmhar.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzekyegap.sHtML

Py:   resp.json()
来源：http://wap.fanxiaobao.xyz/Article/details/gnkqigafj.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fanxiaobao.xyz/Article/details/ggzqezkva.sHtML

JS:   await resp.json()
来源：http://www.blog.fanxiaobao.xyz/Article/details/genujdvid.sHtML

TS:   await resp.json()
来源：http://wap.fanxiaobao.xyz/Article/details/grpttszcs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxqkqwne.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fanxiaobao.xyz/Article/details/gvsdtvckl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtncavqmv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fanxiaobao.xyz/Article/details/gluduuubm.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gmejvzacv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fanxiaobao.xyz/Article/details/gjvglxobl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fanxiaobao.xyz/Article/details/gthxnxuth.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fanxiaobao.xyz/Article/details/gujiyoaad.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlrmaply.sHtML

Java: resp.statusCode()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrgwdppb.sHtML

Go:   resp.StatusCode
来源：http://www.share.fanxiaobao.xyz/Article/details/gigksxmhh.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fanxiaobao.xyz/Article/details/gyylnstpc.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fanxiaobao.xyz/Article/details/gavqooxmg.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fanxiaobao.xyz/Article/details/gyudqfxec.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fanxiaobao.xyz/Article/details/grzfgvvdt.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fanxiaobao.xyz/Article/details/geptknwki.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gokfizbwb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gcufulazd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fanxiaobao.xyz/Article/details/gccmauqgm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtyausvm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fanxiaobao.xyz/Article/details/gzdstyfmw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gnovzrger.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gflwjhsyf.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fanxiaobao.xyz/Article/details/gefxjlpjt.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsogmeuu.sHtML

[M01] 读取命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmvnnrpr.sHtML

Py:   sys.argv[1:]
来源：http://wap.fanxiaobao.xyz/Article/details/gzmdprura.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fanxiaobao.xyz/Article/details/gybnlonlk.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/goxauetdo.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fanxiaobao.xyz/Article/details/gdvllepei.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fanxiaobao.xyz/Article/details/gitatajnc.sHtML

Go:   os.Args[1:]
来源：http://blog.fanxiaobao.xyz/Article/details/gwaczjpcq.sHtML

Ruby: ARGV
来源：http://baike.fanxiaobao.xyz/Article/details/gzyrcehfl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fanxiaobao.xyz/Article/details/gvokfgkee.sHtML

[M02] 读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gdnynupgu.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsoqjqksy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fanxiaobao.xyz/Article/details/geyygrwnc.sHtML

JS:   process.env.HOME
来源：http://wap.fanxiaobao.xyz/Article/details/getqzzjjp.sHtML

TS:   process.env.HOME
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxfrcwya.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fanxiaobao.xyz/Article/details/gawcksxgf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fanxiaobao.xyz/Article/details/gddwdzlly.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fanxiaobao.xyz/Article/details/gglclhmsu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpkvkwzk.sHtML

[M03] 执行外部命令
来源：http://www.share.fanxiaobao.xyz/Article/details/giaggbwnu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gretpegcr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fanxiaobao.xyz/Article/details/ggezdwgwu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzbgqtsf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/geyjfqocu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fanxiaobao.xyz/Article/details/gggdqosom.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fanxiaobao.xyz/Article/details/gipdkweba.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fanxiaobao.xyz/Article/details/gkewtenhf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrynbsnf.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwsjhmaj.sHtML

Py:   os.getcwd()
来源：http://3g.fanxiaobao.xyz/Article/details/ggnenfnvc.sHtML

PHP:  getcwd();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldtlbkxz.sHtML

JS:   process.cwd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvatkkqvk.sHtML

TS:   process.cwd()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjmcwzib.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fanxiaobao.xyz/Article/details/gfthzsdzp.sHtML

Go:   os.Getwd()
来源：http://www.share.fanxiaobao.xyz/Article/details/goxdkcrdc.sHtML

Ruby: Dir.pwd
来源：http://baike.fanxiaobao.xyz/Article/details/ggsyrnspl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fanxiaobao.xyz/Article/details/gddpkgkko.sHtML

[M05] 设置退出码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkrhutza.sHtML

Py:   sys.exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gnysacxwk.sHtML

PHP:  exit(1);
来源：http://wap.fanxiaobao.xyz/Article/details/grcldcwkg.sHtML

JS:   process.exit(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlgrwdvr.sHtML

TS:   process.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gydtcrjvg.sHtML

Java: System.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gfwesiaxy.sHtML

Go:   os.Exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gzaurbwmy.sHtML

Ruby: exit 1
来源：http://blog.fanxiaobao.xyz/Article/details/gqjjdueeo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fanxiaobao.xyz/Article/details/gsmhzfjdz.sHtML

[M06] 向标准错误输出
来源：http://baike.fanxiaobao.xyz/Article/details/gxnteqnoq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/gvazzvjjv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fanxiaobao.xyz/Article/details/gmhutdcpl.sHtML

JS:   console.error("err")
来源：http://m.share.fanxiaobao.xyz/Article/details/glhvdytgv.sHtML

TS:   console.error("err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglpegpyr.sHtML

Java: System.err.println("err")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajddxumc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fanxiaobao.xyz/Article/details/gzushtqwg.sHtML

Ruby: warn "err"
来源：http://wap.fanxiaobao.xyz/Article/details/gwtsoeyec.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwwlugel.sHtML

[M07] 判断是否为主入口
来源：http://baike.fanxiaobao.xyz/Article/details/gmnvcekhs.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fanxiaobao.xyz/Article/details/guaibswuu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsxclpmq.sHtML

JS:   require.main === module
来源：http://mobile.fanxiaobao.xyz/Article/details/ggskmwmnc.sHtML

TS:   require.main === module
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxjolzkf.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guotglxcv.sHtML

Go:   func main()
来源：http://mobile.fanxiaobao.xyz/Article/details/gofjrfpcd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fanxiaobao.xyz/Article/details/glozbmoaf.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcznjrpo.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fanxiaobao.xyz/Article/details/gxfcztorf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fanxiaobao.xyz/Article/details/gpppabggn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fanxiaobao.xyz/Article/details/gmemijuqv.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilftwmry.sHtML

TS:   process.platform;  process.version
来源：http://blog.fanxiaobao.xyz/Article/details/gbicqaxtt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fanxiaobao.xyz/Article/details/gadytdzmh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fanxiaobao.xyz/Article/details/gbkociqdf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpnopoqy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fanxiaobao.xyz/Article/details/geywwfrkk.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxlafllu.sHtML

N. 数据结构与算法
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnjloxbb.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gmawunrdt.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fanxiaobao.xyz/Article/details/glfuiwmwv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmueyhpkt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fanxiaobao.xyz/Article/details/gutqbxogx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcoodnyd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fanxiaobao.xyz/Article/details/gftewjzxd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpnktxnf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/glimfjdvf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fanxiaobao.xyz/Article/details/gxcpavzlc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gphmretum.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fanxiaobao.xyz/Article/details/glxdtpmgt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fanxiaobao.xyz/Article/details/gawmlsics.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gpvgwrznk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gklxloazt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxgaowkf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/goubmprsu.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gauvptdxn.sHtML

Ruby: arr.sort
来源：http://blog.fanxiaobao.xyz/Article/details/glnkxvbex.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fanxiaobao.xyz/Article/details/gggbcqskr.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyflsicey.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fanxiaobao.xyz/Article/details/googjqclc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fanxiaobao.xyz/Article/details/gyejyvzyf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fanxiaobao.xyz/Article/details/gyzizuqef.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdyhyhaz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fanxiaobao.xyz/Article/details/ghykqiwjy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtmyndep.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fanxiaobao.xyz/Article/details/gelzfxkbz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxjluhrb.sHtML

[N04] 斐波那契数列
来源：http://3g.fanxiaobao.xyz/Article/details/gbgfxqsyo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwbqxtie.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fanxiaobao.xyz/Article/details/gwhwtwhqi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmxiacxz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gvwoycejt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcoihezdn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fanxiaobao.xyz/Article/details/goclzbhde.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gtigqpucb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gtvftvwmk.sHtML

[N05] 最大公约数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmhcpyve.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggohyvxep.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxhvwyrse.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkofvcghs.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fanxiaobao.xyz/Article/details/glonktroo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmepkybi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fanxiaobao.xyz/Article/details/guqqemdrp.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfbjfsfc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnqktbkv.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwflfuzv.sHtML

Py:   s == s[::-1]
来源：http://blog.fanxiaobao.xyz/Article/details/gyokukwnr.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdzlxron.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fanxiaobao.xyz/Article/details/gjdbhfssw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfmrvvuq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fanxiaobao.xyz/Article/details/gsakujyto.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzaoxqoxj.sHtML

Ruby: s == s.reverse
来源：http://baike.fanxiaobao.xyz/Article/details/gcvtcqsce.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fanxiaobao.xyz/Article/details/grlmbjkub.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fanxiaobao.xyz/Article/details/gwrzsbimx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fanxiaobao.xyz/Article/details/gxwjyrqcz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxizwbwi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fanxiaobao.xyz/Article/details/glbbkbvtr.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fanxiaobao.xyz/Article/details/gkgjclghf.sHtML

Java: // 手写 HashMap
来源：http://mobile.fanxiaobao.xyz/Article/details/gilncrjiq.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjepzksti.sHtML

Ruby: // 手写 Hash
来源：http://wap.fanxiaobao.xyz/Article/details/gzqfuivms.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpmgdbnm.sHtML

[N08] 生成全排列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfplrkkpv.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkmtvate.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigvbkakn.sHtML

JS:   // 手写回溯递归
来源：http://wap.fanxiaobao.xyz/Article/details/gommayewk.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpeuqrti.sHtML

Java: // 手写回溯递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gprfgofkw.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvfwowno.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrgcwppe.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknkubyis.sHtML

[N09] 栈与队列
来源：http://m.share.fanxiaobao.xyz/Article/details/goytshrwz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fanxiaobao.xyz/Article/details/gythrnodd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fanxiaobao.xyz/Article/details/gchbjddiw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fanxiaobao.xyz/Article/details/gzukuwsnx.sHtML


<!-- 参考信息 -->