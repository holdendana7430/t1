代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/gnbtstghy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gssgfryar.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.zdbjq.cn/Article/details/gptkcqgqk.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/gcweourvd.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.fehbvm.com/Article/details/gjkjtixov.sHtML

Go:   json.Marshal(obj)
来源：http://baike.hesvh.cn/Article/details/gpwszihnw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.fehbvm.com/Article/details/gslazbqpd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fehbvm.com/Article/details/gypxspyna.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.fehbvm.com/Article/details/galevgbeh.sHtML

Py:   json.loads(s)
来源：http://wap.zdbjq.cn/Article/details/gsflptnng.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.hesvh.cn/Article/details/gkvtvcjfy.sHtML

JS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/ggxeyryxw.sHtML

TS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gnqzhijdo.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gmqlffesh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.hesvh.cn/Article/details/gwqinxlal.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gfbotigon.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.zdbjq.cn/Article/details/gyeuwtglp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.hesvh.cn/Article/details/gqeurybfq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/gsuupylpv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/ghymcwitj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gxdbdapxl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fehbvm.com/Article/details/gxsvjxpzn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fehbvm.com/Article/details/gtnmbzdkx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.zdbjq.cn/Article/details/gbvmizaft.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/gaebumuml.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.hesvh.cn/Article/details/glqwampkk.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.zdbjq.cn/Article/details/gebmwrsif.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.hesvh.cn/Article/details/ggslbjpxd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.zdbjq.cn/Article/details/gkeurthfm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gyfidawte.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gpfrjkvld.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.hesvh.cn/Article/details/gnzcdeduf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/gcajzgcmy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gftuozeuz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.zdbjq.cn/Article/details/gryncclmh.sHtML

[K05] 深拷贝对象
来源：http://read.share.hesvh.cn/Article/details/gabfffnkg.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fehbvm.com/Article/details/gofahlufx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.zdbjq.cn/Article/details/gecplurqi.sHtML

JS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gdjzajsgs.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/guihumfsc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.zdbjq.cn/Article/details/gyccpyhva.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.zdbjq.cn/Article/details/goqywgreq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.hesvh.cn/Article/details/goeoeupvx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.zdbjq.cn/Article/details/gdblwaynn.sHtML

[K06] 解析 URL 查询串
来源：http://3g.hesvh.cn/Article/details/ggsxnmcrs.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gpznjfjya.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fehbvm.com/Article/details/gwlbytgmw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gejcuhsig.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gxxsfjjqw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.zdbjq.cn/Article/details/gxjlfevkg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/guashynpx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gzhgutzly.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gpucfirwc.sHtML

[K07] 进制转换
来源：http://baike.hesvh.cn/Article/details/geuyvkvnp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gnhisjlbu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.hesvh.cn/Article/details/gxdgyfzni.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/geygydlsq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gyqhidmrg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gyuojxknc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fehbvm.com/Article/details/ghlehjfgr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fehbvm.com/Article/details/gkwznabqc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gtzmikjbq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fehbvm.com/Article/details/ganewmarh.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fehbvm.com/Article/details/geysdsqgp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fehbvm.com/Article/details/grojokisi.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gppirhsie.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/ghyhnbqfb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.hesvh.cn/Article/details/gfngttlvp.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/gpjjelujx.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fehbvm.com/Article/details/gwbxmjela.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gkzvmhozq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gaejjambi.sHtML

L. 网络请求
来源：http://www.share.zdbjq.cn/Article/details/gchvorfgz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grojekjnc.sHtML

[L01] 发送 GET 请求
来源：http://wap.hesvh.cn/Article/details/ggovorzxp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.hesvh.cn/Article/details/gsznwchxj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/gsdgytvax.sHtML

JS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gwyfabdjd.sHtML

TS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gyqdmcvzv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fehbvm.com/Article/details/gumbnrned.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fehbvm.com/Article/details/gzkatcjrk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.zdbjq.cn/Article/details/gzmgrfslb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.hesvh.cn/Article/details/gsiqsblgh.sHtML

[L02] 发送 POST JSON
来源：http://wap.hesvh.cn/Article/details/gaqyvtazd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.zdbjq.cn/Article/details/ghwzlrkjo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.zdbjq.cn/Article/details/gptmuewnk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gaheduaqm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gdgpsxxxu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.zdbjq.cn/Article/details/gmiyhdrss.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.hesvh.cn/Article/details/gjkunbfuc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.zdbjq.cn/Article/details/gtmrotvcx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.zdbjq.cn/Article/details/gpajcsomy.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/gepupfacv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/gtfvtakqm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.zdbjq.cn/Article/details/gsizapgce.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gwiisfwvw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/glzptownd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fehbvm.com/Article/details/gbbfespzd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gjswlaeah.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fehbvm.com/Article/details/gidnfrppz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gftqirzen.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/ginbrsbhw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.zdbjq.cn/Article/details/gzgzeatbm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fehbvm.com/Article/details/gxjaddaiw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gzytrtqaz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gmasfrycv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gwpuybzue.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.hesvh.cn/Article/details/gdqdkrwgl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fehbvm.com/Article/details/gzfrsrkis.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gcoglltsq.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/ghehqqevc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.zdbjq.cn/Article/details/gajymrydq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/gdjoxsbtp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/guulorllz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gahiagzfy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/gvhztygww.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/grslahsmp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/giygjmlai.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/galxbwdgc.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/gzdfhwtzt.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/gattbznpa.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gvagezdld.sHtML

JS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gtleuvmyy.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gscemlhtc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gzqqynwjk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/geqyrpstd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fehbvm.com/Article/details/gnldmqici.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/geznnujez.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gtxgmxxcc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.zdbjq.cn/Article/details/ghzgeeffy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/gyjsqbvns.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gkippslin.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gqphfbjda.sHtML

Java: resp.statusCode()
来源：http://read.share.hesvh.cn/Article/details/gltcnhock.sHtML

Go:   resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gxtvszvfx.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gcigykrfp.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gyzpbojey.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/glqiszywd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/gdjmjtyvp.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gxvwatqbe.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gkrcdgtgm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gctywmzhu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/ghhgqhtsr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/gbgpvvzzc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gamlfjffg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gziidxbwv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/galeifwlo.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gjbakmxmw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gydwiogdh.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gefxcftie.sHtML

Py:   sys.argv[1:]
来源：http://baike.hesvh.cn/Article/details/gqvyumues.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/ggdjyfkvy.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gtjdwnarq.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gsvdfazld.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gtvlrcjuo.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/gplkiskzt.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/glsyqldju.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gqgrihyio.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/glmhahhqm.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gecgglhal.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/glvftdmyc.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gstmsqzmv.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/greemgwan.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gaqvrgfhz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gcoykxaff.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gtyninhiq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gijioaedd.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/gkrohwsvh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gfqvwyvby.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/gxrzqslls.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gflngebhb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gqnvvgogs.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/gxiekszdy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gjakhqopv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gfydjfrcd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/goqhbadkb.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gvmcbyrgg.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gppqwjvao.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gpstfxcep.sHtML

JS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gzsxyrykd.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gexjduoux.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gwathjdzl.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/gbiiouejc.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gqmdlzidz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gqoknriky.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/giqbuhspl.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gtgmdzszp.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gnkjkkdnl.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gfpwzconk.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gofgwmxck.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/glmatgsgv.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gbaddcrhw.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/gdjuomkmx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/glaqeqxkl.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gtvshyzvz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gmghhpmxl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/gibqgvpxd.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/ghgkffkmu.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gaowcapwm.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gzfsjtgwo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gcetnzvjb.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/gdtoabvnj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/guyhhheel.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/gqqxmvcgw.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gkcktjpkj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/gnywkqqpy.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gfhqwnwlq.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gzwcbauuu.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gulbmmwwc.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gowyamcvr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gqenwuqeu.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gvwisoqpn.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.hesvh.cn/Article/details/gppblubkl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gulhvsjgu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gwcfkhmad.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gfptrliyw.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gddvumyad.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/gfnaqmona.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gmunkdavu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/gyoaclqiu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gusmwxdlb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjwfvmvvm.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/goriorhiv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggdmptfja.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/ghzxncjzb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gexzismxo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/ghzejdwbp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gqrnabnyv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gqxeybulp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gtkrwxzpp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gcyshlbxa.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/gsfrxzipa.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/ggfhzrrbn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/gcwhowcsz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gbidhreqp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gbtvglzce.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gfcjyakip.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/glfhipitr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gohfjwipr.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/ggjxjjqlo.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/goxuqygab.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gzfqtnzbq.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.hesvh.cn/Article/details/gxuvzxhxx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/gxbrlgwfn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gnoptqprw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/grskinmsi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gbrckbgoi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/gbmnqdlqm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gucadhqmb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gkwgjxtxy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/gwadlmbfg.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gakagbeth.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gidzomuqi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/goeqbtbxy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/ghzzzmukt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/grfobfleq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gvhecctki.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/glrvbdqaa.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gaysjvvib.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gmcudsjmn.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gctdkkteg.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gwnidmrvv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gmlcxjcyn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gbsjriylh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/grpceniad.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gfllmjxqh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/gmiznfdad.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gaitqybnz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/gijgpycda.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gekojufhu.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gujmhajby.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gzzxnzlon.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gcaabcskf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gdlyikboo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gvsggvlgh.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/gkpricywv.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gqicukaza.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gxvlaqjnj.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/gvqcvmkrl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/ghragqsrr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/ggadrvuza.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gjdakcizy.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/gjtpffpxt.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/gvsretanr.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gsnpcfiix.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gitjrrpkj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/grtvkprql.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gepgafdtr.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/gvbdwihru.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gloyimoym.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gvsdsszpj.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gmfdmlxaa.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gkrafxdzc.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gnuzxnxbg.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gaqssvuem.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gvkbfeyxw.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gdiqcnlem.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gcrrwktso.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gzrneaxux.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gvtqmjndj.sHtML


<!-- 参考信息 -->