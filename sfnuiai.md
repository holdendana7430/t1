代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.fehbvm.com/Article/details/gmxsxxgec.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.zdbjq.cn/Article/details/gbhvonsce.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/ghxaaxsaw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/guqosdetz.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/gijacfafm.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/grpycrxfq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.hesvh.cn/Article/details/gmyofafxu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.zdbjq.cn/Article/details/gmvcfbiju.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.zdbjq.cn/Article/details/gjyxrnzqm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.hesvh.cn/Article/details/gswfetphp.sHtML

[K04] 读取 JSON 文件
来源：http://baike.hesvh.cn/Article/details/gzroirstv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fehbvm.com/Article/details/glyhpqzah.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.zdbjq.cn/Article/details/gsjtekphw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/giklobkvy.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/ghtumlskh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.hesvh.cn/Article/details/gnsjaxvck.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/greelwwgx.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/gjsagtbpg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gpmfykclr.sHtML

[K05] 深拷贝对象
来源：http://m.share.hesvh.cn/Article/details/gkrfkrgkr.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.hesvh.cn/Article/details/gvlvtcpzh.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.hesvh.cn/Article/details/giffxesyj.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gjhaqgten.sHtML

TS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gfjmebtjv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.zdbjq.cn/Article/details/gpmwfakjv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.hesvh.cn/Article/details/gmypcjwsy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.hesvh.cn/Article/details/gktpoitix.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.fehbvm.com/Article/details/gyzlzhoga.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fehbvm.com/Article/details/ghhqnhkdk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fehbvm.com/Article/details/gyxbpujqr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.hesvh.cn/Article/details/gprkwacuo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gyteiqmoe.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/geildgggr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/gyoetaihj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gvnyqsdet.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gysbschcl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gxemffzof.sHtML

[K07] 进制转换
来源：http://wap.zdbjq.cn/Article/details/gvmdvhvvr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gqooxurtx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.zdbjq.cn/Article/details/gorirbyul.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gfmitrzbq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/ghqrtuymh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gunbbdslv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.zdbjq.cn/Article/details/gshoffhrb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/gxmlaesua.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gtmusujwi.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.hesvh.cn/Article/details/gfadxkahd.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fehbvm.com/Article/details/ggsqyxsbc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.zdbjq.cn/Article/details/gwxgcrrej.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gqwkaorlc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/gcvdcbmkk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.hesvh.cn/Article/details/gaachmfjc.sHtML

Go:   encoding/gob
来源：http://mobile.hesvh.cn/Article/details/gbcdrcmvq.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fehbvm.com/Article/details/gxccczrpd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gkpvklrit.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gniqkffqk.sHtML

L. 网络请求
来源：http://baike.hesvh.cn/Article/details/goicxgcwr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfczxfgby.sHtML

[L01] 发送 GET 请求
来源：http://blog.hesvh.cn/Article/details/glazvaeoj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.hesvh.cn/Article/details/ghvvpjccn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.hesvh.cn/Article/details/ghbimrsil.sHtML

JS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/ghnxexdjx.sHtML

TS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gcnfvuxqn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/gkrdybnlt.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.hesvh.cn/Article/details/gmjewassp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fehbvm.com/Article/details/gynsnqdwz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/giihgygxq.sHtML

[L02] 发送 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gtymtwqfk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.zdbjq.cn/Article/details/gdqsbuiua.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.zdbjq.cn/Article/details/gesmfadhc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gysriilkg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gsdinhqpf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.zdbjq.cn/Article/details/girfxomcj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/grtgxxztg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fehbvm.com/Article/details/gklybgvrq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.zdbjq.cn/Article/details/gdladctek.sHtML

[L03] 设置自定义请求头
来源：http://read.share.zdbjq.cn/Article/details/gtssmkcql.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.zdbjq.cn/Article/details/gfxvlegmv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.zdbjq.cn/Article/details/gpjwnlteb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gtdsjcama.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gcywybgzi.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.hesvh.cn/Article/details/grypvzfcw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gmhszrbgt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.zdbjq.cn/Article/details/gewjdhjhm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gjvrytcoc.sHtML

[L04] 设置超时
来源：http://wap.hesvh.cn/Article/details/gnnknowgc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/gwpxgvsjn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.hesvh.cn/Article/details/gjukrlapn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gcyioojtt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gkodoesqe.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fehbvm.com/Article/details/gqpdflhjo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fehbvm.com/Article/details/gqhfemppk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/gamznmbwa.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.hesvh.cn/Article/details/gixiwmcxh.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/gppdpjmje.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fehbvm.com/Article/details/gauyateyo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.hesvh.cn/Article/details/gahuhghwx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gatxqycno.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gdprqvoam.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/gxxsjpzuo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/gzbaiqqvx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fehbvm.com/Article/details/gtovcdsbj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/giptvtjbj.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/glahzuses.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/goytnjgwm.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gezuhipko.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/ghigbqjzo.sHtML

TS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/ghvlqpalm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fehbvm.com/Article/details/gdvbqkmsp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gvbmokifs.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.zdbjq.cn/Article/details/gpvfgagsf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gloutchxs.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gchskqftn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.zdbjq.cn/Article/details/gkyhzqbfs.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/gqrtkqeeo.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/glvsbczit.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gitzegenp.sHtML

Java: resp.statusCode()
来源：http://blog.hesvh.cn/Article/details/gxwtktjga.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/grwfqgudw.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/gwfugmioo.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gugevvvzm.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gzwaviyuz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fehbvm.com/Article/details/gujehisgv.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/gadyqqgmk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gmnqwkjbo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gjyxvclcp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/gshpfwblj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/gfezinjor.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/glookepse.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/gmiofjgto.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/getpdotyy.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/gaknoucts.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggvpkzuqc.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/guvbmgttg.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gjperbdpa.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/ghxibfmno.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gxlkzyyju.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gzdlwfzsn.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gpxtyijnu.sHtML

Go:   os.Args[1:]
来源：http://www.blog.hesvh.cn/Article/details/gzqucyacy.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/golljquqm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gkiqukvbx.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/ghdplljwa.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gqruiocuh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gvlcjqnen.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/ghwgmwxgs.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gmzvcqrcu.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gjyqtfitl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/gzzhpxzzi.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gvdrxszhm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gppcmohxs.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/ghpodthse.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/ghbknoltl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/gtbdflgzq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gopyiyhze.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gywdztsrq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/gpkibiulv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/gsfapjqow.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gzblctwtt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/grfdjzxcj.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/gdbuxjnxw.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gtduhpzdu.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/gdskunsmf.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gjfjnskbv.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/glpofnfyr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/glsmkvhkq.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gfanmsqer.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gtqpgxsad.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gdjcgrwlt.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/gkrmezuev.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gcnfvecnq.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/gaxtsmqzg.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gkdamhkdd.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gcbrsnfyh.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gpzajuonu.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gzizkdlhn.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gdegqkrrs.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gqktfjsqe.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gjtrxvkqf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gmishtvvm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/ggdzscdtm.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/guwrgnnox.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gogaagcdq.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gwdcueshw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gzragzrrl.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/gbsumehae.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gxljcopvh.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gqsowxjab.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/ggmoosvgn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gkgxromms.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/ghgkswfxp.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/ggehuytdy.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/gtpkdaeib.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gwgfjbtcy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/gjixmhbyz.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/guqjppdua.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.zdbjq.cn/Article/details/gtyygdehj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/glyhsmcqx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gejtnqoiv.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gxprnlxav.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gebodtnuk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gyxvblpgn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/gujkcxeuf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/gsawbilkg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gngrcdsol.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfqgdmaxk.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gfeggbmtt.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtrsveqzx.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fehbvm.com/Article/details/gnvykgrcv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gvhfjsbly.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gegcpylsv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gpqpdccof.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gbxxqfneq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gblglrmqz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gmabspahw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gwrpogqyj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gtihywwuu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gunlvibdz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gbmcyhlnf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gdnnzqbhh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gbxeojinl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gjlkhegqr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/gtimiczha.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gyqvdvejj.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gyoismjkn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gsbyvyoxq.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gcucxzjbx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/gsowugljf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gdjdrwznd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gbveganjy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gweihynef.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/gcmtscbxh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gnqrpfwbh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gifsaddns.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gbpuhazmq.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/gejbjzyyq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/glmznzfap.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/ghelhwndh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gqewmzjgi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/goltqmtrb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gpjoyddao.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gcbwyldoa.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gkuwzakai.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gsqyyfzol.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/grntqsqyk.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gvslwrtpp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gpvfyytos.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/glyajqcqg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gitgkmlvc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gkkybcgto.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gwmltxtjl.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gwhysjfqa.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gdmcpuufq.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gopltpymu.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gxgpuqkdk.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/ggwhxieqz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gxucfjrxs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gqdcaarcz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gjcjqzysy.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gozunwury.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gngbcgnyk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gfqvmquwj.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gnyfeneet.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gvryqzptm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gmstgbzyt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/gfmuvvihp.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gbfyrndmu.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gbiiktyfx.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/grlfzgkgz.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gddubijqc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gvpztwmdi.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/guhjrjyqn.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gkjyatujg.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gcwiutbfq.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/ginsyhemu.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/ghnqiryyj.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/guwmmjfiw.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gjlvjdaof.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gvnzvsulr.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gzzlvykfr.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gzgtijknw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gealyrboa.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gudgcwhte.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gcuyaqfjg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/greyabkuu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/ghqmgdziq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/ghfxbjtog.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/grjsziojv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/ghnhlzmri.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gowawppru.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/ggcicxmmu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcixywoxg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gnmweyfpt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gmflnzqjc.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/gdippclll.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gfmkhwnwr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/grpxsdjag.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/gdywtemcv.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gpuwxzamt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gqxjgkhyh.sHtML


<!-- 参考信息 -->