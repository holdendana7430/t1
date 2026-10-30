代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.hesvh.cn/Article/details/gdttbcxfg.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fehbvm.com/Article/details/ggesctagk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.zdbjq.cn/Article/details/glduotalp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.hesvh.cn/Article/details/gjhhuchpq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsurzqlwd.sHtML

K. JSON 与序列化
来源：http://wap.fehbvm.com/Article/details/gbqdmpffg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gejnxlpsr.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.zdbjq.cn/Article/details/gjflwojvp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/gbejnfpcc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/gkscdbqfe.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.zdbjq.cn/Article/details/gnfhaqgsd.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gwifwtsuw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.fehbvm.com/Article/details/gbmatmpdj.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fehbvm.com/Article/details/gfgnqdfpl.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.hesvh.cn/Article/details/gkflkppbs.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gauofjuit.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.zdbjq.cn/Article/details/grzloizag.sHtML

Py:   json.loads(s)
来源：http://www.share.zdbjq.cn/Article/details/gcpvkkjko.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.hesvh.cn/Article/details/gqojsjvwe.sHtML

JS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gcbvgxzok.sHtML

TS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gcvbxwuce.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gpjkstmqp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gngwtazzp.sHtML

Ruby: JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gxwiuarfw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.hesvh.cn/Article/details/gfceekjvd.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.zdbjq.cn/Article/details/gvpjtnvyn.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/gnhpuwgwg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/gfffvravj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gtlahfazj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gvzoafqrm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.hesvh.cn/Article/details/gfzdjwsge.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.zdbjq.cn/Article/details/gnovpfogi.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.hesvh.cn/Article/details/ghufjbgbc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.zdbjq.cn/Article/details/gyzxkvhye.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.fehbvm.com/Article/details/gjeurkair.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.hesvh.cn/Article/details/gpnizjahp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.zdbjq.cn/Article/details/gaioqdvsu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/ghozpifhk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gwjkxsscp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gajvwldmp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/gzuixjfgi.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/gqqetzbza.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fehbvm.com/Article/details/gfpfvjcgo.sHtML

[K05] 深拷贝对象
来源：http://mobile.fehbvm.com/Article/details/gfrxotrgu.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.zdbjq.cn/Article/details/gxdytpgli.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.zdbjq.cn/Article/details/gejdaeqlx.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gjmujsufy.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gvahxoatp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.hesvh.cn/Article/details/glqfwbgrd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.hesvh.cn/Article/details/gzvatoioe.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.hesvh.cn/Article/details/gabeetqsf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.zdbjq.cn/Article/details/grfjijgdo.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.zdbjq.cn/Article/details/gdfhbkmup.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gmmhreaqh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.hesvh.cn/Article/details/gfaottuco.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gedngbsic.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gwdyvyndq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.hesvh.cn/Article/details/gsvohicds.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gkbenphju.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gwyacjohc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/ggrmrriwr.sHtML

[K07] 进制转换
来源：http://www.share.fehbvm.com/Article/details/gajioqoep.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gvrqqmdcu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.hesvh.cn/Article/details/goaroduqd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/geplcbgmw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gisgfeige.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gunjbimts.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.zdbjq.cn/Article/details/gwrccbspb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.zdbjq.cn/Article/details/gyvasdmxp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gtkirqast.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gfdzbumlz.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.hesvh.cn/Article/details/gpogptyzx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.hesvh.cn/Article/details/gtczyvbva.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gxckxrjwt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/guontanlm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.fehbvm.com/Article/details/gxjimvqnj.sHtML

Go:   encoding/gob
来源：http://wap.zdbjq.cn/Article/details/gmwmtsgur.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gzmfistyc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gqfzynclk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gevdtpasp.sHtML

L. 网络请求
来源：http://mobile.zdbjq.cn/Article/details/gqsqgeecc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdgjtqirf.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fehbvm.com/Article/details/gsrfdmesv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.hesvh.cn/Article/details/gndgsmrem.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.hesvh.cn/Article/details/gcphqcxoa.sHtML

JS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gswyqxwrr.sHtML

TS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gmekmerwk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.hesvh.cn/Article/details/gprbidjuk.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.zdbjq.cn/Article/details/gkknkrhlv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/gqprjlzue.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fehbvm.com/Article/details/gbjctlfju.sHtML

[L02] 发送 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gfrmzflhf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.hesvh.cn/Article/details/gkwqcchdn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.zdbjq.cn/Article/details/gdhcsbqur.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gkjfzzjnz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gfejfcdff.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.zdbjq.cn/Article/details/gfjckvivm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.zdbjq.cn/Article/details/gxmjcxlzf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.zdbjq.cn/Article/details/gkwijpkbs.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/guzpacdok.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fehbvm.com/Article/details/grszqjpoa.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.zdbjq.cn/Article/details/gdhmxumnh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fehbvm.com/Article/details/gbbugcesp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/grmfsyfdj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gabjzfvkw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.zdbjq.cn/Article/details/gdsfezqds.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gkokqepnz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.zdbjq.cn/Article/details/gjwhecqxg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gwrmeufmj.sHtML

[L04] 设置超时
来源：http://3g.zdbjq.cn/Article/details/gsfgkghzf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/gndztuvmp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/gzurvhskc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/ggyuvpaxd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gwtfuosqo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/gtfvpwdnc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/gbmwiufaa.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/gjqidudxq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/gxprynrnc.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.hesvh.cn/Article/details/gyfvwoohe.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.zdbjq.cn/Article/details/ghitkokvm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gawfmgboj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/ghtrabzjn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gzwiyolnp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/gvsruozzd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/gunvtxbvy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.hesvh.cn/Article/details/gejdhtvyb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/gagminvqe.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/grykfuhcs.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/gwhozpipi.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/guatxhjmr.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gjalbveya.sHtML

TS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/grydumpap.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gpvieerci.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/gbazhreth.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/gxdhdmwwl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gggkkneth.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gbkrdqxer.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/gojkkduwx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/gxujnrxok.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gnavrenok.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gqkygogqm.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/gwihlrgiv.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gbjfpjbbg.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/grfbwdrut.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gzpltmirp.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/gmrpclwdb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/gtbtlchfv.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fehbvm.com/Article/details/gzqrvisus.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/geoxhlpfw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/ggjscvkbv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gipyrhrdn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/geizjikpm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/grntmxbit.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/geqinpati.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdxgolnhk.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/glljvvwsk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbnngfecd.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/grjlqpmzr.sHtML

Py:   sys.argv[1:]
来源：http://blog.hesvh.cn/Article/details/gpeyksvlu.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/gchiapyqe.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gzunmnvdy.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gkbzewdbm.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gkeplmfuy.sHtML

Go:   os.Args[1:]
来源：http://read.share.fehbvm.com/Article/details/gddkgqhko.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gnidyyfjv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gqqtscynp.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gqcjspnwk.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/gvcystjyj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gqyeigjce.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/glvggjzei.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gjcmwtvup.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gdkpgjqpw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gdnuefkhu.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/gqqwpizru.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.hesvh.cn/Article/details/gjombjqcx.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/goisspcrp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gjnirjmsb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gjbowlmwx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gxedhtpab.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gwbnmjsji.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gjhhcgkdi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/gbztjmfxq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gdjokxqjs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gwgnrebcl.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gtccvdylj.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gxuxclmgp.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/ghzpvvawe.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gfouwhbvv.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gsqrqincr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gmacyzfpa.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gftmcnyyg.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gnbnojprj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gkfehqozy.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/giuamrknq.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/gfadgkbrz.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gsekvjivh.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gclubfdtc.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/geqlhzroz.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/gvecufwoc.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gjjytqler.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gimnfvrnp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gcdebkpqg.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gtjkhatjk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gggkprxgq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/gvidgpvrg.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/grpwrooef.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gugcqgtko.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/gxhxvfwkd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gcjuyvqqq.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gessllvee.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/grdjjzyah.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gctalrsyo.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/gnwrtdras.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gdsrnsqyv.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gkuufjwql.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gdisivasy.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gijrdowst.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/ggslvjcaf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gsrpbfdna.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gfpfzmwpi.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gpzoywtmy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/gswwerjwt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gsudrrfox.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gauclykng.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gsdtegwis.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/guytxdwyj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gxofafdjt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/gdnswylhh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gtugqdsyf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gllgqhkyt.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/giqqsazql.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqsinrwed.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/ggimbauym.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gmjarnpbt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gihjyuuuv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gmnahmtzw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/grmlgicht.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/glrbefgts.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gwdwlgnhq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gfrtvrboq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gjcmachix.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/grtddzgec.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/ghqfortqe.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/ggemdrrlx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gdzefzvmv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gnfyzkxne.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gqwvssiur.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gczwtital.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gdftsplmk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/gmqkrhkwm.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gilrtnsqw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/ggwrewgqk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/gjrmxxgrn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/ggbqhmcvx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gjfryvocg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/gqmmfxzcx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.hesvh.cn/Article/details/goiapcatt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/giycwdpui.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gvvzushoj.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/glcqsnnul.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gsgexcphz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gcdppkomw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gaweqmcwb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gtgbdcqkl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gwiorxhzo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gqltanfyf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gmxglzkkd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gattbpcdy.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/guzqgdlde.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/giyjazeao.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gzmpcyfpq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gorbikvoh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gebjylboj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/ggzbsvfcv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gltdulluk.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gwkxyyajb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/gmamrrtxt.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/griaprqjj.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gsupoyzco.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gaqrelwjr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gidgkoflh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gfogcxxfo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/grfwspnec.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gaiugjpyl.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gnrjzcmej.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gfqltxrma.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/gaqknkini.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/gwpfrhjhe.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gyscislbs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gunhbneck.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fehbvm.com/Article/details/gpnrejltw.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gdikhlyob.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/grfrolvaq.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gslthosuo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/ghijsapwf.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gehzjmpol.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gwtqxbvxp.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/ginmebgiu.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gvmbifwzv.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gyvpzktip.sHtML


<!-- 参考信息 -->