代发 wailian999

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gofmwseel.sHtML

K. JSON 与序列化
来源：http://mobile.hesvh.cn/Article/details/gwwzyoanj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqqlivvtq.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.hesvh.cn/Article/details/ggtgoffmp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/grtjakgsp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gmelpnvkc.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/grfvuwizf.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.zdbjq.cn/Article/details/gamwcwzob.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.zdbjq.cn/Article/details/ghtrkycvb.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.zdbjq.cn/Article/details/gpcfnxrfa.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.fehbvm.com/Article/details/gwnzwhpbw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fehbvm.com/Article/details/gbodatsrc.sHtML

[K02] JSON 字符串转对象
来源：http://blog.hesvh.cn/Article/details/grrzjljql.sHtML

Py:   json.loads(s)
来源：http://m.share.fehbvm.com/Article/details/gmpaslujc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fehbvm.com/Article/details/gmvlrezfw.sHtML

JS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gcxrytprl.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gnrnreqhg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fehbvm.com/Article/details/gamgicjiw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gzkoaqtcy.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/ghpwtvmhk.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fehbvm.com/Article/details/gcqbruauj.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.zdbjq.cn/Article/details/gaypqqkve.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/gyjrrgorc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/guctsjzwd.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gstqaolii.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gdqwdcrxo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.zdbjq.cn/Article/details/gbpedkais.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.hesvh.cn/Article/details/gvmyowjrz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.hesvh.cn/Article/details/getbgjgpi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fehbvm.com/Article/details/gdabprwnt.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.hesvh.cn/Article/details/gbjskdpim.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.hesvh.cn/Article/details/gavctizcm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.zdbjq.cn/Article/details/gguahqhno.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gbvillbnw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gobfpekog.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gphxjsesm.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fehbvm.com/Article/details/gcrexjtcu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gchacrpoh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/geqwpfpvd.sHtML

[K05] 深拷贝对象
来源：http://m.share.hesvh.cn/Article/details/gnjtuffpz.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fehbvm.com/Article/details/gpriqiakg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fehbvm.com/Article/details/gnnoiyrua.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gxeoqhsjm.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gbfhjgjds.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.zdbjq.cn/Article/details/gulydnvkc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.hesvh.cn/Article/details/gfwjxnhhy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fehbvm.com/Article/details/glxpzauhy.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.fehbvm.com/Article/details/griyiehlu.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.zdbjq.cn/Article/details/gcllxpjwt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.hesvh.cn/Article/details/gzvrnsktg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fehbvm.com/Article/details/ggktmeeha.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/gfxddxmvx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gsyofvote.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.fehbvm.com/Article/details/gtkvjakip.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/goorwoxcm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/ghmldlxhh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gvlkhkxhp.sHtML

[K07] 进制转换
来源：http://3g.hesvh.cn/Article/details/ggwvwkfrd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/ghvbwkqsc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.hesvh.cn/Article/details/glchwapyb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/guqokfvxq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/ggyhlhmyw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/ghgzxproo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.hesvh.cn/Article/details/gbnydbbui.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.hesvh.cn/Article/details/gdhtorfas.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.hesvh.cn/Article/details/grygrjqwy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fehbvm.com/Article/details/gumnrvnzt.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/guehnxhfo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.zdbjq.cn/Article/details/getfolqnz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gcytpabpb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gjwjmojya.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fehbvm.com/Article/details/giqkakwim.sHtML

Go:   encoding/gob
来源：http://blog.hesvh.cn/Article/details/ghodwqfve.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.hesvh.cn/Article/details/gksbbkgdo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gcbmjenxd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gutwztpvy.sHtML

L. 网络请求
来源：http://read.share.zdbjq.cn/Article/details/gipcpehdz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gaacidllf.sHtML

[L01] 发送 GET 请求
来源：http://wap.fehbvm.com/Article/details/gdhqelnqs.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.zdbjq.cn/Article/details/gxxoonfpt.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.zdbjq.cn/Article/details/gnravapsu.sHtML

JS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gtzjvcznk.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/geehmwfxk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.zdbjq.cn/Article/details/gadihdnyv.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/gepqppadg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/gntynovdu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/gmotrkkap.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/ghoywkohv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.hesvh.cn/Article/details/gtxnkmyby.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/gttdrvrjs.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/grwmlocdb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/giwraenoj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fehbvm.com/Article/details/gwphrtiqt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.zdbjq.cn/Article/details/gxqxywusq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fehbvm.com/Article/details/guitwpdzn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fehbvm.com/Article/details/gzzgiapnx.sHtML

[L03] 设置自定义请求头
来源：http://baike.fehbvm.com/Article/details/gyrgcbfjg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/gsdpjcddh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fehbvm.com/Article/details/gzhqpdwpp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gandwholy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gftrebquo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.zdbjq.cn/Article/details/glnupfvuu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gfarymxuh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fehbvm.com/Article/details/gprvzdcul.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gdwgfpvxo.sHtML

[L04] 设置超时
来源：http://mobile.fehbvm.com/Article/details/glzqxarih.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.zdbjq.cn/Article/details/grlynaeoq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.hesvh.cn/Article/details/gepnmtmgh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gtizyvaif.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/grdleubdq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/gepqhzdkc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/gqyniaxxl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/gcwuwewkm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.hesvh.cn/Article/details/gsxfqkwgc.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.hesvh.cn/Article/details/ggegaksmm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.zdbjq.cn/Article/details/gycdrtizy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fehbvm.com/Article/details/ginefnfpu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/guzodlwrl.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gsvchyhfq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/grqsdewiw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/grjcaqohk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.zdbjq.cn/Article/details/gpepuuhsk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/gqljfssip.sHtML

[L06] 解析响应为 JSON
来源：http://wap.zdbjq.cn/Article/details/gxmqpcqrj.sHtML

Py:   resp.json()
来源：http://read.share.hesvh.cn/Article/details/glbbaynnu.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/gjqcwxpix.sHtML

JS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gxxokhopj.sHtML

TS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gnienafpg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.hesvh.cn/Article/details/gnkwwomsc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.hesvh.cn/Article/details/gopeanysx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/gaqyaqhhz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/gvdngnluy.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/ghvcwpthd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.hesvh.cn/Article/details/gwboewkfj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/gvdsfylbh.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gnaqqzark.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gmwtevrgf.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/gfdixdmaq.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gybxcoofm.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/gnxazfyvc.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gzvogstak.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/ghzkhzwkg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gjvwfgitj.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gdcikckfi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/giafolaeb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/ggtpmijsi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.zdbjq.cn/Article/details/ghrkgpkjc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/gobzkfdfy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fehbvm.com/Article/details/gofzmkkjb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gbksfwwaj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqnizvtcs.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/gyzbvvbta.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdofpidcw.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/gcmouywql.sHtML

Py:   sys.argv[1:]
来源：http://m.share.hesvh.cn/Article/details/gozjgskrg.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/gqllkvvml.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gdxbbtbmz.sHtML

TS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gmjqnlagk.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gnggzeunq.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/gvdgythvl.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/gbuwnuwob.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gnnjjzizl.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gswleryze.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/ggrkwmcfz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gbpihzmpm.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/giqgkrhir.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/godcspbbh.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gsjjbdmvr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gxxnctxub.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/giroisvyy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/gyyvisgps.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gaquxupyf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/gwnvopbua.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gbxuoqjmc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gbzysounq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gdnjrwbix.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/gcmovbmqe.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/gckyiaqxe.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/gdfegbmsw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/ggfiacolf.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/gutcqhxxn.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gaanwuqmd.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/ghbglaemp.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gdubjtpjd.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/ggadakmhb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/gkzozpzug.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gweamkpsw.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/gcgisudid.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/gcyiercig.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/ggmhpxcbn.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gfgwdcxkn.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gwdvlkkzp.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gkqaboqge.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gubeqmqni.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/ggosorbpk.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gkburfhgq.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/gqccbpyoa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gicuolpll.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gsfvpwfjr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gwnncsxdn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gmrwmziyl.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gionjpcrv.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gtehqckko.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gzgskqibm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/gjxuzjjzp.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/ggvthsdlm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/gmhijglyj.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/gwrxqtmlm.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gjuncvnrs.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gpkfsowhp.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/ghqtxakch.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gsiwcefmo.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gtvufwrbh.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gkcsshwhn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gjoxoxtsn.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/gcpixuvpj.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gtoeshydz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/ghtbnesow.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gqiegzpoj.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/glulflwju.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gqojcteej.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/ggnbmnnxc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/gavmwflze.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gglobhviw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/ggmveliqw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghoxcpimb.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gjisjswdr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvqbhmnba.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gfrngurtw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gaxaqqwzc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/gxmfsraag.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gfnedicvb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gsmcluvtn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gejwawokk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gkcpugpnr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/gajnernwk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/geodskbdf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/gyxksunry.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/goagvqgpr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gihaqwhmv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/govdvbhjv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gerqsyhor.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/gvpzczste.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/ggiqxxrjm.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gvgyokyup.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/glwstmleg.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/gsxuslzxi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/giyqwlqkt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gfvzdrmlw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gapnpyxaj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gxjlzdbrx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/gebagqrgi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gyevjbxaa.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gtbbzoitd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/gxqjvfcza.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/gfwdvpgsz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gzjldniws.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gfhatefnl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gydqhxwig.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gpwjvmwwi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gmmilyams.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/grhtffoio.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gvdvgbtkc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gemicvkev.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gmhgjsngp.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gjtqdfryk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/gvsauorvh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gfmdzhosi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gyhbwgfyg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/ghydzgaue.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gmdrgvuxc.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/govgopsly.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gmvhgtwzo.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gmpcchjup.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gipceilbr.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gbovnfkuk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gtdnrxwth.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gfbegvnnk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/gcrptmgtu.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gbusaptja.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gvrwliqwy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gzzyxryjc.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/gkdilmzik.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/grtdrloud.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gtmrwyara.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/gmoxmlkkq.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gawhweecm.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gitsukosm.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gkoubprzp.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gznlgonjq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gdmfjzngu.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gloddlabl.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gidwkaqll.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gbonhhscb.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gdmlidsxl.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gbuezejjn.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gfmmpjwtb.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gmynmyymi.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gmqglfoif.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gyxkzbsfz.sHtML


<!-- 参考信息 -->