代发 wailian999

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gycnlucdl.sHtML

K. JSON 与序列化
来源：http://read.share.hesvh.cn/Article/details/gkdwydqiy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjmwjyiqf.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.hesvh.cn/Article/details/gfszibrvq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.hesvh.cn/Article/details/giymamcmp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/gjmgllnnm.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gnrvrzsnu.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.hesvh.cn/Article/details/gllvkdkwg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.zdbjq.cn/Article/details/gofbvvgok.sHtML

Go:   json.Marshal(obj)
来源：http://blog.zdbjq.cn/Article/details/ggdptuhkg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.fehbvm.com/Article/details/gdivwobob.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.hesvh.cn/Article/details/gnpdavcvc.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.zdbjq.cn/Article/details/gzryzjcur.sHtML

Py:   json.loads(s)
来源：http://www.share.zdbjq.cn/Article/details/ghrxuhetv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.zdbjq.cn/Article/details/gfwyssgkr.sHtML

JS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gunvhhasg.sHtML

TS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/grikztrql.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.hesvh.cn/Article/details/gtdhbbklw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.hesvh.cn/Article/details/gonwtdckg.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gtmjoyaor.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.hesvh.cn/Article/details/gepphnazc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.hesvh.cn/Article/details/golsdczuz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gooiszuda.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/gelscrulf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/glgrkxtrw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gxmbrbybj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.zdbjq.cn/Article/details/gpuvjrrir.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fehbvm.com/Article/details/gwvbhopcs.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.hesvh.cn/Article/details/gziebmivg.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fehbvm.com/Article/details/gvxgybhfz.sHtML

[K04] 读取 JSON 文件
来源：http://wap.zdbjq.cn/Article/details/gbawvszwa.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.hesvh.cn/Article/details/gvgdevklg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.hesvh.cn/Article/details/geibiphen.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gnvcelcqg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/gsxuodyea.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fehbvm.com/Article/details/guybilqec.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/gpxlnzvif.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.hesvh.cn/Article/details/giqruqskn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.hesvh.cn/Article/details/gprgiqdop.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/gfhouirlb.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gotufhbhl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.hesvh.cn/Article/details/gcdrghvvc.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gpklitqwk.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gtzlpyvit.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.zdbjq.cn/Article/details/gpokkkyjl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.hesvh.cn/Article/details/gxzdhtbry.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.hesvh.cn/Article/details/gevkqhvkg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/gisuznurj.sHtML

[K06] 解析 URL 查询串
来源：http://wap.hesvh.cn/Article/details/gqjbufutx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gysqccsic.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.zdbjq.cn/Article/details/gzumjuhjf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gqkdudrcp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/ghukiqrin.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.hesvh.cn/Article/details/gxuivoeuw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/ghfuyfuao.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gewxgsofe.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gazfrudxu.sHtML

[K07] 进制转换
来源：http://mobile.zdbjq.cn/Article/details/ggmnthyka.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gernsskbf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.fehbvm.com/Article/details/gwjlgcubt.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gonrhlduq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gxgbornak.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gjfkyoxdt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/gzzrjltzo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/gzbidhaew.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/ggnjfkrya.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.zdbjq.cn/Article/details/gqrqpfjij.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.zdbjq.cn/Article/details/gizsnqicd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fehbvm.com/Article/details/gcsvtbxmw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gtqvuohef.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gfpqboroh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.zdbjq.cn/Article/details/gmvrhrsow.sHtML

Go:   encoding/gob
来源：http://mobile.zdbjq.cn/Article/details/gzoalbcpw.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gnaqsfloe.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gujzswepn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzhcutnhu.sHtML

L. 网络请求
来源：http://baike.hesvh.cn/Article/details/gobcarkoy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdlzrleak.sHtML

[L01] 发送 GET 请求
来源：http://wap.hesvh.cn/Article/details/gwbrpkdpm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.hesvh.cn/Article/details/gowfphzef.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.zdbjq.cn/Article/details/gpgsftbna.sHtML

JS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/grfsdimle.sHtML

TS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/ghyglocnc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/gngwdmzij.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fehbvm.com/Article/details/gnipkjkuv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.hesvh.cn/Article/details/gppoozlgx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/glxlyyfsz.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gcfxvpknj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fehbvm.com/Article/details/gqqzydryp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.zdbjq.cn/Article/details/glbaeiaii.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gmusjjysr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gbgadzmqz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.zdbjq.cn/Article/details/gzupcfzpb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.zdbjq.cn/Article/details/gpuzufvgk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/gmdhwaiwb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gvxqocvgu.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/gmmpdghfq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.zdbjq.cn/Article/details/gzqrfidhb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/gxnnevhqo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gnrfrwapl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gmbdcnjfb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.zdbjq.cn/Article/details/gdrtlxcgz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gwxromhuh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.zdbjq.cn/Article/details/ghhcexird.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gxkdmjlva.sHtML

[L04] 设置超时
来源：http://www.m.share.hesvh.cn/Article/details/gtodhywxy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gbitedbyo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/gvqskeimw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gyzhuvqlg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gtnnnztxf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fehbvm.com/Article/details/gtfxfrkrx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fehbvm.com/Article/details/gqsrxwyds.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.zdbjq.cn/Article/details/gofbarpir.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gkfjhhhpw.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/gfsogekpr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.hesvh.cn/Article/details/ggyyneqpm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/gbgtmamti.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gwnofmajh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gdkuxyhen.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/gwmkqycvi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gizrwidxh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.hesvh.cn/Article/details/gugvqadjk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.hesvh.cn/Article/details/gbowefrwu.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/guvxpcxkd.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gqrszsdqu.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/gaisjzvva.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gboszamqv.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gyjzwykjk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/ghsojozek.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.zdbjq.cn/Article/details/gkqkjgiwd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fehbvm.com/Article/details/geglvutls.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/grltuniwy.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gxlzmejsz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.zdbjq.cn/Article/details/gzbfsrxzi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gfvxlaicx.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gortlygss.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gxmqbhivb.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/gxuomfsfr.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gkuuxhmvr.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/gkxaeoumk.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gshbxbynf.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/gisvmwkmg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/gsiycahuu.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/guemqlpoz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gqyoplqmj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gwaeujhhh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/gijxlvkok.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/gpqvwbyfv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gdeqirrcc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.hesvh.cn/Article/details/gdecpazmn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/govfddgfg.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/gohejswxy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtawkjoie.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gibapyave.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/gcwugnbpd.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/glblqtcis.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gbfmbafxs.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gxnotphix.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gqbzuhnww.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gijayfkpp.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/gtzdrgtlf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gkiibwimi.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gokxfhllk.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gpobyxeij.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gquypdiyr.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gcpldzhsf.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gaeogwbwr.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gsdxiroxp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gxoplaqaj.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/guscujayf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gorrahyhf.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/geunuoacf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/gbmqijucn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/gjbeuuntd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gcsxltyuv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gbbgfehwb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gvxfboyyc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fehbvm.com/Article/details/ghbopzsil.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/gyppufgnm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/gpgbyrzow.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/ghowmiqtv.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/ggrriwyrk.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/gczmlrcap.sHtML

JS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gkahtaoqy.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/grkvqmkmk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/gdrpsngxk.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gvajwrxrz.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gbikmerst.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gijhmvfww.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/gesygummr.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/gbcrqqfdn.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gxzuzjzih.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gvbeclxcx.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gobjmbdnh.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/gklcrtebp.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/gzcsknzue.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gcqvpsouu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/grusijzli.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gubgjfvoo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gofxzbqzp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gdtbrbijr.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gfwlsagkj.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gtqvyxmgu.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/gmropurad.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gdxynqtnv.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gobqweubp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/gsiuzgami.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gxiokwqyi.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gxayuqmkd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gawiptpmk.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gqamdqznx.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gtlkqfphe.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/gbltjhpnz.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gthiarllo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/ghjsnaemz.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/ggjzrbozr.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/gmfdejppi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/gqmxdtqhz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gquhidyrn.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gjlctlong.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gzjkaruum.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/gdqzsnrww.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/ghxidjbga.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.hesvh.cn/Article/details/ginljcpvz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/griletbxb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbqqevwgj.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gropzmbmn.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfqjhafiv.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gmxnqzrtt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gnfclbgdq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/gsowrbjnh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gwonxnuoi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gluqnbptf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gyilzjyxi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gjiftltxl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gmnyjmubf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gnkjozrlc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gkoggdjbv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gyuazdeiy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/grjdwdtmk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gqrxxydzr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gpiwnrwjl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gzctknmal.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gxhegzfjn.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gmnplbtld.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/grfyrjzds.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gghluiczx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gjladepkn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gthjotsvw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gfvyyhocf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gykpsubib.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/gtlklncst.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gjwbwcivm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/gndoyyccj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/guwspwsdf.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gqfnjjjls.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gtlmzbhhw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gdsolgavg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gptssaikp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gheaixvlp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnojifaki.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gjslmrfcu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gtlsazjjc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gmxvicvlj.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gznqkueyw.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gjzmanozy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gnhnhxmxf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gaglonzgd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gzruvkavu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/grqbzxajs.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gtyytfwap.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/gxkihpoum.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gjviehaib.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gawiuzbuo.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gqngdjtnc.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gnlblbmlh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gvbsmnzkh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gfrblojar.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gmapnetui.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gjoxeytps.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/gobnkimsb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gangxjcbe.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gswxsttnc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gvpohynhg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/gozjmrszq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gvtuywlnb.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/gyenfsmoh.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/gynmsmgur.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gylpinmek.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/ghbtvzmge.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/gndrqwbnw.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gkdewnpar.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/gjxvaldqg.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gjgqruljz.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gtznmdlgo.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/geeeziueo.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gdqbwmylv.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gwalhunuv.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gfwsabvbm.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gbokxgktg.sHtML


<!-- 参考信息 -->