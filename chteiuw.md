代发 wailian999

================================================================================
来源：http://3g.fehbvm.com/Article/details/gacrigzfy.sHtML

K. JSON 与序列化
来源：http://read.share.zdbjq.cn/Article/details/gilpxgvxz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsbvuswud.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.fehbvm.com/Article/details/gqruvrigp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gwwkrspny.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.zdbjq.cn/Article/details/gzbnnbkbj.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gyqvftdzn.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.zdbjq.cn/Article/details/gldpapeqt.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fehbvm.com/Article/details/goowxzsjp.sHtML

Go:   json.Marshal(obj)
来源：http://3g.fehbvm.com/Article/details/gbymjawqe.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.hesvh.cn/Article/details/gncnxdtgx.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fehbvm.com/Article/details/gsxtrxhdl.sHtML

[K02] JSON 字符串转对象
来源：http://baike.hesvh.cn/Article/details/gclqsxess.sHtML

Py:   json.loads(s)
来源：http://mobile.hesvh.cn/Article/details/gwotwqgmt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.zdbjq.cn/Article/details/goymcccbx.sHtML

JS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gnscqdbdg.sHtML

TS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/ggkkvrymq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.hesvh.cn/Article/details/gvpzxwyux.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gaczczybe.sHtML

Ruby: JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gjwlezqda.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.zdbjq.cn/Article/details/gctqoodhe.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.fehbvm.com/Article/details/gtulwlvxi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/ghsofiatk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gaakkdxpe.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gzkgpqldi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gednjbicb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.hesvh.cn/Article/details/ghshgxtvv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.hesvh.cn/Article/details/gimggkiul.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.zdbjq.cn/Article/details/gkcnndwoe.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fehbvm.com/Article/details/geotpdbmw.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fehbvm.com/Article/details/gkhdutmws.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.hesvh.cn/Article/details/grathziuf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.hesvh.cn/Article/details/gwmaeloge.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/gnbysocud.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/gkotqavaa.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gskcdlunt.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/gmmskkpga.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.hesvh.cn/Article/details/grarkpcad.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gshfodyxf.sHtML

[K05] 深拷贝对象
来源：http://baike.zdbjq.cn/Article/details/guaxcujun.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gszphisns.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fehbvm.com/Article/details/gseeclzaj.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/goivnwmca.sHtML

TS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gpsdbwmsf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.fehbvm.com/Article/details/gheqkiyqs.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.zdbjq.cn/Article/details/gznxfbpwn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.hesvh.cn/Article/details/gqwhrmzhz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.hesvh.cn/Article/details/gsgpncbnz.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fehbvm.com/Article/details/guyyqthyh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/ggubzvcnd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.zdbjq.cn/Article/details/gqcwkszdr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/gvvvdlcld.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/guugbrqog.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.zdbjq.cn/Article/details/ghqmreejr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gdfodoqmz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gabaknszt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gygdysnbr.sHtML

[K07] 进制转换
来源：http://www.share.zdbjq.cn/Article/details/gshglkxia.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gjggnndfg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fehbvm.com/Article/details/gzqdlnhsb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gmibjmfpy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gxqeqyrfr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gwqxpkfgg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.zdbjq.cn/Article/details/gybyihpau.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.hesvh.cn/Article/details/gyfpqpjqw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.hesvh.cn/Article/details/giocylcgb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.zdbjq.cn/Article/details/gpkzterao.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.hesvh.cn/Article/details/gicwactik.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.zdbjq.cn/Article/details/geheahfvf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gkqgsnkgv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gdpnnicpb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fehbvm.com/Article/details/gyzcejfts.sHtML

Go:   encoding/gob
来源：http://3g.zdbjq.cn/Article/details/gwgzmquij.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.hesvh.cn/Article/details/gpnevgxss.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gaqyscdqi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzrtsxudk.sHtML

L. 网络请求
来源：http://www.blog.hesvh.cn/Article/details/gxnnscvyz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gamzwnxpd.sHtML

[L01] 发送 GET 请求
来源：http://3g.hesvh.cn/Article/details/gwnsjmrbz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fehbvm.com/Article/details/gsaqeektq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fehbvm.com/Article/details/guaackcax.sHtML

JS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gtfrzyzwx.sHtML

TS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gnyilaztx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.zdbjq.cn/Article/details/gbtvgirlj.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/gvjrpkoqf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.hesvh.cn/Article/details/goioxhyjv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/gqixiwqsr.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/gavqjshah.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/goxisvvcp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fehbvm.com/Article/details/gjpoowcwh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gpwsxowom.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gijdanfoj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.zdbjq.cn/Article/details/gtkrufkpo.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fehbvm.com/Article/details/gxqvtmbzl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.hesvh.cn/Article/details/gzqdfyogy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/gizsvcnpl.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gaafvfxhm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.zdbjq.cn/Article/details/gpakrmtoo.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fehbvm.com/Article/details/giqsauvba.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gpwsvuumh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gimzqlowf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.hesvh.cn/Article/details/gjzhtinpw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gamnpwlrs.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.zdbjq.cn/Article/details/ghpvlgybf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/grepehkvv.sHtML

[L04] 设置超时
来源：http://www.m.share.zdbjq.cn/Article/details/gkobhypys.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/getqezvka.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/ghtbvifae.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gervvmgom.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gtoifrcqf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gdzrfabio.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/gougrwdpt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/gcnycimao.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.zdbjq.cn/Article/details/glimqrtfa.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fehbvm.com/Article/details/gohegokgn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/glcddegkx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/gubskduda.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gffgmbnqx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gdtjuttyh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fehbvm.com/Article/details/gdasqujib.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fehbvm.com/Article/details/gtgafzcts.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.hesvh.cn/Article/details/gilehbsfx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fehbvm.com/Article/details/ghcbpustw.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fehbvm.com/Article/details/gdltcfefg.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/gaoqypcpi.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/gahsuogxi.sHtML

JS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gkhxwxblh.sHtML

TS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gshzvirie.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gdcdctgld.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/groesjyrl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/ggcqpbmjo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/ghqvjleky.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/ghxmdfrpf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.zdbjq.cn/Article/details/gcweoubqf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/gjnacxbyv.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gsthnylfu.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gizwqorrn.sHtML

Java: resp.statusCode()
来源：http://read.share.fehbvm.com/Article/details/gopgiygsi.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gqzjfluin.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/gwcvnkkdo.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gnxqctfpe.sHtML

[L08] 并发请求多个地址
来源：http://blog.fehbvm.com/Article/details/gasqgmknj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fehbvm.com/Article/details/ggivxxsbv.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/gwvgyjivu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gdwzmhdqd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gxokinagi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/guwtoipfo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/gozwgvhzh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.hesvh.cn/Article/details/gnjrrezej.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/geclcbsze.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvcqwoqxl.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/gdihzcmfg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gggmknane.sHtML

[M01] 读取命令行参数
来源：http://m.share.fehbvm.com/Article/details/gostvoplh.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gittgfzoh.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/gboghumku.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gyryjvihs.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/grxistqja.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gfhfixfwd.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gnnbufvgv.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/gzdbnmprd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gactrxowo.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gkzyrvyxc.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/goadajzlk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gegrewunw.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gymlnjfce.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gsyqydhqo.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gvxyykzgv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gksarfmoi.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gxrartfvj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gzhqwngct.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/ghnbvkosk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/ggbevvmab.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/gdmwwnjkg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/grxahwlju.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gcxtpqwjl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gnkbwomhp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gecoawans.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gooeadzlu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gcikctxza.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/godmxepqb.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gmqrxxtrd.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/gtimfnrpp.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gktmwjctb.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/guitlburk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gobbdjbuj.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gpwvwagjc.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/gjeejhiwy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gfwqswmre.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/galjzdzsu.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gseefyrns.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gvzginbbi.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gwkaxfrsl.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gnihqsfhu.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/ggmfqkxrl.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gatdetxfv.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/gpafzunib.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gwcgyfkwa.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gtjgskuys.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gdnoqaqod.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gnirnsjco.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gethxqews.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gzvykuyff.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gclpprbjz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/gtcbnscvo.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gfgldeeez.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gghnsfofe.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/gvnbwcmhu.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gpfocipsg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gohqdenzn.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gcghmqfsz.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/glqnjlbgi.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/gwfttdenk.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/gzelrtfol.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gkmvncewg.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gvepwpgwh.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/gndcrwzim.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gjvsxmfzn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gkqtjuzfc.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gqvtqhhjy.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gjnnkegbs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/gnpaoregb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gdccpbcvy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gjpgqkdjj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gwirjobwg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkntuvbie.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gafmqvtrr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghvtiroco.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gptojktiy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/glbzroozj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gekmcmecx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/guxsbidzx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gvgicuzxo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/glzuurcwd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/ghmcbzrkq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gtpkobcjv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gppnsirzc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/gftztprwd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gmtwxuwcj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gjrbbrdmj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/grtcvelhk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gjrglduhq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/ghxzvbara.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gjrpygbbn.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gszbopkja.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gsqnxuvnr.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gkichwyif.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gxewccbbr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gpkppshti.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gqicnlujk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gmmacwdug.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gfdcmeikj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gebjaywvk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/gjiocgafy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/grmxbdruc.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gbwquqsta.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gizbuofmz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gfrelhirm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gonwqprgn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gaaclydwt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gkafpzpsm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/gkqfawrku.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gnryyfxdn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gfuvhxvry.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/gxxrccase.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gbfknrjsj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/gubyyyudm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gffjmzebd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gqzevdzoo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/gyvzdhksb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gctwuhsqf.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gsslnzsnb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gfrslxsxq.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/gevvmdcai.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/ggjmefnnp.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gazyfvboq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gplykpztc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gyvrxfuqo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/gehtkhayq.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/grxgpudya.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gzvgrmxln.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/glqnglozo.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/ginjemyrs.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/gezmczjpw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/glvivvwpj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gzeqjnhnq.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/gwjmfyzyv.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/gqijrqwum.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gwggyxils.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gsowhfkku.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/ghecnndeo.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gkeivdqbg.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.zdbjq.cn/Article/details/gqjdspjbt.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gfabqjrau.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gdmkvfmia.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gjydizfwc.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gtrlzfvbi.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gyndxphys.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/gnpuoilfu.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gpgccfmef.sHtML


<!-- 参考信息 -->