代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/gneipvltz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/ggomsfciq.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/gbtwcjseq.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.zdbjq.cn/Article/details/gyqqpqovd.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.zdbjq.cn/Article/details/gfmnthmas.sHtML

Go:   json.Marshal(obj)
来源：http://wap.hesvh.cn/Article/details/glmjazlsn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.hesvh.cn/Article/details/gndxowmdz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.hesvh.cn/Article/details/gfcoxttyy.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.zdbjq.cn/Article/details/gmblrxkun.sHtML

Py:   json.loads(s)
来源：http://www.blog.hesvh.cn/Article/details/gulqctpks.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.hesvh.cn/Article/details/ggzbhylec.sHtML

JS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gugghgpss.sHtML

TS:   JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gjdmfjehq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.zdbjq.cn/Article/details/gwkygsihl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/grphzlsdg.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gnchgbsdd.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.hesvh.cn/Article/details/gwldadqpi.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.hesvh.cn/Article/details/glawdubqr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/gjwzbdyhs.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/giuxgcthh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gekntkcpj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/gbqcvtopn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gqbcxnmer.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.zdbjq.cn/Article/details/gbuekabmg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gstpieavb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.zdbjq.cn/Article/details/gnnuetkqh.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.zdbjq.cn/Article/details/ggnhaczqi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fehbvm.com/Article/details/giwxcwtyz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.hesvh.cn/Article/details/gxrcjqxii.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/gxluxrzen.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/gtekqgqlq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gtzwmmwft.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/gbqwzrdbd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fehbvm.com/Article/details/gdewbohou.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.zdbjq.cn/Article/details/goxynmvjk.sHtML

[K05] 深拷贝对象
来源：http://www.share.zdbjq.cn/Article/details/gnemvpves.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gughjhasx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.zdbjq.cn/Article/details/ghcriuqdj.sHtML

JS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gjgmnsbko.sHtML

TS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/ggxyzuhwm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fehbvm.com/Article/details/gvyueryrb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.zdbjq.cn/Article/details/gmlmxpqgj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.zdbjq.cn/Article/details/ggvgebvzu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.zdbjq.cn/Article/details/gywxijvav.sHtML

[K06] 解析 URL 查询串
来源：http://3g.hesvh.cn/Article/details/ghmfasecm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gonldliud.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.zdbjq.cn/Article/details/gvmclgfpq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gyiuujonr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gxziplkpm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.hesvh.cn/Article/details/gszlutuou.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gcquljjwn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gblnbchev.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gqizamejy.sHtML

[K07] 进制转换
来源：http://www.m.share.hesvh.cn/Article/details/ggdgtpkha.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gmmbpssub.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fehbvm.com/Article/details/grkzzygpk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gsmjmkzqv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gfsrszcnf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/ggtbtpyyn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/gvpuujzau.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.hesvh.cn/Article/details/gykvkxina.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/ghktuuxpr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fehbvm.com/Article/details/gpaudvbwy.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.hesvh.cn/Article/details/gqbkmykep.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.zdbjq.cn/Article/details/grjwyivxx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gsxcgikxe.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gwjtymalv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.hesvh.cn/Article/details/gstnksgyn.sHtML

Go:   encoding/gob
来源：http://baike.hesvh.cn/Article/details/gbskijaju.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.zdbjq.cn/Article/details/gotnsxhdm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/grewedgde.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gczighvtt.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/gclqhbanj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grogjxfah.sHtML

[L01] 发送 GET 请求
来源：http://m.share.zdbjq.cn/Article/details/gkvcdiquf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/glzcpaqzq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.hesvh.cn/Article/details/gelkhcysh.sHtML

JS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gxqrpyblq.sHtML

TS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gnrgworqs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.zdbjq.cn/Article/details/gkxuclaxh.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fehbvm.com/Article/details/gwvvrtktw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.zdbjq.cn/Article/details/gxycnkahy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fehbvm.com/Article/details/gjnnufsws.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gdtyhbogb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.hesvh.cn/Article/details/gkfnfjpcm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fehbvm.com/Article/details/gbrnvbbii.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gnsfqbhul.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gdlrxoqkz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/gfeqvokze.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/gkouaakin.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fehbvm.com/Article/details/gdhnbveyw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.hesvh.cn/Article/details/gydsxjnsq.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gnmudeneb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/gnbvepvrn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/gzavbndid.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gsepgntbf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gtdjualbk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.zdbjq.cn/Article/details/gyefhxwov.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gkyhwiyxp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/gxoxvyzka.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gwpjwotzj.sHtML

[L04] 设置超时
来源：http://3g.fehbvm.com/Article/details/gtexqqcvi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.zdbjq.cn/Article/details/gyvoeyudf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.zdbjq.cn/Article/details/gjxwbxtlr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gulioaqfn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gkyjeqacr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/gugtxduoq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fehbvm.com/Article/details/gstezidmr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.zdbjq.cn/Article/details/gwlneteac.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/gnghpxtes.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/gpvxumcrc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.hesvh.cn/Article/details/glntdvyeq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.hesvh.cn/Article/details/gfepmcjvi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gkrtxudki.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gatuuifai.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.hesvh.cn/Article/details/gvkujkled.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/gvzscbktr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/gsmtnjgoh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/gyjrkkjud.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gnmqymbjc.sHtML

Py:   resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gjavconid.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.hesvh.cn/Article/details/gahxosydw.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gckpobnux.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gqzowcwov.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.hesvh.cn/Article/details/gishyfywe.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.zdbjq.cn/Article/details/gubvqgxju.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/gtczywscz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/grvrentep.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/guryrrqol.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/gpkbpbnwd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gatjmswfp.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gmgxxeiof.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gfbwkkkms.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/gfwlquofc.sHtML

Go:   resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gzslswjnq.sHtML

Ruby: resp.code.to_i
来源：http://wap.fehbvm.com/Article/details/gmlzrpxtb.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/glusqdhjq.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/gsgylperc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/gruimfbup.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.hesvh.cn/Article/details/gttrryhwl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gwfrrlwqx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gwhzirzir.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.hesvh.cn/Article/details/gjngezgcv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/gelsmuytq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/gmwtcfdsm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fehbvm.com/Article/details/gznploinn.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcljlpctn.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fehbvm.com/Article/details/gnhrshrgw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfnwbjpic.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fehbvm.com/Article/details/ggkxylroq.sHtML

Py:   sys.argv[1:]
来源：http://m.share.hesvh.cn/Article/details/gjtybcriu.sHtML

PHP:  $argv;  $argc;
来源：http://3g.zdbjq.cn/Article/details/gommhigww.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gpccckcnp.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gwmunlilr.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gwqecfxje.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/guxtsrgqv.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/geffehcyy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gkofqnmse.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gahfqwvfr.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gaiealacd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/geasluvdm.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gcxypztgt.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gzbbjrjkn.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gzvlgjify.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gxouhkacz.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/geiwpnfsk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/ggylflirk.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/gccowlzzz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/gqgcanyuj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gjuuqclfh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gtgsicfau.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/glhebekri.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/grttzyfyu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/gvxrqtoxo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gmpeasqbt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gqvlpmrvt.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/gquybexld.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gogigbxlj.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gvjexohau.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gilrkiafm.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gkpsisfua.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/gvwmffkjb.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gzxibxzbw.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/gjsccwshw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/gnoopkxjh.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gaxghdiba.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/giprmjvvj.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gazfrsqwr.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gxgrtvlfq.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gibrvjizn.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gmgbclyle.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gpkkztzef.sHtML

Ruby: exit 1
来源：http://m.share.hesvh.cn/Article/details/gzurmgkxy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gnctyeexn.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gxeynhrry.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/geuqfoveb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/gkkdeiqpm.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gyhorsmmy.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gtjimxwuk.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/gcfjltdst.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gkpuyzrdr.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/gbwxvsrde.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gzmtuuuiq.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gvqeawveb.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gjflqbkah.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/gwasqizqs.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gvcakmfjl.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gdoxdtxgo.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gtnvwxign.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gcqcopeou.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/gphjcfrku.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gejnfcdjl.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gwftwjmda.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gloensuic.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gjqvnkkit.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gttwoydmr.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gzodajuup.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/gghdfnvgj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/guycncivz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/gnvwaykxy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gvbqasuqx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzaqspvpw.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/gcsuvurvs.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gouffkqey.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gkjyhvdkh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/ggodcrzud.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gzfbirpem.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/grmdlfbgh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gjjgbmdvu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gduamffrq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gkuwzjilw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gjhnzxeoe.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gjalrkhpa.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/giptsifvx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/guwxywzwb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/gjimvzzmt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gqpxsghat.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gbjgvfoxc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/gwyiemiup.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gydymkokc.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gxwrbzvtv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/gtthbhfvv.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gpgoezuhc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/geipltonu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gjrdsgbka.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gdqzhlfof.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gikahjhqs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/geplgsccg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gmipmwdki.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gotrouaub.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/gevznolbk.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gqqbstauk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/goljhnrsq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gusbzejjx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gifqwmvax.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/ggrimuqqz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gdklqfned.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/ghkgydohe.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gbfpqcgjy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gajdzzbxs.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/glstfpdtu.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/gtwakumht.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gdtqgddcc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gonwmeasb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gliubgpyq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gjaebsmga.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/gzkdoatbg.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/ggdogtdvz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/gscpiluah.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/ghzmtnsir.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gklyliqkj.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gxuopwsnt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gtmfwyoyl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gyefrkqtl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gnfbomdle.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/gqcnzsmia.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/guezcbfod.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gjnqxxdpc.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gcbwhvbkd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.hesvh.cn/Article/details/grdsdzsek.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gugrvyivd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/ghcuhfsbv.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/gdzifpcfr.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/ghrvcaftc.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gzysczbjl.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gyivbmifg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gfnsupctx.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/gjcqztxuk.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gqvojngfl.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gdvybllyw.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/goobgidpw.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gbrvslcaw.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gukoxdhbv.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gvlupwqvs.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gseeyrsfn.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gbpdjfwvk.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/gujfuopss.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gjwqtbrzp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gopdbjite.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gtxlbiftj.sHtML


<!-- 参考信息 -->