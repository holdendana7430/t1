代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.fehbvm.com/Article/details/gxwtpxhoz.sHtML

Go:   json.Marshal(obj)
来源：http://wap.fehbvm.com/Article/details/gogrflnac.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.zdbjq.cn/Article/details/gsmqpwqci.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fehbvm.com/Article/details/gkluwyrua.sHtML

[K02] JSON 字符串转对象
来源：http://baike.hesvh.cn/Article/details/gtslrrfiu.sHtML

Py:   json.loads(s)
来源：http://baike.zdbjq.cn/Article/details/gvnksdxds.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fehbvm.com/Article/details/gdkqxdiyk.sHtML

JS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gaeebkweg.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/giwuxtfko.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.hesvh.cn/Article/details/gnloawgtn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.hesvh.cn/Article/details/gaxtdgwqk.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gmlzdsbsv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.hesvh.cn/Article/details/ginlriwjt.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.zdbjq.cn/Article/details/grwlvosbx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/giubemtdu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fehbvm.com/Article/details/girouhenr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gjlsiepyz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gcqpegvrc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.fehbvm.com/Article/details/giztbslua.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.hesvh.cn/Article/details/gisojbhir.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.zdbjq.cn/Article/details/gjglzqnvx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.hesvh.cn/Article/details/grykjlytt.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fehbvm.com/Article/details/geoyplwch.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.zdbjq.cn/Article/details/gpzfmtfby.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.fehbvm.com/Article/details/gulynagip.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/goqdfjdub.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gcgphbhwp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.hesvh.cn/Article/details/gntucvbcb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.hesvh.cn/Article/details/gcgmkijum.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gxoqgolxh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gdhiryhkz.sHtML

[K05] 深拷贝对象
来源：http://baike.fehbvm.com/Article/details/gklfpmojm.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fehbvm.com/Article/details/gplndwlqq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.zdbjq.cn/Article/details/gvmarizdm.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gilhydoxe.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gqpvyejjo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.hesvh.cn/Article/details/gzrpjtuap.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.zdbjq.cn/Article/details/gubtenlhc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/gqvbgjomz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.fehbvm.com/Article/details/gboauqrdc.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.hesvh.cn/Article/details/gskhxagpq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.zdbjq.cn/Article/details/glkhfzaib.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.hesvh.cn/Article/details/golzpenap.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/giipkskxg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/geshljmnm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fehbvm.com/Article/details/gyujxvfix.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gbzonjspq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gbkkadlhs.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gjypukpgg.sHtML

[K07] 进制转换
来源：http://wap.zdbjq.cn/Article/details/gemxlfiis.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/ggsiwuyzm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fehbvm.com/Article/details/grbkzbwdf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gcigvswhg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gkkfiwnpe.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gvltdfqsq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.hesvh.cn/Article/details/ggbelbhcj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.zdbjq.cn/Article/details/girjrcyxr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fehbvm.com/Article/details/ggfinoocw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fehbvm.com/Article/details/gaopapsii.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/gtejinfqu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.zdbjq.cn/Article/details/gnpjumnob.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gzmaiuqja.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gluszjgqz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.zdbjq.cn/Article/details/gdsqzrcrl.sHtML

Go:   encoding/gob
来源：http://m.share.fehbvm.com/Article/details/gsqwabhbh.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.zdbjq.cn/Article/details/glodkllmh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.hesvh.cn/Article/details/ggpppywxz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grjmvwhth.sHtML

L. 网络请求
来源：http://blog.hesvh.cn/Article/details/gixcoceec.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggorjybge.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/gwpvyxazp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fehbvm.com/Article/details/gfghsssnc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.zdbjq.cn/Article/details/glakyitgo.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gfqpcmeyz.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gtjkqerif.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.zdbjq.cn/Article/details/gurerkakt.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/goyrheuol.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/gnduyhife.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.zdbjq.cn/Article/details/ggxxxhfrb.sHtML

[L02] 发送 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gclktctqt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gwslsomwe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fehbvm.com/Article/details/gekpfykjw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/glfafgsjc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/giqiwzdih.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/gujagzvvt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/gcufesnqa.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.zdbjq.cn/Article/details/gzamoamex.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/gzisaubvz.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fehbvm.com/Article/details/geyhijvuo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.zdbjq.cn/Article/details/geukkkhqr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/gskhmzdte.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gawurfrwr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gfwduuhel.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.zdbjq.cn/Article/details/gmfvdriid.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gjgfrdycz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/ghvisdhnm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/glaxuotne.sHtML

[L04] 设置超时
来源：http://www.m.share.fehbvm.com/Article/details/gscxsfqvk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gpvyynzom.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fehbvm.com/Article/details/gfzahpdwq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/ghtytzoci.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gmcdzveoo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.zdbjq.cn/Article/details/gmreagupo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.zdbjq.cn/Article/details/gqytmoisv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/gqtgwhimc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/garekytub.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/gvyhpptdp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/geacuruqw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/gittatcnq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gubdapesp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gpifknonz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/gkxojeeea.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.hesvh.cn/Article/details/gqvremkyz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/gomscwbof.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/gqcwtsmnv.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/gomyqrrnn.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/gzikqkasn.sHtML

PHP:  json_decode($body, true);
来源：http://wap.hesvh.cn/Article/details/gywgkzkrb.sHtML

JS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gttqossaw.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/giebcceie.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gmhouvndt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/ggbcgjgix.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fehbvm.com/Article/details/gprqmrjha.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/gqqkoerdn.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gvxmdpdhs.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/genbdjdwi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.hesvh.cn/Article/details/getxbngml.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gyntuugvt.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gwkyhcigd.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/gewatkmuf.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/ghmavrswa.sHtML

Ruby: resp.code.to_i
来源：http://wap.fehbvm.com/Article/details/gdavuzbyt.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gckmiesgz.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/gvpikiwnn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/gucbirtlh.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.zdbjq.cn/Article/details/gekofnyrd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gksucagtd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gbywwfhvk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gqfwoabor.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/gkafmusal.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gaykwjyyv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/galnaqkjd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpkyzcizj.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/ghtnfuqha.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvdhwyzhc.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gcwxrtmio.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/gfamxuhii.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/gbkpytdhv.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gliiflmav.sHtML

TS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gfdglpowd.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gutrrwopn.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/gjqgrdryp.sHtML

Ruby: ARGV
来源：http://wap.fehbvm.com/Article/details/gdcyehebu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gsudcmcub.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gpsnejvgj.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gbboayubq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gqsgafwlx.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gvupkhrcv.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gwssumbfj.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gveezreli.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gdhbalbqn.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/gbidpxmre.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/ghxecwtpc.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/gqnqckvzi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/gaxjsznwm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gpclygozi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gwcvkscfz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gjyrvadtd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/gjosesuhg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/ggsnozfbm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gatctbqme.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gqhjdznxn.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gyhpgvhut.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gjojqhtns.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/grpipuwsh.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gxmzywypz.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gxiduoupc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/gqzpfpndn.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gkmylfzwx.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/gnslklmpn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/gnrkviqxk.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/gjokecgzs.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gjyoykpel.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/gtfynhgfm.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gxkjeluzd.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gduihmjeg.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/giuxelcmv.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gyttnzrnz.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/gwxrgngge.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gitylxtvn.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gnnczxhbr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gtxkcikop.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gyyhojdoh.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gbputrkcd.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gklptagqx.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gnbtugxvp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/grvcfcvwy.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gihfufbwa.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gbxkrccyu.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gthipoarg.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gdcrnywxa.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gtnxyzzzj.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/glursbgdc.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gyupyjpap.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gnsfugwab.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/gosniqkcm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gwuqoopvl.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gwotlziut.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/gzynjisli.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gljuihxfu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/guxckdwax.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gmoowchsk.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gaqbhcaxq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gkqcyvsxn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gjuwswtcm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/gaxeyywec.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/giasyhflh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjvddddrt.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/gjvdlxlbn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gltbmjtly.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/ggdlcurbe.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gmpamjtwt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/gasktsnxq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gqgzmqudf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/grfrepiiy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/grzbnmovo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gwdcaxttj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/gptcbpzur.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gohhrdlqv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gnxerdynd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gnrdqvbfr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/gxabmdccl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/grwwoquhl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gtaxcvbat.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gtopsjjty.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gmmmhtphd.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gfbeiapkj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/ggylfbttf.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gbgpwhytc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gglctdkpp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/gupunywvj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gwgxstfcf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/guyghnagp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gdylrhpfk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gyzgtekqc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/gmqoknlpt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gfjrmgrky.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gowtpptys.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gkuqlmprd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gdzkinoeb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gmvyxmdfw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gmxftjarc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gxxqlhvgf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gkemdgzja.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gqrbmxdru.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gorunikkb.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/gurxvveca.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gkouzjugl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gcplkecwa.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/ggbrqgfei.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gpysxorrk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gnckstgjq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/goywrldtd.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gvfacgfpq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.hesvh.cn/Article/details/gzvxrrynu.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gedafhpgs.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/goeyktacd.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gthrzojqj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gcyrfffmy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gnilpbctk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/gwltriflf.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/gnbzraewy.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gatafyprr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gvxvcyifl.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/gkjqblnvo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/grhzmwrmu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/gkhtduiiy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gvqclvwzh.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/gmcwkssja.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/glmtzyokz.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/gwvcchleo.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/gqjnmbmrq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gfueoswaz.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/gyexbssza.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gcxogpwei.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/goplcqbwe.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/goxwuleue.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/goulfprhw.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gzgxlbezw.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gfzaijykr.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/gfrxryquo.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gvddyefyj.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/gykrpwayy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/grbwcbcnr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gxkyrquei.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gzhxuvutc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gmqkomxlp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gqmsayqpe.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gspxzzbvc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/ghdecvxqs.sHtML


<!-- 参考信息 -->