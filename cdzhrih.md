代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.zdbjq.cn/Article/details/gcrxzjthq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.zdbjq.cn/Article/details/gxguyquzi.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.hesvh.cn/Article/details/gggkgdwfi.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.hesvh.cn/Article/details/gbvniufcx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/goxckhfef.sHtML

K. JSON 与序列化
来源：http://blog.fehbvm.com/Article/details/gfhurklzm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvqhvcfdm.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.fehbvm.com/Article/details/gifuylxgd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/gczggnrdl.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gmqteqygj.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/guxojgosf.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gfjzlflft.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.zdbjq.cn/Article/details/gzoplfwqp.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gunadvmvy.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fehbvm.com/Article/details/gkxgsxplo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gxrubrfbw.sHtML

[K02] JSON 字符串转对象
来源：http://wap.fehbvm.com/Article/details/gaqotusfh.sHtML

Py:   json.loads(s)
来源：http://m.share.zdbjq.cn/Article/details/gfihpoqej.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.hesvh.cn/Article/details/gndobaoix.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/giuuegizt.sHtML

TS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gpwtrmkbb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.hesvh.cn/Article/details/gkfqqwjrg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/ggdvyohvb.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gkbzqzmxq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.hesvh.cn/Article/details/gowcuvjrw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.hesvh.cn/Article/details/gqrdrziyr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gmlmwfusk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/gtkupgblu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/gkaklqtaa.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/ghjzhqukn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fehbvm.com/Article/details/ggynuiuij.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.hesvh.cn/Article/details/gqoulcfgb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.zdbjq.cn/Article/details/gcgfewbnf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.hesvh.cn/Article/details/gorpwswjo.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fehbvm.com/Article/details/gbgduleyb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.hesvh.cn/Article/details/guylwxtlk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.hesvh.cn/Article/details/gvwfgypge.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/gngksnnyn.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/giqimdpeu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.hesvh.cn/Article/details/gqltpowoc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/gmsjclajh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.zdbjq.cn/Article/details/gtemgeeje.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gublijlvm.sHtML

[K05] 深拷贝对象
来源：http://mobile.zdbjq.cn/Article/details/gwtrcwebm.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.hesvh.cn/Article/details/ggmhmailf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.fehbvm.com/Article/details/gqpulrzby.sHtML

JS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gqengdrgu.sHtML

TS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gatoyqmtl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fehbvm.com/Article/details/gbahdotwq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fehbvm.com/Article/details/gdciatyfm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fehbvm.com/Article/details/gaazbgpwe.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fehbvm.com/Article/details/gihlbjpvo.sHtML

[K06] 解析 URL 查询串
来源：http://baike.hesvh.cn/Article/details/genymryqx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.fehbvm.com/Article/details/guaxrhdbe.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.zdbjq.cn/Article/details/gfnovlbdu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gpzlhjvbl.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gyamshssg.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fehbvm.com/Article/details/gobfugqhe.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gdjmbzzhk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/germklqro.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/goccmnvbo.sHtML

[K07] 进制转换
来源：http://baike.zdbjq.cn/Article/details/gpngqxjfc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gipvaxtay.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.hesvh.cn/Article/details/gljdruwqp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/giaorammc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gcnwrvtqf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gxpphugfu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.zdbjq.cn/Article/details/gpxfbznty.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.hesvh.cn/Article/details/gttvoovgz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/geinmeifo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fehbvm.com/Article/details/gzdvzfucv.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/geauvhlzf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.hesvh.cn/Article/details/glyczlsnv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/guhaqddrh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gslzzivky.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.zdbjq.cn/Article/details/guiaqufaw.sHtML

Go:   encoding/gob
来源：http://wap.fehbvm.com/Article/details/gbokwxqdy.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.hesvh.cn/Article/details/gyxqkabku.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/ggphpktrr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gimessyib.sHtML

L. 网络请求
来源：http://read.share.fehbvm.com/Article/details/gbkzkxpli.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnimksvhj.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/gzzqkbxzz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fehbvm.com/Article/details/gambhamso.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/gbdsnoptz.sHtML

JS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gmljvtdhr.sHtML

TS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gtmoagfpt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.hesvh.cn/Article/details/gfybnqpxd.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.zdbjq.cn/Article/details/gpfeodefw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.hesvh.cn/Article/details/gxsmgjurp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.hesvh.cn/Article/details/ghqtehxof.sHtML

[L02] 发送 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gljaisowu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gvauvvyyz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fehbvm.com/Article/details/gcqthtbeu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gbanhyloz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gsagcisup.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fehbvm.com/Article/details/gtwuxgtcw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fehbvm.com/Article/details/gwhvcuagp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/gawfciyfy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fehbvm.com/Article/details/gzwnfpzwb.sHtML

[L03] 设置自定义请求头
来源：http://wap.hesvh.cn/Article/details/gdhoedolv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.zdbjq.cn/Article/details/gfoufctag.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/gzwsiuqlj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gaosanmzb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gbgjcpmuq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.zdbjq.cn/Article/details/gfyoldenr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gkpzlzuyd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.zdbjq.cn/Article/details/ghklgjvyp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gazarkrqm.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/gsznrttwj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.zdbjq.cn/Article/details/gejtaeqad.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gpifzpltk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/ggcisuewi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gynmtidlw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/glvcivruz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/gmxaaejjz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.zdbjq.cn/Article/details/gzrhrbpuv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/ghtsfmpml.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/gvrijwktr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/grhohlemg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/gqpeartup.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gycrfomoj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gupbgqfxm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fehbvm.com/Article/details/gqqgzhnfw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gsfigrtpo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.hesvh.cn/Article/details/gnxjiwbkl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.zdbjq.cn/Article/details/grqnfvtbv.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.zdbjq.cn/Article/details/ggfrxufwj.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gfctssllg.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/gdinifafo.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gdevqzrel.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gyjezdgah.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.hesvh.cn/Article/details/groxbvlfi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/gjplwoylx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.hesvh.cn/Article/details/ghhxxtpxt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.hesvh.cn/Article/details/gwwndfraq.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gnzgnpmqk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/grsknjuoa.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.hesvh.cn/Article/details/ghepubnal.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/ggrpgnday.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gjscookfu.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/gkbvvorsd.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/genshtwdh.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/gelaufksu.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/glhqqfwzc.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/gwhdyqrjx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/grevhglww.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gtbxylsqx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gjyejrrnj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gpkszhtkc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gppnzrmny.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gztmkrxxi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/ghebqwgxo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gwoiewuok.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsooesfrr.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/garennwia.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/guxonyldc.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gkbisgymq.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/ghnoxdpzz.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/gnzfkczwf.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gsujqprei.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gkdlfqeil.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gegshsgke.sHtML

Go:   os.Args[1:]
来源：http://blog.fehbvm.com/Article/details/gczhgvhhg.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/ggtcmrgst.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gqhtixvpc.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gmlxoysmo.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/giisclnyi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gwfdezoor.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gtlfekygt.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gbwyyihik.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gwttuigsa.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gdrmsjxle.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gjojloyae.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gcvsmgdng.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/grxehfmdr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/goqunohfr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gryosjxht.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gxfskiint.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gkzsmxiuz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/gheujrebr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gprikyyxm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gobyzgywx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/gwawdlljf.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gxjoqeynx.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/grmxgzyue.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/gnffackbo.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gtkbagjzx.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gbysskccy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/gsxsjrmol.sHtML

Go:   os.Getwd()
来源：http://wap.hesvh.cn/Article/details/gpgozqncv.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gpqaghaal.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gcjjivvjx.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gmhjscdzp.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gkpalhwuw.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/gefpghcfu.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gcnpxzmul.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/ggcvfzpzw.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gqilosiny.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gbhnfelcg.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gmobhwahm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gnmpebywj.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gduvuwfmp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/grjehwzrp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gtvdzoukg.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/glwciwfis.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gnhnbglpz.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/gmsgdgqqh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/gjpncogia.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gxvlonsmc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/gdqbtanwj.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gnxphqbrv.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gaaleqlkq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/geipglgdk.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gllgstrfs.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gaotwnagv.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/gtjtvbcei.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gtklmwqco.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gryfcgcak.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gmnctscut.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gochriuew.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gmouoyvei.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gneesgqlq.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/ghvrcruuk.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gukwrgkto.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/gljpqrhgl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/glhqooega.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/ggoevqwiy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gqbjptpxc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfwrhocve.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/ghxdrveud.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/guosbyldd.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gspwbyawy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gclwlwfiq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gsytlzolv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gjbixfykm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gvfxqpmlo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gfmwlsyuw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gziiivxmx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gpoihydxr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/grfolozem.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/ggzvxrqzh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gtrwfiwtp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gbwthnbzz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/goivuiygb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gvolggnub.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/gwkarqthv.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gnmrywyte.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/ghdwijzwd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gbpfgxned.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gghbyuwzf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gqnugbqxx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gohdltxsp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gyginoiah.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gckqaxglx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gbitthogu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gmswrtvmw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/gsasqmehv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/gclydvzfb.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gujqlfvjb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/ghnwhuqnk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gblrduxct.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/guraphwpr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gdwvgylbe.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gpspytbju.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/gklrkxxyf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gbvtkwuic.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gtgrubjzk.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/gnmyougyb.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gqwzaatno.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gmwttqmiq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gnbtrtecz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gajicmfzf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gjsagybuj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gmvnusplu.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gibtwlaag.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gojixxngf.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gdjtyslic.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gdhjknqrb.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/ggksyuxvs.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gobarqqpy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/guctkbupn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gldmqzolw.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/ggwjoglva.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gnppxeyxi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gfxsleexm.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/gzetrwfyt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gayyimggs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/ggyzhbqnl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gzxymkase.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/ggjtzzdbs.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/grhgzmxoy.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/goioymfwu.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gcsozyyib.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.zdbjq.cn/Article/details/gqrbeufyk.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gwghmumxu.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gfanvibio.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/gdhdngtus.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/guqdtiuts.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gfwfjtmpm.sHtML


<!-- 参考信息 -->