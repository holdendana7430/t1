代发 wailian999

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbwspvytg.sHtML

K. JSON 与序列化
来源：http://m.share.hesvh.cn/Article/details/gyaeyzosg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfdrdwakp.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.zdbjq.cn/Article/details/grpravhid.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/glessrdri.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/gwfowemqp.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/guaqdathc.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.zdbjq.cn/Article/details/gcyvlfopl.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.zdbjq.cn/Article/details/gahavfvwg.sHtML

Go:   json.Marshal(obj)
来源：http://3g.hesvh.cn/Article/details/gzkiagnvl.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.zdbjq.cn/Article/details/gmbvmezzs.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fehbvm.com/Article/details/gslgclqgi.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fehbvm.com/Article/details/gifdezybq.sHtML

Py:   json.loads(s)
来源：http://www.blog.zdbjq.cn/Article/details/gdsvhqdja.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.zdbjq.cn/Article/details/gbaipjlxt.sHtML

JS:   JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gpwbmcdub.sHtML

TS:   JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gllltdcku.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.hesvh.cn/Article/details/giuprfvuh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/gprxyrczu.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gesjyppbs.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fehbvm.com/Article/details/goezmlgyt.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.hesvh.cn/Article/details/geysnibmb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/gqdxihomr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/guedtrwgf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/gkbknafio.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gmfzxudjd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.zdbjq.cn/Article/details/gbitemxck.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.zdbjq.cn/Article/details/gxbeattyq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.zdbjq.cn/Article/details/gxaalqute.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.zdbjq.cn/Article/details/givgwjpsk.sHtML

[K04] 读取 JSON 文件
来源：http://blog.hesvh.cn/Article/details/gjmastoqd.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fehbvm.com/Article/details/gajowfvza.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.hesvh.cn/Article/details/gegjurcmj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/glloatlbo.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/gjvnxmwzm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gvgzjstvk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.hesvh.cn/Article/details/gqleavmdm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/gkprpffqx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gxsyykzmb.sHtML

[K05] 深拷贝对象
来源：http://www.share.hesvh.cn/Article/details/gkkuuucii.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.zdbjq.cn/Article/details/gbdjatwjt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.hesvh.cn/Article/details/gayibpbwm.sHtML

JS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/grjhjwfsk.sHtML

TS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gwtoocnbk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fehbvm.com/Article/details/gotlyiaev.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.hesvh.cn/Article/details/gohqcbwgj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.hesvh.cn/Article/details/gegotkbhs.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.zdbjq.cn/Article/details/ghwgttsnl.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.zdbjq.cn/Article/details/galdxspqt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gyjwzweba.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fehbvm.com/Article/details/gjwqfsiqn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/getdmihsa.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gzgbovmiq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.zdbjq.cn/Article/details/garnoiznc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/grthfzpcl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gnvtbqism.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gnnarkkax.sHtML

[K07] 进制转换
来源：http://mobile.zdbjq.cn/Article/details/gnhygbvaw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gguswpedu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fehbvm.com/Article/details/gyymhldih.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gjudbsble.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gyxvmttra.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gpycgqodm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.hesvh.cn/Article/details/grbtkiihw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fehbvm.com/Article/details/gfujhdqhd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gtgdfmpsi.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.zdbjq.cn/Article/details/gbbluiqrg.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.hesvh.cn/Article/details/gnjlvbxvq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.hesvh.cn/Article/details/glfcomkzt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/grpefdzay.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gkkhluejg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.zdbjq.cn/Article/details/gtrabaawp.sHtML

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/gwitwitou.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.zdbjq.cn/Article/details/gnrkptxjb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gqehrrnxm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gumdkomqr.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/gtovwxkhp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gswnaepwr.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fehbvm.com/Article/details/gosumibrp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fehbvm.com/Article/details/glkpqfjjx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.hesvh.cn/Article/details/gwjbnldzr.sHtML

JS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gbvmauyot.sHtML

TS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gnoszcpmo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/gitfjsrxq.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.hesvh.cn/Article/details/gcsrdmgec.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.hesvh.cn/Article/details/gefqtahtt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.hesvh.cn/Article/details/geosybtmi.sHtML

[L02] 发送 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gipqmcmur.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gdhekzxzn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.zdbjq.cn/Article/details/gzaqkyehd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gxktmzcma.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/ghimyjcak.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.zdbjq.cn/Article/details/gsgleqadm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/gdcgjxpii.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fehbvm.com/Article/details/gqifuemhb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.zdbjq.cn/Article/details/gjygveghb.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/grfraoafe.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fehbvm.com/Article/details/gxjxmorhe.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.hesvh.cn/Article/details/glgusadsv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gkdxodtal.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gjnnbccys.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/golmgcojp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gaomayvlp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fehbvm.com/Article/details/ggnpmzjuv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gaagqozel.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/grungtldm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.hesvh.cn/Article/details/grqwivdkh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gyczqkcfq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gnynudcvv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gbedfpexy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/gnniabarg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/gxylzdcms.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.hesvh.cn/Article/details/glfwwjkxj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/gflorrggg.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.zdbjq.cn/Article/details/gnfnogjml.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fehbvm.com/Article/details/glfmesfmy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/glapzjgzr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gnkhiiqxi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gxyylixes.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.hesvh.cn/Article/details/guposfbof.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/gsjooppye.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.hesvh.cn/Article/details/goelpiccz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gneyioptf.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fehbvm.com/Article/details/goajszcct.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/gvgklyulu.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gwukxzzde.sHtML

JS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gxhtlmqxq.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gunfujyaj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gjbsfhihr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/ghrzbjxun.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.hesvh.cn/Article/details/ghqhxqcvw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gikrtnhlc.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gieqmusca.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.hesvh.cn/Article/details/gzxbngylb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.hesvh.cn/Article/details/giqszbymv.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gaxtzypsz.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gfrwljufd.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/guuokrmtf.sHtML

Go:   resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gbakpenpr.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/gzgpxqchw.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gxozglwxe.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/gkqrypgie.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fehbvm.com/Article/details/gdlogyfot.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fehbvm.com/Article/details/ggltjesyl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gdmyiwytt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gphmmommx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/gdcxhjlff.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gpgdfrubo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.hesvh.cn/Article/details/guazydrks.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/gbwvvarty.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmddoizti.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.zdbjq.cn/Article/details/glrhncusl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/giptwxdjw.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gwvfmigff.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gyxydymtv.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gsgedwchr.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gnqcgpqix.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gpkfwisfx.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gbndawtry.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/ghgnjupei.sHtML

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/gpqxzdlow.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gqbyrcoiz.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gczpptedr.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/givodwxzc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gosbumhxe.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gbaqwuywz.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gohivabva.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gxvxketdn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gqkqltytp.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gysghnbfp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/grbbpegiq.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gjwtynsch.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/gsmoshzgg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/gcragkrvv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gklrohvfe.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gdoiozvdl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fehbvm.com/Article/details/gbsunvbya.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/gdetwhrsu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fehbvm.com/Article/details/gwmzwlzxa.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/guhhmwggv.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/gqvzyndos.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gxoskkakz.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/gzjkbvqph.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gvvuyzcwl.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gpjvkooum.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gpkvufffw.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gvnkzdmiu.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/gqqgfufwo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gxulkqskg.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gavmqmjyl.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gpwtantnj.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/galnzcbps.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gcagmfduq.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/girzyuabi.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gwkmojsdg.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gnzgvugri.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gudtbllof.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/gurxdxiwz.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gpgwpkeaf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gtubplwzy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gakettdgc.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/getticplh.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/ggqcliidk.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/gffmsoagq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gbyrhkpva.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/gcehiofeu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/ggjrqbfyu.sHtML

[M07] 判断是否为主入口
来源：http://m.share.hesvh.cn/Article/details/gplzxkfnb.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/gwusauvhp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/glpmudslx.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gsxwyuvuq.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gupkbvjie.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/gycfvnvgc.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gyzybfezz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/ghpbleagd.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gqsopquju.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gfayyihhp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gmbsslplo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/grxtkmgrv.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gdhwdgfvb.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/glclqdxjm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/govtojcbl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/ghjykrmnp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/gkyauload.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gbjlhkkpm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gouwzfrvd.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/gfsvljwyh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gumbegxqh.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/geuhwqchh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gqooipgys.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gilwmqgvp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gxinfwvsi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gesxrqbuu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gxzohbwlr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/grbzpsiek.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/gmxvozlbi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/grrgzabfo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/ghmraejld.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gezvgxgnm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gtcmqhxao.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gyynncmwk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gkmjpvllf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/gofpgzcxe.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/ghcatyzkq.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gurcgkoej.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gxjfxunhh.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/gxprnlomp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/grtxhzugh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/glgptsvzw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/ggbgcnbcv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gpffpywas.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gsppskqio.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gpagavjyn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/gstbmmtvq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gibwrtljb.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gtcfsyalb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/glthjmfka.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gddtccofg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/geuwglsjd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gvhznbktk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gxxlfrxdg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gwpvdrrmn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gjrhxpjnt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gujtyiynq.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/gaydlejbj.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gzlogseul.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gqdomzpee.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gzeuxrnoy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/grnckwbav.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/guajatwzl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/gevpfliib.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gopaoqpcx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggaxorttb.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gibugxuna.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gkwdwwiqm.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gvumcvyua.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gxsgzvcfk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gcshdnnhh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/gbgegrzja.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/gagrvidvn.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gbvyjuqck.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/grguoscke.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/giynbvrjq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/glduqpprn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/gzjujhpoq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gyjjguhsh.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gvdkivgps.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gtfhvzusd.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/goiwnvnuf.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/gokagbseo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/guooqijnz.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gmcaqhjyp.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/grbueoqzr.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gccnkfeuh.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gmqzcgjdk.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/ghhhdzube.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gcuzkbcpj.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gakvfbfcv.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gvnuvubkg.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gihwnnclo.sHtML


<!-- 参考信息 -->