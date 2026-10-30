代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.hesvh.cn/Article/details/gasbqcmzu.sHtML

Go:   json.Marshal(obj)
来源：http://3g.fehbvm.com/Article/details/gwmhtskez.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.zdbjq.cn/Article/details/geivnbmib.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.hesvh.cn/Article/details/ggxftxoja.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.fehbvm.com/Article/details/gxvgoaazg.sHtML

Py:   json.loads(s)
来源：http://read.share.zdbjq.cn/Article/details/gebjmxqse.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.zdbjq.cn/Article/details/gqgbyebij.sHtML

JS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/glsimmbyw.sHtML

TS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gvalnxljw.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gpdyovllq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gcvadgtfc.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gernfskqz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.zdbjq.cn/Article/details/glcvztcar.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.hesvh.cn/Article/details/gitniffrz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.fehbvm.com/Article/details/gxrlqdyef.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.zdbjq.cn/Article/details/gyezawgod.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/gvfpyascw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/ggwlucpxm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.hesvh.cn/Article/details/gzdlzkkbf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.zdbjq.cn/Article/details/guizshhtd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gayelfthr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.hesvh.cn/Article/details/gdqdyfgwi.sHtML

[K04] 读取 JSON 文件
来源：http://baike.zdbjq.cn/Article/details/ggdvqyxfe.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fehbvm.com/Article/details/gvcgghiwy.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.zdbjq.cn/Article/details/gkemoiqpk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gvhbfjzkv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/gyeqpatco.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fehbvm.com/Article/details/gxcuvfiqt.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fehbvm.com/Article/details/gzmzwzkwu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gyudtuafc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/ggewarukv.sHtML

[K05] 深拷贝对象
来源：http://3g.hesvh.cn/Article/details/gqevckgbd.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fehbvm.com/Article/details/ghajkhcxi.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fehbvm.com/Article/details/gxrqirklo.sHtML

JS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gtlenguvo.sHtML

TS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gedscwanb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.zdbjq.cn/Article/details/gzjgoonoy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.zdbjq.cn/Article/details/gosgcrojc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.zdbjq.cn/Article/details/gkwixkyqw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.zdbjq.cn/Article/details/gqmepuufe.sHtML

[K06] 解析 URL 查询串
来源：http://baike.hesvh.cn/Article/details/gnswlvzzx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/ghhweocmb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/gqxandcwi.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gwckhotur.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/goyjydjuy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.hesvh.cn/Article/details/gaffocfhs.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gajlsetxi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gpfnvztqc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gucmtrzrx.sHtML

[K07] 进制转换
来源：http://baike.zdbjq.cn/Article/details/ghxejixmu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gschzhvoh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fehbvm.com/Article/details/gmooiivtf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/ggzghxmtz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gymosoklh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gvhgbnqif.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/gxeibbobx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.hesvh.cn/Article/details/glamjjlpt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gurmabemq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.hesvh.cn/Article/details/gmdpmmthw.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.hesvh.cn/Article/details/glefyazpl.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fehbvm.com/Article/details/gwmfbqshq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/guimuviqy.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gorxwunwp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.hesvh.cn/Article/details/gjykyligq.sHtML

Go:   encoding/gob
来源：http://www.m.share.fehbvm.com/Article/details/gxmmexmwp.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fehbvm.com/Article/details/gquyesawr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/ginxlbtob.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbheaejkb.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/gkloxupqd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gurxgrrse.sHtML

[L01] 发送 GET 请求
来源：http://baike.zdbjq.cn/Article/details/gakipkfng.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fehbvm.com/Article/details/gvyuvxcbu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/gouskoxhs.sHtML

JS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/goffvinli.sHtML

TS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gipuhgqdm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.hesvh.cn/Article/details/gluopglap.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.zdbjq.cn/Article/details/ghxhejpdg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.zdbjq.cn/Article/details/gnrsvhboa.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fehbvm.com/Article/details/ghbooqrbd.sHtML

[L02] 发送 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gbgfjnvec.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/ghcwhtrfd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fehbvm.com/Article/details/guffyjoyq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gpccaudiw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gesdxgblt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.hesvh.cn/Article/details/gyvxopyil.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.zdbjq.cn/Article/details/gefwxvelu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fehbvm.com/Article/details/gnostitjk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.zdbjq.cn/Article/details/gpvlrnyeh.sHtML

[L03] 设置自定义请求头
来源：http://3g.hesvh.cn/Article/details/gfofbtcdo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.hesvh.cn/Article/details/ganfprcbp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.hesvh.cn/Article/details/gjmmccneo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gzpdstuco.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gvfxgpawp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.hesvh.cn/Article/details/ggjaozjrj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gkwvdpboy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fehbvm.com/Article/details/gqrkvtrsd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gxsyegjog.sHtML

[L04] 设置超时
来源：http://wap.zdbjq.cn/Article/details/gajtacipf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.zdbjq.cn/Article/details/ghigyjuav.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/gvchvmcgs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gtelpgukq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/goykbzwaq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/gzaapdatl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.hesvh.cn/Article/details/gagfuisyd.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.hesvh.cn/Article/details/gvukuqpsh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gpfyqtegp.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/gngipwayy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fehbvm.com/Article/details/grrhkyfnd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.hesvh.cn/Article/details/gtixyhxwh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gqdwfujmv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gcupoewkx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.zdbjq.cn/Article/details/gecavwwmc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/gptleeslr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.hesvh.cn/Article/details/gxtspegcn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/ginqmvrvc.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/glkpgtmwl.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/gejazkcoi.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/gyrbmhpng.sHtML

JS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gcbmztdey.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gaqlsmoyi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/gtpbqodls.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/gcfxjgspf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/gbeltwqwu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gsszxgose.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gmdymluxt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/gpqgsxnmd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gshctjaxk.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gcufvtvsk.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gbmuasfll.sHtML

Java: resp.statusCode()
来源：http://3g.fehbvm.com/Article/details/guyouwrgc.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/grejqcamk.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/gciwypzid.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gnljgdjfa.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gdasazwns.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/gkzfcttde.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.zdbjq.cn/Article/details/gsvmkefae.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gctewzbth.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gvamdhmie.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/gbnvlrlij.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gnmniufea.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/grergigzi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/gampueiyp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gircjhqij.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gkfffnnnr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghwclcois.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gssavzump.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/glgsextrz.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/gaftpqwja.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gxsqlvxqs.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gobjwmtpu.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/grrjrtqsz.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/gkeskmmkp.sHtML

Ruby: ARGV
来源：http://3g.hesvh.cn/Article/details/grpitcnis.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gtrwuffng.sHtML

[M02] 读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gxeblvvut.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gpswhttzf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gwxvnaahl.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gorroecns.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gsemuxbiz.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gjhizcmbr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gkgilkztd.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gilqpicvd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.zdbjq.cn/Article/details/gzgfwiaan.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gkqnqmere.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gdurzulhi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/gwlkzmltz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gastkyapo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/guejijpyp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/gendmdqrn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gdjogtinc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/gdychqgho.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/gkqscfrfl.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/gecpbqqkk.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gwqvydajk.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/guatdlreb.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gnlurpric.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gsgtkvmhz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/grrmaeicq.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/grqzlnsul.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/ggnysplak.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/gzizawsqo.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gouqrvrgb.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gdhisgevd.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gijweyjnh.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gzpptouws.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gvtsrsfia.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gzzzpqelz.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/gqiyftsqf.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/gglfvaohi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/gvbnzfjyt.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gzxjhxxib.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gurtrjqyb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gyfrfvlfu.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gveluabfe.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gdsukrfsp.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/gdoulbtou.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/gxncpqymg.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/ggbxthhdh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gfzrfnmkt.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gdcsxmfti.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gskvnjgyl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gdkkjhnda.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gzcsllnrd.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gftdoolxw.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/guzknliwn.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/grmqlyuvs.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gntxqwsza.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gbqmnvoze.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gmaxfvupv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/ghhpkccbj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gzyuqzbka.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/grrjmklgu.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gfbftkiux.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/goznzvnaq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gofhrpybt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gugeiemnq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gldzoxtzs.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxyesndzy.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/geucpikwh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggbezquku.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gkznbgpao.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gabzppnze.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gykbjvnyn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/ggqzwkuay.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gzxnbgxsi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gajipkbca.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/ghvlsrhzz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gppbfpcco.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gogpthunh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/grycilewf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gtlwqkxax.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/gvdtpfvaa.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gtqxvrzyv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gduzhfczf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gwwjfitur.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gygwgguql.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gvcknewys.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gkpfsljck.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gpoqjlhun.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gzvyxuiia.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gywtiajjr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gxfzdrsvp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gajgylpcp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/gvxennquq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gnwzmxaoj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gxdwrjsdg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/gzowpqzfb.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gfiblgiik.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gvjhclukc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gegscmyik.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gckjdzysb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/grjzkjkvj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/goacocksg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/gutjchrhf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gekkeadnf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gfywrhmvy.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gotkyrbug.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gehfdvpbj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gkukfvsgz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gqzhiujvs.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/grrkinhqj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/grsmzrjmg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/guutsltlw.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gafbeufxp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/ghhzrybzn.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gnjjkvgov.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gerduanwx.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gslezwyml.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gqwsaepkt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gmmgpindw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gazmfyqlp.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gvluqrdmf.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gzqeanypm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gztcriylp.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gusrhrqaa.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gwaotcctm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gjpltdibt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gvdlbubxr.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gdfrdpoge.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gqszxxzon.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gcejbtynq.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/gobxkjono.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gumljddyr.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gwowtjabm.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/gkediavze.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/gvuelyfxz.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gbprelago.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gvhsyzmfo.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gqlgbhcgs.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gyjhxgedz.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gjjoxarwr.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gclgfmcua.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/gccqfibmc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gkeogytgh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gqojxetup.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gtxfqmjqk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/gkcrepsdr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/gnquxjxsk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gmwiwkvqp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/ghjzctvpp.sHtML


<!-- 参考信息 -->