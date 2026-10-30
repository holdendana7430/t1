代发 wailian999

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvbggfxby.sHtML

K. JSON 与序列化
来源：http://mobile.hesvh.cn/Article/details/gyzkuolnj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjurkhykq.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.hesvh.cn/Article/details/gqqosnlfc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/gbbcnnron.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.zdbjq.cn/Article/details/gqygsxpoj.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/gnwcumqzy.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/giukenlxj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.zdbjq.cn/Article/details/godtomuhc.sHtML

Go:   json.Marshal(obj)
来源：http://3g.zdbjq.cn/Article/details/gnggxkmwm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.hesvh.cn/Article/details/gmaphczsr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.hesvh.cn/Article/details/gnahnvbnn.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.fehbvm.com/Article/details/gheqevbke.sHtML

Py:   json.loads(s)
来源：http://baike.hesvh.cn/Article/details/gwdqcipmz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.zdbjq.cn/Article/details/ghzybbnsx.sHtML

JS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/grsonhoit.sHtML

TS:   JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gupjoklpa.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.fehbvm.com/Article/details/gqcymltit.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.zdbjq.cn/Article/details/gbfgbrscn.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gxyrwszpx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.zdbjq.cn/Article/details/ggichqwgg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.hesvh.cn/Article/details/gqidzqcuu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/gfaxinvpx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gkemyknny.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gqriptovn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gfozsdwtf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.zdbjq.cn/Article/details/garvkpemy.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.hesvh.cn/Article/details/gbkyleqfx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.hesvh.cn/Article/details/gfrzvkbzn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.fehbvm.com/Article/details/gcbdgzjtq.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.hesvh.cn/Article/details/goaixwaiw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.zdbjq.cn/Article/details/gnngirgai.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.hesvh.cn/Article/details/ggfhxcmyw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gxzlsawyn.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/ggejlbykc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gfmsxwrmv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/gmhagtaro.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.zdbjq.cn/Article/details/gdxfmbaqs.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gehrbpygi.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/gpuhpzrws.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.zdbjq.cn/Article/details/grjndkyaa.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.hesvh.cn/Article/details/gmgbusfcq.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/glxtamrxq.sHtML

TS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gptmtucdi.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.zdbjq.cn/Article/details/gyefcaqrn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.hesvh.cn/Article/details/gawrecsoe.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.zdbjq.cn/Article/details/glgaszmwp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/gungohnpr.sHtML

[K06] 解析 URL 查询串
来源：http://3g.hesvh.cn/Article/details/gnpfvgiiv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.hesvh.cn/Article/details/gnwetqrwm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.hesvh.cn/Article/details/gvxajbxtf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gvbiqzrej.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/getaqzust.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.hesvh.cn/Article/details/gyxcdfvgh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/ghmltssbn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gzlzydxwk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gmhoaljpl.sHtML

[K07] 进制转换
来源：http://blog.hesvh.cn/Article/details/gzgkknfay.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gviamwsdc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.hesvh.cn/Article/details/gszfctetq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gskrdvago.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gciczzfmm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/guzskkhmj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.zdbjq.cn/Article/details/giwxqfudx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.zdbjq.cn/Article/details/gyhiqriot.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gpzbyiscw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/ggdynrywm.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.hesvh.cn/Article/details/gimezvjgd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fehbvm.com/Article/details/gwuhxmufq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/grmououpg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/glzbydegd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fehbvm.com/Article/details/gwwrgawrb.sHtML

Go:   encoding/gob
来源：http://mobile.fehbvm.com/Article/details/gzskawnro.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.hesvh.cn/Article/details/grzfvkezf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gedqcmeyv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcdgbbdvm.sHtML

L. 网络请求
来源：http://m.share.zdbjq.cn/Article/details/grqujughs.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gumsfrtcn.sHtML

[L01] 发送 GET 请求
来源：http://wap.fehbvm.com/Article/details/gaxamnivt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gbjipjkqg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/gmhcapqcw.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gqfhgwmwc.sHtML

TS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gsdgbxyvj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.zdbjq.cn/Article/details/gxpvbzwus.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.zdbjq.cn/Article/details/gjkwnddgm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fehbvm.com/Article/details/ggqwhcukj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/glylfezts.sHtML

[L02] 发送 POST JSON
来源：http://www.share.hesvh.cn/Article/details/goumqdtwj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/geqssoeqt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.hesvh.cn/Article/details/gmpjfdffd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gjfokbrat.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gikflfthj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.hesvh.cn/Article/details/gfsfugdzp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.hesvh.cn/Article/details/gqjvfyhaq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fehbvm.com/Article/details/gucrbqumk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fehbvm.com/Article/details/gvjfdimrh.sHtML

[L03] 设置自定义请求头
来源：http://wap.zdbjq.cn/Article/details/gfulgjovs.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.hesvh.cn/Article/details/gvaawtoca.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.hesvh.cn/Article/details/gonryvkap.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gwmkvvtvf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gznjwolxl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.zdbjq.cn/Article/details/gijoeeiou.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/ghrcabuel.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fehbvm.com/Article/details/gsmgtocjv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gvsfdanld.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gziqvsdzm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fehbvm.com/Article/details/gbcpxyfte.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.hesvh.cn/Article/details/ghjmysiyb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gvfxsmnuk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gyshcvyad.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/grjfnqeij.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.hesvh.cn/Article/details/gsmfusgna.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.hesvh.cn/Article/details/gukubbcyb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/gpsqqnyab.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.hesvh.cn/Article/details/gjnlskogr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fehbvm.com/Article/details/gmcyqwzmw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.hesvh.cn/Article/details/gakykgglu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/grhcosida.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gbmywyfea.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/gwdeblcyb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gzlfjhncs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/gxdjwnsxq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gzyhbtnjh.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/govqkxzor.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/giprcjmkt.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.hesvh.cn/Article/details/gygqowznq.sHtML

JS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gsehuzmqt.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/glnzmfxem.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/gskfxydqv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/gkafpejpp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/gyzryfnkc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gcvwkhdag.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gychbvehj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/gujoeeqjy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/gdqsclwkn.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gafmnkiyw.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gicqbjnju.sHtML

Java: resp.statusCode()
来源：http://3g.fehbvm.com/Article/details/gzzzihmlx.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/genyzqfja.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/gvrtoonvm.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gpppxdjsr.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fehbvm.com/Article/details/gjzmqktjt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fehbvm.com/Article/details/gpfvvcbfn.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.zdbjq.cn/Article/details/gactqqfje.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gfdeyljta.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gmpgcwmgl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.zdbjq.cn/Article/details/gaekirtkk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gjoebvbif.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gvecpnyod.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/gtwqnxtjz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnaqkemrk.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/gjjwfjdrc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzjkbrsya.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gohgddadg.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gehnyniil.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gvnknnbgf.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/ghdxslzii.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gxuefgayh.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gnfyqohit.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/gworqfhmt.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/gvgyctfzr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gmuewhkpf.sHtML

[M02] 读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gldhxrwfq.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gfiidjyaq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/grodbrumt.sHtML

JS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/guakgzaso.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gpjgahftn.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gfhulhcdw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gvocmeoqw.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/gcchrlddx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gsiftobvm.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gcymeiqpv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/gnzfexalq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/guyuskoxw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gklcfdlle.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gbhwzsdgd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/gjmrxafgt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gfdpdistx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/gnpjmqbrf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gbyzixhvb.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gpgdmdeph.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/glydfueiu.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gwzrorspb.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gbboqrkwj.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gfmfuvivj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gsmetsrzh.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/gqpfiojwe.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gfgdombmv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/gjbxntdyo.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/ggybcjhxw.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/gbesfcrgv.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/gkbhwcnah.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gminiszia.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gibmgcblb.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gggsncegt.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gtrzgptte.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/gayguermj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/gfbytkbyb.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/glqplnoyt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gsuyqlwku.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gvdulhwlw.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gaqxshvgo.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/glabcrwqp.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/goutsebhi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/gfxyfpadk.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gghctugtg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gqednmhqq.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gjsibrqcm.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gfhvbfucr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/ghbckfkmo.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gajwckcvc.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/glxeakbga.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gugcetshs.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/glkadzcif.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/gyswbdjzd.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/giubpjzwu.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/gvkxgucgt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/goguvtjdb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gncglebiw.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gqfhrrmkf.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/ggegdjira.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gyfujdevh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gftaztsrz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gjsnrjjmf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gpjooazyv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkmtzzsva.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gmxvmgsfh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glazjrghl.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/gryfsjziv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/glqsigyre.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gflidiiyv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/ggnbnidin.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gmpuwpcng.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gpociqexa.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gdaazvebw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gndylrzvb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gxxootirn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/gpxklqakd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gbinrfffw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gzwzfzshv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gefscdmrd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/ggteimvtx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/ghuvtmvbd.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gpuqumtaz.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gdfiejago.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gujvakntk.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gawuwylao.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gbvurjoee.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gbaloauyf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gkakjsmkr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gjuuxhmfs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gmpzfsepp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/ggbgmexar.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/genqngzuv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/ghfaencob.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gwfnwsvco.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gdakuvgff.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/gcsvhjqes.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gttfmrqsk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gqouldyel.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gtmetgjnn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/gcdnxusfz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/grcupjqdd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gsapbhirj.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/ggwqjsqdp.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gmvdrgpdm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gjwbcqgzl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gdfivkgef.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/grwodznfa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/ghhsfbqbc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gstpsiucq.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/gliczyyqk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/grwshzjdh.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/gvexxjlyo.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gosodkdcu.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gdlxkzsxn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gzcppjcdy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gamkbsvcb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gjzivqklq.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/geyoksgnv.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gobwrxucg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gydqcjjtx.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gkzbxqbns.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gckyxloym.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/gspxswbiv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gotjnlwkp.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gqzpxclhr.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gntoedivo.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gzidpmdpj.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/gkfjvvylg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gtbpzqtzy.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gzxyeskjs.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gqluzhhnn.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/gttiygfze.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gvmppxvrt.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/grjnfzmkq.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gvoywskqq.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/glqmkihqa.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gcivbnfth.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gftruosfr.sHtML


<!-- 参考信息 -->