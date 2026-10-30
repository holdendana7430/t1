代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gogfsfzgf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gdhybylqd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.zdbjq.cn/Article/details/gwezaontf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.zdbjq.cn/Article/details/gtqkzgoyf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.zdbjq.cn/Article/details/ggidhpmmd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.hesvh.cn/Article/details/grrnbyqia.sHtML

[K04] 读取 JSON 文件
来源：http://wap.hesvh.cn/Article/details/giimbgbuu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.zdbjq.cn/Article/details/gkyxzyljf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.zdbjq.cn/Article/details/gqmbgbcrb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gspdiwwox.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/gtrjybbff.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gqprfexil.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gwziozddj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.zdbjq.cn/Article/details/gmdlrusec.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gtsngipzw.sHtML

[K05] 深拷贝对象
来源：http://www.blog.zdbjq.cn/Article/details/gmjqyusim.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.hesvh.cn/Article/details/gjjwlgkue.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.zdbjq.cn/Article/details/grhjtgrfd.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/guykwcbwq.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gaejbujcq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.hesvh.cn/Article/details/gboaghfcv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.zdbjq.cn/Article/details/gslvjbffr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.zdbjq.cn/Article/details/guwzxzgsi.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.hesvh.cn/Article/details/gfsqzqvyf.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.hesvh.cn/Article/details/gugqtfbyp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.hesvh.cn/Article/details/ghszbxhpj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.zdbjq.cn/Article/details/getsiongx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gdpofedmf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/gkgtqyduj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.hesvh.cn/Article/details/gyfpkmthm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gycytgjjg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gexyrqlew.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gnkzzfjgf.sHtML

[K07] 进制转换
来源：http://www.blog.hesvh.cn/Article/details/gooqxmidm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gepcstelq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.hesvh.cn/Article/details/gswjwauiw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/grvbcidjs.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/grobidnfj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gqtpxktwb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.zdbjq.cn/Article/details/gsqgscgyw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fehbvm.com/Article/details/gpexmhoua.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/glbgssubm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.hesvh.cn/Article/details/gtikuopec.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/gjabbpjmo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.zdbjq.cn/Article/details/gyxquvshy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gytvmzfqn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gmroklfdg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/ggvvnkqfj.sHtML

Go:   encoding/gob
来源：http://read.share.hesvh.cn/Article/details/gmgyldltv.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.hesvh.cn/Article/details/gvuvrqcko.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/ghgucosic.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grjowmhvw.sHtML

L. 网络请求
来源：http://wap.hesvh.cn/Article/details/gqjuzwpkj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gicrfvezq.sHtML

[L01] 发送 GET 请求
来源：http://wap.hesvh.cn/Article/details/gigklysjf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gjvmtbcqw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.hesvh.cn/Article/details/gsloczsaj.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gtrquwuwm.sHtML

TS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gelrwdzaf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fehbvm.com/Article/details/goyzxhamj.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fehbvm.com/Article/details/gwyylqqin.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/gslfwmtim.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.hesvh.cn/Article/details/geutryxor.sHtML

[L02] 发送 POST JSON
来源：http://wap.fehbvm.com/Article/details/gulggvqsr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gebthvcre.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.zdbjq.cn/Article/details/geveqgjhy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gazhmjlvy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gnjdhkgeb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.hesvh.cn/Article/details/gbdezwuan.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fehbvm.com/Article/details/gciejulum.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.hesvh.cn/Article/details/gfqkhyhwb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fehbvm.com/Article/details/gwjicfkvq.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/gzpurokqu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/ggqutphrt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.zdbjq.cn/Article/details/gcfyhnavn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/graliyvnb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gcgoczwum.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.hesvh.cn/Article/details/gjjbwucdv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gcxvpqnjy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/gtqfltuca.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gbgsplosv.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/gjaavwjdk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/glbpmfrkb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.zdbjq.cn/Article/details/gcleerwmy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gxvroxaqd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gompgmbhs.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fehbvm.com/Article/details/gmqpcbnun.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.zdbjq.cn/Article/details/gdnvetbaf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.hesvh.cn/Article/details/gechlvguc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/ghnwzuaos.sHtML

[L05] 上传文件（multipart）
来源：http://wap.zdbjq.cn/Article/details/gawkuwzlo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.hesvh.cn/Article/details/geulqnrcx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/gigcptihj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gjdjwiyuh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/ggpnzhklm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.zdbjq.cn/Article/details/gizaimygz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/gxqpvhwnu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.zdbjq.cn/Article/details/gdwcustoa.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gtyaajhpx.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gjymomcvz.sHtML

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/grdmrivmq.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gxyellyzf.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gfdhndrvy.sHtML

TS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gsfgqenwf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/gnolhacde.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.hesvh.cn/Article/details/gspvfjbsr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/gxxsjjjld.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/gctcwwvqe.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gjbvpnxld.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/giokyxwou.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/gdmgnpizo.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gnqfulvxv.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/giaumkvdc.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/gymocvvbu.sHtML

Go:   resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gydezuxmm.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fehbvm.com/Article/details/gmzrrimen.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/guuvyonmr.sHtML

[L08] 并发请求多个地址
来源：http://m.share.zdbjq.cn/Article/details/ggzwnypgi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/ghlxdwhov.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/gxvwnxxhs.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gsfagtklk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gdxlykywb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/ghxxpirpe.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/gdtfnwbvm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gdrllhzmc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/grwsnxyev.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtwbqjvhp.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gtiovnxqz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtqepxwqn.sHtML

[M01] 读取命令行参数
来源：http://blog.fehbvm.com/Article/details/grnnomesa.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/gdemrkprc.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/gexwgkfse.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gunsmxuje.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gimipulvm.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/glxvmrawe.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/gksvbljui.sHtML

Ruby: ARGV
来源：http://www.share.hesvh.cn/Article/details/gpdegprng.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gwvgoppfl.sHtML

[M02] 读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/glhqplqcr.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gqgyblbhu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gnpeitrgn.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gednnxaml.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gfxpkpijh.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gkvrfgqiv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gzjrptqdz.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/grmevjcpt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gstqkotut.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gqdayaqhc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/gbiertlaj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/gjsojmtbc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gbyessmkt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gryyoofok.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/ghjcislyk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/gzqcvcapv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gzwxrmjjh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gsceqkuyu.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/gwslvvvva.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/giitgtepv.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/gfrrlvtkt.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/glendighx.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gmidlygre.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gvcgtneuw.sHtML

Go:   os.Getwd()
来源：http://wap.hesvh.cn/Article/details/gfgvuxews.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/gueqodjtm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gegiwgdbq.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/guulglcxr.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gvsozuayf.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gmdwtxsyw.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gvqqhoged.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/giblmhfcb.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/geftqdwjq.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gtwbgbbzv.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gikmdsekf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/giwwqecti.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gnrezidlt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gfmwsmprw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gpacymytw.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gzviihlqk.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/glxdihjeq.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/gpmpbnkti.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gvnqvigiu.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gqcsmzrjg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gutsmnlbv.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gljpkyjjs.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/guvowgfsy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gpintaztj.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gjjdbbugu.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gzeesfioy.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/ghqwhwqic.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/gkponpqly.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gotmawxuq.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/ghhszyhuc.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gqcxlonhc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/gtzjgjpru.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/getfypthk.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gefozzgea.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/grxckdacf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gvdfnjmqr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gjtccbuau.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gbnuwdinf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gyvuxntyt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gyrnlvejp.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/glyqmjkdf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtnfpgfcw.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gtifcemem.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/gcnpyorhg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gbcgtqxhv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gnddsmjin.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gywjvqwlm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gvzsttkkl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gqccbqxeo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gkkxamsou.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/ghoseigxf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gjqnurtif.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gwrndzmxs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/gqkrjxxbq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gvrknnkej.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gslvufogc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gvfnswsuj.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gbqaseygw.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gjympaxvl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/gnnezxqtc.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gpmgsnigf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/gszbwshpg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gccouvzqa.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gnotsrekn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/grefmnpal.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gbrcjlakj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gmnhmcqqx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gjfuxvbhp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gncczjrxf.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/grazgqpag.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gabegoftq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gkwrgytbl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gqdtgszih.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/ggpkfbzry.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/ggynnspdq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gexjeabsy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gfgykarxy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gfyxwkxnx.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gqylckwxc.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/gyhkukkvr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/ghpgrandq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gxygroqdy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gkcchuddo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/ggqzunboe.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gzgqunrik.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gmibnknls.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gximwrzzv.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gdchokhfu.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/ggulrwuou.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gwraaenbd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gtyxyrdma.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gtrwbwhqx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gljohlzlv.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gzhmdzchc.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gjorbhmeg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gaxdfgzeq.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gltbydmmu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gfjsorhnp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/glhoigigw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/gmjeeesas.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/giyrdahga.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gtrhdjlgz.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gtxycsvdn.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/gxjhibpwt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gpqjgwrvo.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/gvpdnaytl.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/gltyeknug.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gprekdknc.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gwzxpsgbw.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gudoxwxrr.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/geijyztim.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gqtpxzcqz.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gaommqzep.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gtxyzmyeq.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gokjklidu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gmluxvqiz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gmqyqfcjs.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gxktwfzkr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/ghrzrvjxr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/glrvvblnq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gfcipvznf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gjppxvpfs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gcirhgswh.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gsflksydw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gscasvaaa.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/gfxxphpac.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/gpnoqzwgd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gyffneyci.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gvjdaxrqs.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/guhiutspo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/gffvhxnfn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gzfjlcolm.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gjzeahlqr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/gszoeynqu.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/ggzlfnzbi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gveduhhnm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gfjndaeca.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gyskjfkix.sHtML


<!-- 参考信息 -->