代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/geafqlhbi.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gjalwgijd.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/gjwjezcrm.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.zdbjq.cn/Article/details/gecpnorgp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.zdbjq.cn/Article/details/gyudtpzoz.sHtML

Go:   json.Marshal(obj)
来源：http://3g.zdbjq.cn/Article/details/gtuihqbks.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.zdbjq.cn/Article/details/gtztqrrwg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.hesvh.cn/Article/details/gjhyuiykq.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.fehbvm.com/Article/details/gucushwgs.sHtML

Py:   json.loads(s)
来源：http://baike.zdbjq.cn/Article/details/gchxujuar.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.zdbjq.cn/Article/details/gufuygcwo.sHtML

JS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gilbopmkb.sHtML

TS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gsmuvnjlq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gfccmfrgt.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/glhdmsmyk.sHtML

Ruby: JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gfsqtlwns.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fehbvm.com/Article/details/ghetbgdtb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.hesvh.cn/Article/details/gzkbhhvbx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/grgqkofxn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/grkroxudc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gryozloeo.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gkpryzhra.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.hesvh.cn/Article/details/gbafmahbh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.fehbvm.com/Article/details/glrqzrkrs.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/grnwostyn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.hesvh.cn/Article/details/gucyrorpp.sHtML

[K04] 读取 JSON 文件
来源：http://baike.zdbjq.cn/Article/details/gujacntox.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.zdbjq.cn/Article/details/glaxxmqof.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.hesvh.cn/Article/details/gsyhpwkyo.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/gypkqzugv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/gehiqgbwt.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/goiwtkrka.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gmcjitolh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gqbajydik.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gttaofsxl.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.hesvh.cn/Article/details/gprltrivl.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.zdbjq.cn/Article/details/gktlsqwla.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.zdbjq.cn/Article/details/gyqqfuycs.sHtML

JS:   structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gjravwwmc.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/goryyorfr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.hesvh.cn/Article/details/gygworeci.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.zdbjq.cn/Article/details/ggwdefbmj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.zdbjq.cn/Article/details/gecdssedi.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.zdbjq.cn/Article/details/geoetmmos.sHtML

[K06] 解析 URL 查询串
来源：http://blog.hesvh.cn/Article/details/gsuyconrz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/grviospaj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.zdbjq.cn/Article/details/gusugdazx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gvlwfwxem.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gconowkzr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fehbvm.com/Article/details/gtgyfzhwx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gssgkvnot.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gcjtwmnna.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gairzggqe.sHtML

[K07] 进制转换
来源：http://wap.fehbvm.com/Article/details/grpdhcdgj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.hesvh.cn/Article/details/grshonmqg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.zdbjq.cn/Article/details/geqooezsc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gfvjcrigr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gtujbxnke.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gvafkgknu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/gzwzpwzkf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.hesvh.cn/Article/details/gmlwecidi.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gwmwuvpwg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fehbvm.com/Article/details/geckiknpd.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.fehbvm.com/Article/details/gvkakudbq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/gcyntulkg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gvtvkeqtm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gdsngplab.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.hesvh.cn/Article/details/ghnuwxwtd.sHtML

Go:   encoding/gob
来源：http://www.share.fehbvm.com/Article/details/gcxinooaj.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gdpnzcfho.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gffqvhmve.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gekasgyxu.sHtML

L. 网络请求
来源：http://www.blog.zdbjq.cn/Article/details/gyxpgsomv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gknpissuu.sHtML

[L01] 发送 GET 请求
来源：http://wap.fehbvm.com/Article/details/gizywxtje.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.hesvh.cn/Article/details/gyflprncy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/grhbfecdc.sHtML

JS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gqytitgsh.sHtML

TS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/ghvxnebao.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.zdbjq.cn/Article/details/gwfeevhtr.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/gbmrdetzn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/grwhnuclt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.hesvh.cn/Article/details/gbuhbbjtr.sHtML

[L02] 发送 POST JSON
来源：http://blog.fehbvm.com/Article/details/gmlqarfei.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fehbvm.com/Article/details/gqsmaszyt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.hesvh.cn/Article/details/gnnhwqoqz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gjcxaaulb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gioanrdqi.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.hesvh.cn/Article/details/gdichntyp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fehbvm.com/Article/details/guqiylgyd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.hesvh.cn/Article/details/gifdylcno.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.hesvh.cn/Article/details/gcfrvotyc.sHtML

[L03] 设置自定义请求头
来源：http://www.share.zdbjq.cn/Article/details/gesslawaq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.fehbvm.com/Article/details/gghkiryqw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/gtnpzksyh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gnasskueh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gbxreyvbo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/gwjlxytuk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gmdxjrvoj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.hesvh.cn/Article/details/gghwfrdaa.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gtgdwxbcr.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/grfpzsmvs.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/gjinkfava.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fehbvm.com/Article/details/grjzgqigc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/garnjsvju.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gtacqmxwf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/gvkodmjlh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.zdbjq.cn/Article/details/gypvqsiaq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/gtyqhwldf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/gzfoatgpf.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/gsckvwevf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.hesvh.cn/Article/details/gmgxnevrr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/gwmqsyuam.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/geqmijufq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/goqqxzzkt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/gcepfihev.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.hesvh.cn/Article/details/gdzywjpbv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fehbvm.com/Article/details/gudxeznik.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gtgoayuiu.sHtML

[L06] 解析响应为 JSON
来源：http://wap.zdbjq.cn/Article/details/gpvcgblzj.sHtML

Py:   resp.json()
来源：http://read.share.hesvh.cn/Article/details/gaqimynog.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/gvdbbtrva.sHtML

JS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gumfoufue.sHtML

TS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gzitixtsu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.hesvh.cn/Article/details/gcqnmfmhp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/gvztocnwy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fehbvm.com/Article/details/gjxhxbrwt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.hesvh.cn/Article/details/goyvnirqr.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/glmcjoymg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.hesvh.cn/Article/details/gkwuzdnht.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/gahlfhnki.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gooirwxtp.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gntvuzwun.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/geencfcde.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/guffsouel.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/gkahgxhuv.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gpupcnlgv.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/gkbkgamui.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/gouatlvnd.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/gtmiqsfui.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gbhmijvvq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gqkhpltqp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/grjjvgxvj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gtksghqsz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gbpwvkrxk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gxregiaqr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gndbnuang.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/gkgpuxdew.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwainnzxj.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gbqbwyvua.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/gqtdsihnf.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/gdubobbvo.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gnpndjvxw.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gzkzsgpdp.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gezoaiswq.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/giwfzsmgv.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gyccrilnx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gwuojicjo.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/giloohklv.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.zdbjq.cn/Article/details/gxkeogdmr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gwafzpiyf.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gkxtedkao.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gdxxjpmno.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gvbofmlmx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/geqwyhtga.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gwyprqchy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/gflyewkaf.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gqbqqrkud.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/ggzudaagv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/ggxwpxjnj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gssgpopvi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gfseatokt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gfmqbbolg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/gphjmfdzf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/guejhacxu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/gloerudvy.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/gfxslnycp.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gjhtpnbov.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/gtkbdhoab.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gqymxtoky.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gxoqsvlyw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gykavnawa.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gwxvhwjes.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/grtlohlzb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/gmjlqpqqj.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/gezcxxyjf.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gtnzoecwl.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/gbwclgznn.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/grqrbnyio.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gxhoibbcb.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gyafqwpew.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gknadbdom.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gfvwatpuc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/gvtvmktex.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/georzolco.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gqbjqwkwn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gduttxawr.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gkvdgyrxv.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gptmutqtm.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/gsuxchmih.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gebatlwrj.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/gtvhydyzo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/grypdihgt.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gerdseyqv.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/gjnacjmhz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gojmwhiae.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/guknekszo.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gocbccsjb.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gbgtmxqwf.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/gpleflhwr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/gvqfnqqnm.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gfyualgta.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gtriwdrun.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gmicpbcbl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gueceubpi.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/guokvnfnw.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gfdluhbyo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gdzbeaxoy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gatohxiek.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gvqfzjmjf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gjdpbvkis.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwzhfjduu.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gutdlxdsz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzzpvrofe.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gzackhsqn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gfksbprzj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gijizxhqv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gyjaomwfw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/grdrmbkzy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/guvbzfemu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gmcqmuaqy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gknmjhmft.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gupcquwzv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gfcnabgpo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/ggslaomuw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/giqqazevs.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gwsyhgola.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gewvkuqrn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/gsszlnrwv.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gmipgeiaf.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gqqiqdcpb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gqbunqqny.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gayznoenx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gqgwvkoph.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/gaglbnmlj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gvyeyaoep.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gbbuncplg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gmhnftbwc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gxwoyysnu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gxvcesyxp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gmlfwjwyo.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/giynbhwbr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gqcmikmia.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/gwqxhlpqo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/glpuecsrf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/ghhaetdiv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/gemxtsutf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gitbbnhrk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gzkgnzljw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gqezdkyzs.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/grngryvwx.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/gghbwkxto.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/galhbqttx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gfqrrhcgr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gawyrwugf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/ggygvuekg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gyyntowfq.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/gcefptbpx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gaiendszm.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gmxawsker.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/giohvppzi.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/gyyvluthr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gyhkrmewf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gfhvtntdv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/grjsbhsnq.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gjmxfsoon.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gjlcpmnwi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gcsrculwk.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/grqkifsuv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/glikejlje.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.hesvh.cn/Article/details/ghlzmnbwf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gzottnaia.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/ghqinujcp.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gqyesmhub.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gvtnczthk.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gpqljcppv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/grksnrmwt.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gwuhehywg.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gwcepylhc.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gbssudjgg.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gjseyealq.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gjqbvbkyw.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gcoqdkeup.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/ghlqsqrjm.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gusiusmjl.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/garcgspyn.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gslhpeuzz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gcfbqpkbc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gzxrrodmg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gfxnkrhmc.sHtML


<!-- 参考信息 -->