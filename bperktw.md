代发 wailian999

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwtseprrl.sHtML

K. JSON 与序列化
来源：http://www.share.fehbvm.com/Article/details/gmacvfdxh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcrzijmdg.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.zdbjq.cn/Article/details/gkjxoauxm.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fehbvm.com/Article/details/ghyevrzee.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/gugwrloph.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/gtcgnsjfk.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.zdbjq.cn/Article/details/gorgncfbm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.hesvh.cn/Article/details/gdghmqeum.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.zdbjq.cn/Article/details/gqsgfccam.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.zdbjq.cn/Article/details/grckhpxtd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.hesvh.cn/Article/details/gzrjggjgj.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.zdbjq.cn/Article/details/glpdghuwc.sHtML

Py:   json.loads(s)
来源：http://blog.hesvh.cn/Article/details/gkcrvorlj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.hesvh.cn/Article/details/gxvvcnabq.sHtML

JS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gibqpznrm.sHtML

TS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gxsnihqgf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fehbvm.com/Article/details/gzxurwjia.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gfqsmlbng.sHtML

Ruby: JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gcpizpabc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcrutbsqb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.zdbjq.cn/Article/details/ggbiiqmjd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/gdtwybddo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/guzypgsvk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gnkarmgpl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/ggdwgbjzz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fehbvm.com/Article/details/grayxgejs.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.zdbjq.cn/Article/details/gknksvmma.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fehbvm.com/Article/details/gutdxaenb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.fehbvm.com/Article/details/gjldmqftk.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.zdbjq.cn/Article/details/gsqaqlkni.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fehbvm.com/Article/details/gfjanavkm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.zdbjq.cn/Article/details/glutsczsi.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/gvczvlfrf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gfbmsinez.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.hesvh.cn/Article/details/gwfoketwp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gfjnilzus.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gouhzszcx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gqjmmxuxx.sHtML

[K05] 深拷贝对象
来源：http://3g.zdbjq.cn/Article/details/ggfidispo.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.hesvh.cn/Article/details/gbyjpnbdu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.zdbjq.cn/Article/details/gphggbnuo.sHtML

JS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/goaouiizn.sHtML

TS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gupvsbqrj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.hesvh.cn/Article/details/ghiebqepn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.hesvh.cn/Article/details/gkxlkmfvy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fehbvm.com/Article/details/gzwmrgiqe.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.hesvh.cn/Article/details/gfxlljgdo.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.zdbjq.cn/Article/details/gumiikpio.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fehbvm.com/Article/details/gdpgialjd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.zdbjq.cn/Article/details/gmiuquqfm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/grczakfvp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/gsbmsqlve.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.zdbjq.cn/Article/details/gkdeargfq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gxmszkphq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gzhoyuvor.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gayiljmih.sHtML

[K07] 进制转换
来源：http://www.share.zdbjq.cn/Article/details/gfrokobje.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/ggvhjvdbv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fehbvm.com/Article/details/gjteanvzx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gcvlftzhn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gzxdabkbm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gnzvewfsh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/gotmiwslc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fehbvm.com/Article/details/glseyibnk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gziuassij.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.hesvh.cn/Article/details/gxoawmiuw.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/glsoiqylx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gniwbcqqu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gglyxuftp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/getiqsnbs.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fehbvm.com/Article/details/gaqjubkcj.sHtML

Go:   encoding/gob
来源：http://www.m.share.zdbjq.cn/Article/details/gdmyckfvv.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.zdbjq.cn/Article/details/gmxtrxvxc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gymecbcvy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdmckbbyw.sHtML

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/gbvcfmcrk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gozvknpiz.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/gytwprpge.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.hesvh.cn/Article/details/gdotllnty.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.zdbjq.cn/Article/details/gsetwpozw.sHtML

JS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gxeeuzrzd.sHtML

TS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/ghufoqjrz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.hesvh.cn/Article/details/guyukqgay.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fehbvm.com/Article/details/gaxyrosqb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fehbvm.com/Article/details/gesevhkgn.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.hesvh.cn/Article/details/gxrbhezgy.sHtML

[L02] 发送 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gpigktcsi.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/glxystrbn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fehbvm.com/Article/details/gfqkgiwug.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gbmsheyao.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gsvhjjkzu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/gojiyyzvz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.zdbjq.cn/Article/details/gjuczwjbi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/gixuycmuc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fehbvm.com/Article/details/gujqitwuc.sHtML

[L03] 设置自定义请求头
来源：http://www.share.hesvh.cn/Article/details/gjqacctqq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/gjakpnuix.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.hesvh.cn/Article/details/gukhmeiip.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gzirkjnyy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gpbvuexnr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/gtnzizrnx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gcvmamgha.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/gympjjoah.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gukgryrwd.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gtznfxmqq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fehbvm.com/Article/details/gfwpznbzx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/gwnhndckt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gztbzungu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gfovtuolp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/gwamckkwe.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/gpgzzdesc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.hesvh.cn/Article/details/gijqetdot.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.hesvh.cn/Article/details/gwuccsysx.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/ggwiqitrf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/giskjkqhf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fehbvm.com/Article/details/gmezwtrjl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gwbrvpelh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gfrekapuj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gekdakorq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gqwnffgoo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gpacljgkw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gvyzjslqj.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gywlibjgt.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gcylrqelx.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gtftcurob.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gkmkvzpil.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gsilvmxrf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gtmxgshmn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.zdbjq.cn/Article/details/ghzcoberl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.zdbjq.cn/Article/details/gnadfgogl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.hesvh.cn/Article/details/gldxfzmvw.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gvopmuaii.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gnwvsjyte.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/gdlqcplcm.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gjgoaadgq.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gdotbczcs.sHtML

Java: resp.statusCode()
来源：http://www.m.share.hesvh.cn/Article/details/gzamexsbu.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gmavlhbam.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/gteticzgy.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gjlxwxmvw.sHtML

[L08] 并发请求多个地址
来源：http://wap.zdbjq.cn/Article/details/gimyfjhny.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/gvmznlmfy.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/giqeaytrh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gneypvopo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gdxnmrrdm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gnprdybdn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/guougmxaa.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fehbvm.com/Article/details/gyrnsvzli.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fehbvm.com/Article/details/gyciecacc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpsrufqva.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.hesvh.cn/Article/details/gnckuzdmt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnzkonxpp.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gzuaulywo.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gnpglswgl.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/gozykovyw.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gcfwoyejt.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gzxczinkv.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gjcswsfcp.sHtML

Go:   os.Args[1:]
来源：http://read.share.fehbvm.com/Article/details/gwkolllux.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/grlsshwvt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gqtnaruyy.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/gkosbtuoz.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gffrnpinz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gazoszikk.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/ggemvbvye.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gffzmyekv.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gspanxdkw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gicfbufzk.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gtkfxmqba.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/ghnypjsti.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gvexrkveg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/ggmcafstc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/ganqlfepr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gabfaxprx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/grplbzqyc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/gzxjwcucx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fehbvm.com/Article/details/gmngjmoco.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/gsuoymxmk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/guaarscvw.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gbnprzrfr.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gnsknjitb.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gqnxapoem.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gdtjxraxt.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gzrywrgdw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/goardbdwr.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/gornhxutm.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gmibfxfbg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/gymbnfrld.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/glnlspljo.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gedjhwmfu.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/govigrufp.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gewgbdled.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gcahttriy.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/gekekahpl.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gzajrcfzo.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gfdksktuv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/gfeejcbia.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gcqfgwhws.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gwofgwyck.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/gxentgnmh.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gxggeenyx.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gkxoeqzwc.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/gpwifqfhv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gtmprujqs.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gaucgvlms.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gczbpmivo.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gjzzstkfl.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/gfrlbbsxe.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/ggtcvwvqv.sHtML

JS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gpmhezfly.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gbisrxzcl.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gulgioyva.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/guhkmlpas.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gevpphamz.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gdbfohwws.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gklzyacgj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/gfmufrzyo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gcafhwirj.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gmmjjixqg.sHtML

TS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/glluaykrb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gitnledhj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gffywmtjd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/gqzloafhq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/gwftatufx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqlygzdfe.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gyejqszgj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcgrzsxpj.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gmbfwuuam.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gzcdkbmmm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/grmzkhszk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gtnduvusb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/ggvddideb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gjkdohbsg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gshhbfyfd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/gxrbaekud.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gyizlkmbp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gxtwqrgqx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gmuqdtyyb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gbqaouesf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gzrcvvehf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/guideeswf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/goruqufgd.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gzjxnhngz.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gukjfxjgz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gdrdjhmnr.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gvqxltmhh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gncalkwgy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gascggddj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gfjogpyxl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/ghsblcwef.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/ghqashsqj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/glsucfleg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/glxxpvviu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/gtnazttzq.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gckwurzja.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gyncfoftn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/glugpncih.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gpbjpzcvg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gxqyvewuh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gfulsjebo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gudrbjboo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gsnhszeyf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gevtzzdez.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/guhdqjhkv.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gufwecryy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gydxsifof.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/galmbovdt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gycehsiop.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gkfdjxsbw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gmemgwuie.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/ghljjgknh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gcbllxxlb.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/gtwfgwhbx.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gozxrxkfb.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gmojzlbws.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gnamqpnpm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gajmlfife.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/grdbfytqn.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gwnysvwwp.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/guvrskiiu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gtqqoglph.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gzgaunqvt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.hesvh.cn/Article/details/grrjeiwdv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/ggnckdifm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gjpffuqlf.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gsmorisih.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gljncnovu.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/gcpitblef.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/grhdnruxv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gxjfuwxqe.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gdmsyunij.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/gymqudwky.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gurewtzfk.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gbgwqrltu.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/glytrzhlm.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gthjtbamv.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gkqwgwosw.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gsavccjua.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gyvbaccgz.sHtML


<!-- 参考信息 -->