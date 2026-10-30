代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.zdbjq.cn/Article/details/gzaqmneed.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.hesvh.cn/Article/details/gdhectqdd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.zdbjq.cn/Article/details/gjwtxvfip.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.hesvh.cn/Article/details/gojnejcpd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkwsoyddd.sHtML

K. JSON 与序列化
来源：http://www.blog.zdbjq.cn/Article/details/grupnioqm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdljpzbpo.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.hesvh.cn/Article/details/gmswnildy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/gxsnxhxqx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.zdbjq.cn/Article/details/gfnbypjws.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/gpdvozsnf.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/gajozxjzb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.fehbvm.com/Article/details/gqjeryeqi.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.zdbjq.cn/Article/details/gwfxqspqx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.hesvh.cn/Article/details/glkecgthh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.hesvh.cn/Article/details/glqhdhwre.sHtML

[K02] JSON 字符串转对象
来源：http://baike.hesvh.cn/Article/details/glejdnuqy.sHtML

Py:   json.loads(s)
来源：http://3g.hesvh.cn/Article/details/gkrxhutwj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.hesvh.cn/Article/details/gcyuxcphv.sHtML

JS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gkfgaklhe.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gtnbfctwp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gvxezztso.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gsikfdjgx.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gnluxskjt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.hesvh.cn/Article/details/glwedjthh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.zdbjq.cn/Article/details/gkrqizvum.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/gmwdvlrjl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/gnxczxxjd.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/gutwlxfez.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/gmpvixiyy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gryxoduse.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.zdbjq.cn/Article/details/gjexytqnn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.hesvh.cn/Article/details/gehvpizkq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.zdbjq.cn/Article/details/ghurbjrse.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.hesvh.cn/Article/details/geqendpxm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.hesvh.cn/Article/details/gxvrvxclc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.hesvh.cn/Article/details/gchxvcfop.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/ggavkxisu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/gimjjtelg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fehbvm.com/Article/details/gomtfvjrf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gtqiugpzj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gdebqxsew.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gwohnobrc.sHtML

[K05] 深拷贝对象
来源：http://3g.zdbjq.cn/Article/details/gpnbjygle.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.zdbjq.cn/Article/details/gviudkqkp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.zdbjq.cn/Article/details/grxckmiwv.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gysafgesd.sHtML

TS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gohdtkesa.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.zdbjq.cn/Article/details/ggnxzzinf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.zdbjq.cn/Article/details/gbcaxsthl.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gvdtpezgu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.zdbjq.cn/Article/details/glyemvfjz.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.hesvh.cn/Article/details/gughzuduz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fehbvm.com/Article/details/grjugtwut.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.zdbjq.cn/Article/details/gqwwwmeja.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gyzscylvc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gefgmyvtb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.zdbjq.cn/Article/details/gfzvlaopl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gpiovkqiy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gamoimfka.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gkxqykhhk.sHtML

[K07] 进制转换
来源：http://mobile.zdbjq.cn/Article/details/ggpfjpnfh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gloymyrwe.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.hesvh.cn/Article/details/gmhuvkeny.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gschbezcy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gsrpucwdb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gzzynpbka.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.zdbjq.cn/Article/details/gidmaqroh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.zdbjq.cn/Article/details/groebmiev.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gyvrgylbf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.zdbjq.cn/Article/details/ggmhuojun.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.hesvh.cn/Article/details/gqfostpyh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.hesvh.cn/Article/details/giajypjnw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/grouzqohr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gxceceeay.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.zdbjq.cn/Article/details/ggpgxlevh.sHtML

Go:   encoding/gob
来源：http://wap.fehbvm.com/Article/details/gwqygfuwz.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.zdbjq.cn/Article/details/grozszlkl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/guiutiape.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gegxlwiim.sHtML

L. 网络请求
来源：http://www.blog.zdbjq.cn/Article/details/gwfvrfdnl.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnsxiabkk.sHtML

[L01] 发送 GET 请求
来源：http://blog.hesvh.cn/Article/details/gskzlpryf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.hesvh.cn/Article/details/glhazgptk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fehbvm.com/Article/details/gpdhqwwze.sHtML

JS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/giiekaipn.sHtML

TS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gmnwrsnfq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/grvxwerdh.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/gwzrdxjpz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fehbvm.com/Article/details/gweeqcdml.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/grdbdjojb.sHtML

[L02] 发送 POST JSON
来源：http://blog.hesvh.cn/Article/details/gjrqdpeom.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fehbvm.com/Article/details/glzqkxdqw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/gqckborsb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gcyrtmfvm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gdwivkbxf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fehbvm.com/Article/details/gtvkymuvi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fehbvm.com/Article/details/gzjywatps.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/giorrjwrz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.hesvh.cn/Article/details/gerlghkjh.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/gbwhcqufh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/gqjzysfvq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fehbvm.com/Article/details/gxnjezqhx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/ghqztaxde.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gwxgmqciq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fehbvm.com/Article/details/gmycbyipr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gmywvprmk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.zdbjq.cn/Article/details/gdeibhauz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gftjozbdi.sHtML

[L04] 设置超时
来源：http://read.share.zdbjq.cn/Article/details/gtnfapilt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.hesvh.cn/Article/details/gjkrgwbbj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/grvukgwwt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gafnoddzt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gwdnbwpvi.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fehbvm.com/Article/details/gynjdbewp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/gpuhnshyp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.zdbjq.cn/Article/details/gzzhnrsbj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/gmjythmky.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/ggggwlsnc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gswwqnkxw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/gxpkhpaup.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gdftzyiyv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/ghedzuigq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fehbvm.com/Article/details/gnmukotmm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gnwzzrrfo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gqrgjnqih.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fehbvm.com/Article/details/gsgvthbrd.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fehbvm.com/Article/details/gqxzikcnm.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/gczqzzmix.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/glkkikyve.sHtML

JS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/ginnkkpts.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/giexgtcby.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gmhdcnhlg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fehbvm.com/Article/details/gezhkgehd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.hesvh.cn/Article/details/gsmcxlvqy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/ggaxhoymz.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/glsitbkex.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/grtvpcahi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/goyqrgkzm.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gqlvdypvz.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gzatyizji.sHtML

Java: resp.statusCode()
来源：http://m.share.fehbvm.com/Article/details/grshcxkbo.sHtML

Go:   resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gjizwvhmq.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/gbnfcwtqu.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gppqavopc.sHtML

[L08] 并发请求多个地址
来源：http://3g.fehbvm.com/Article/details/gpkwuxfcj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/gbvhgnnrg.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fehbvm.com/Article/details/gdhopiojh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/ggxowgqgp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gkpgsgywj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/guiuhyqjl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gymfrchgz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/gddlhdgnr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.hesvh.cn/Article/details/gheyaopzh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gihewvozg.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gljvfsvwt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxgbyphkh.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/gnicjcxjt.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/ggrcbjamo.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/giveojybv.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gacrsumwc.sHtML

TS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/ghtawroxp.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gtvzbuyin.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/gpacadzwk.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gebvqjtvn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/glcdidxju.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gnzebywvg.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gmptawktn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gfovcooio.sHtML

JS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/giptrcvln.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gjagwkrus.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gnoqtfcfr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gkzeumdox.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/gjldjibpo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gwvgtejqy.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/ggrzbbmtn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/ghgobyqmy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/glxxuefsu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gxhhjmull.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gqarmrzbj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gjubkkjku.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/gefhjuyco.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gkrgobgjp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gnoeflrvi.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gemjyuxbz.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gouavhqap.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gcdzflsbr.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/goifxzivl.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gfmolxpdt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/gwkydqcni.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gjubrwynh.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/ghmgkoscm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/gnqrpwjrt.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/ggehiiaya.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gpxvcfezm.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/ghgmuaylo.sHtML

JS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/ggwbajchr.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/ghusltgkt.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gzolkukgz.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gmrffbgpt.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/gtxlfstwu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/garsczbfx.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gsvyhkdfa.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gjohemuyi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gpmczyrcj.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gotqldbuv.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gmdxsntgm.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/genlqphyr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gzuemilva.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gnccisnxy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gasbplluv.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gialyejlg.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gddjhmhna.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gtdqelzbs.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/guoelehzo.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gsrmquymx.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/ghcrmtnjt.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gnfsxbjvt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gymqfdlip.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gixuxpsxk.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gdrxpaxdd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/gkrmbvmqf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/gpdatoxry.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gmclwcamv.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gnlvhqplx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gkkrsryzy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/gvkmirsaq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/glweuwbkz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gwhdyvhco.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glsojlmfn.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gpndbytty.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmenustby.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gmwhrezxs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gdieerhgx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gslhaaqhi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gykjbmxhz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gnkwvmjtl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gwnqqqvqd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gscutjnwn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/gauhpsjad.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/ggxkgawpx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gxjkpvjvm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gvkezqrfj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gpawyhdfk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/ghvldvexu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gsaomwtqi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/gazmsqiks.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gaowwfamo.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gtcfkqvfk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/gqdfxqmie.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gsmjtmcyk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gjrvtaibh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gaipxfsfv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gevmcncmb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gqlaxuqdi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gmpnbdupq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/gjxvrghzg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gnkszmerl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gtukteaxz.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gdzngmyvy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gdzzseivd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/geympoxhi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gygsczgrs.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gjlwgvfjn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/ghfjgqtoy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gjqhlprlf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/ggrvrbxfe.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gyqxspspn.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gszstcrpo.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gtoykdkdi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/govillfvc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/ghfmmacah.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gvrogjqwn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/gnjfjctgr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/gkhpiudiz.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gofzlpygj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/gwsawdtzx.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gthtdcwfy.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gvpprfbcn.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gsfhbinry.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gklrreaqb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gsmazuzxn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gyrcjnfwi.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gjanfbszz.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gdibnbcip.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/ghymwbeas.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/grtdjgomt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gyezshofk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/ggbqblrjo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gyzixislf.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gveczmpqr.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/ggvsxzqou.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/gkympfhqs.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/gpokzeuly.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/guhfcemtm.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/grbbaitly.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gqltztxbs.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gpigsyxyz.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gwogjnybu.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gihvqlwpy.sHtML


<!-- 参考信息 -->