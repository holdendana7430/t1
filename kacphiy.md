代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gchnxhvko.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gpklfnyrv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gkjernxay.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.hesvh.cn/Article/details/gpiihvlqb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.fehbvm.com/Article/details/glkkcrjlx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.zdbjq.cn/Article/details/gjrtaoyfq.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.hesvh.cn/Article/details/genefsjex.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.zdbjq.cn/Article/details/girwphzdi.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.hesvh.cn/Article/details/gqhqllqqv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/gnvgqybxj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/gpxghdxsr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fehbvm.com/Article/details/geepruomn.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gszfmfsxi.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gndilnflw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fehbvm.com/Article/details/gdkcasyro.sHtML

[K05] 深拷贝对象
来源：http://wap.hesvh.cn/Article/details/gpuyiuzei.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.hesvh.cn/Article/details/gwnzefurp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fehbvm.com/Article/details/gfbfgctmy.sHtML

JS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gybzvolek.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/ggwnuuaql.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.hesvh.cn/Article/details/gyemsmtpk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.hesvh.cn/Article/details/gvcltoehf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/gyzwlvtnk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.zdbjq.cn/Article/details/gaegyheni.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fehbvm.com/Article/details/grnfrsmhb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/galosykrp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.zdbjq.cn/Article/details/gwvkkzjui.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gsxmwkjnn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gbkltagyt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.hesvh.cn/Article/details/gtefbzljj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gyeslooci.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gwfpsxack.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gudajoqws.sHtML

[K07] 进制转换
来源：http://wap.fehbvm.com/Article/details/gurmqqwfd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/ghjqrbceo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fehbvm.com/Article/details/gmjwmxgkd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gatmuasqw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gwfmglrji.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gpichialz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fehbvm.com/Article/details/gfygwdkcr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.zdbjq.cn/Article/details/ghaupenur.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gojmuzhus.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fehbvm.com/Article/details/gfwzyoidt.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.hesvh.cn/Article/details/goderznuk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.zdbjq.cn/Article/details/gyduwtdgy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gttcqiuym.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/ghexjzpsf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fehbvm.com/Article/details/gqaulujne.sHtML

Go:   encoding/gob
来源：http://www.m.share.hesvh.cn/Article/details/gotrxwlbo.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.hesvh.cn/Article/details/gfpjzbspo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/ghhwjbdyx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gywniipbn.sHtML

L. 网络请求
来源：http://m.share.fehbvm.com/Article/details/grgxolqdm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghnomrndy.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/gavvltvci.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.zdbjq.cn/Article/details/gdrlfzfhw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/gnuarxews.sHtML

JS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gkotlumzz.sHtML

TS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gwxfnbadu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.zdbjq.cn/Article/details/gipvstncc.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fehbvm.com/Article/details/gfcvmvtfe.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.hesvh.cn/Article/details/gqtbssdxg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/giyidhape.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/grskpwlmb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.hesvh.cn/Article/details/gilkbqskm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.zdbjq.cn/Article/details/gqgsakioc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gnmauqaib.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gincitiux.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.zdbjq.cn/Article/details/gkqggrvdm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fehbvm.com/Article/details/gqjuawhhu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/ghxjnkaly.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fehbvm.com/Article/details/gshpuhxyg.sHtML

[L03] 设置自定义请求头
来源：http://baike.fehbvm.com/Article/details/gahyleboe.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fehbvm.com/Article/details/gnymsggdv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fehbvm.com/Article/details/ggjtkttma.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/glzkftvbw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gvurtcqsp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fehbvm.com/Article/details/gsaatzqmc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gmpbqpwqo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/gbwlgyufk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/ggmomxjsy.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gqrpogubw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/gnhdsqnni.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.zdbjq.cn/Article/details/gyjsfgshx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gvpkazdnj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gcvcgwppj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/gecoxfvsa.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.hesvh.cn/Article/details/glrplwgit.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/giurhriau.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/ggljzgqjh.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/ghzyrilpr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/ghwptkyns.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.hesvh.cn/Article/details/grxfkrkfi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gjmkcgqoc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/genrckmsj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/gtgklzcll.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.hesvh.cn/Article/details/gekozyfoa.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gqedtuzjk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/grvkdhwst.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/giwgcyrvx.sHtML

Py:   resp.json()
来源：http://mobile.fehbvm.com/Article/details/ggvjqcsvp.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fehbvm.com/Article/details/grjrrfonx.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gypcgdctl.sHtML

TS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gyxsijrth.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fehbvm.com/Article/details/gvuvscjuv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.hesvh.cn/Article/details/gjtcnbefw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.hesvh.cn/Article/details/gwfkregng.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/geldiexjf.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gwyrutcop.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/gsyilmbyi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/gcvbibysm.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gzbywmyhx.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gtjqyfetz.sHtML

Java: resp.statusCode()
来源：http://blog.hesvh.cn/Article/details/gmlmgvoaw.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gtuhpftiu.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/gokcvpbpr.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/guwukhqvy.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/gbyulmkjr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/glbvmmjez.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/ghuatcbau.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gqfkhlyhh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/giekjzikx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gthzxszen.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/gcnyztkvp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/gmgicnchc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/ghnajobui.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmdeghhhz.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/gtrdrbnjq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvyawgvtk.sHtML

[M01] 读取命令行参数
来源：http://mobile.hesvh.cn/Article/details/gvtbeslui.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/gxetutpqk.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gfnrkkloa.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gvkymtura.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gmevrdqsa.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gyepdetog.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gtyexlags.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/gxvuucnfv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gsudusvce.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/galevcppw.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gzmczgitr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/geuuaduag.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/guuyspgae.sHtML

TS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/ghkicmrfw.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gqzjmiout.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/goetxdgte.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gjcgbglxg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gawznlwoj.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/glxlnwvul.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gikqplnwk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/ggbvdrbzj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gbyetwxlg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gomyjbilu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gtbrkbmke.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gcvyqesen.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gmgyqnawn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gmxnoizbg.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gyarmqqgd.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gmsircwov.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gyqskbork.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gfxoafhbt.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gtgulbydc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/grcmkyrjl.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gsrwbhnnu.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/gvvxhfsao.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gayogumqb.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gzmrqsest.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gzgvfuzhj.sHtML

PHP:  exit(1);
来源：http://mobile.fehbvm.com/Article/details/gjhmujmzf.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gcjlfnwoj.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gnodisjrl.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gcefernxi.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gzphkwrhb.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/gzhpweusv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/gytsthjup.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/goeycptvd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gxxbbtfvk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gfwgnbopw.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gxhzumbwt.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/giovxhqhs.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gucakwohe.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gqyitrtqz.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/ghhgxsqzb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gravufbjd.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gmwniexpi.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/grzxmhdvz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gmmtdrfqm.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gjijvnguf.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gljvmajuf.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gbutkooxp.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gcsuplqkq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/gccrqylgr.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gbpabzcne.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gzegeymkw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/grkymlfpm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gcelcqiwq.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gisqkwkdd.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gesqgkmxg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/ggakpzslg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/gumzjpyuh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gkmwctkrh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gjphykagc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gikghitby.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gaymdogtl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvuvexynd.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/ghazgvebu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/gqorukiot.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/gzxjkudcp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gqtsocvgi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/girbwbcqh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gyqoslyus.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gakntmwfb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gntvmijpg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gdwxaberr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gxhfaslcj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gzegsbirg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gxgksotet.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gggdiavgm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/ggcszeoau.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gmnhmvadx.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/guqazzepk.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gfsbhaaln.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gqglkjbrn.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/ghumyoydl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gezrioczr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/grpqahfge.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gvdubpxin.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gmdsudnhp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/gbkqsbhhw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gitnoxday.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/ggpdbzflc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/gzzdknykz.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/guedvbcyj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gtqxmktpt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gflemcwgz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gwglhcjcn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gvuwxwjzd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gacmrbmom.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/gopoqdpws.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gpjtayets.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gozgwnotv.sHtML

[N05] 最大公约数
来源：http://www.share.hesvh.cn/Article/details/gllmdclcd.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gefztjuwf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gntoghues.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gcjdxirfi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gtlaoeewr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gbjnsxype.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gqmppkkdr.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/gdamxedws.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gboudvpbw.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gxrcirkew.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gyzwcbjoz.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gqefgbfvc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gsxbbtprf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gvhudxlod.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/ghtbrwfyu.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gdkcnnusd.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gopsvskbz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gwqujbqzk.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/ganujrpfk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gaotmxtxw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/gfmkjjslg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/geocbacim.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/galroytzy.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gdiqwagdr.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/gkjkvcket.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/gldtjfwke.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gptnxtmjg.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gxshiwswa.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/grrcavavl.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gbmaadwrb.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gdmtsvgpy.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gihpkrnpa.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gcbvyuqdx.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gemqqmvev.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gbbysqpgl.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/glcgvekqo.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gmwfqdmei.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/gywcoztoi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gbgujcsiq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gtirqcpsy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gaqstpusp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gigjptheg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/giqigdmgf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gopluklhl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gdyldelhy.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gutfjtobv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gifgvyhvr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gqtedbipe.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/gswciclbg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/gqotvavlw.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/giivqcboe.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/giqzgrtve.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gphyrthwf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gdsrukund.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gwuiauupt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/gmxeeayah.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gyrrqowus.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gjotliipt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gxdfkojss.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gpqszjukw.sHtML


<!-- 参考信息 -->