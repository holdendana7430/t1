代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.zdbjq.cn/Article/details/glmcuofng.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.zdbjq.cn/Article/details/gjiwezkzi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/gxqoggzkf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.zdbjq.cn/Article/details/getyhefqn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gcadelfxn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gwrttvvzi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.zdbjq.cn/Article/details/gxehbtnif.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.fehbvm.com/Article/details/gfpsawmbk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.hesvh.cn/Article/details/gmcvdsmsp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.hesvh.cn/Article/details/gjbrcqzli.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fehbvm.com/Article/details/gagxurpqo.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.zdbjq.cn/Article/details/gquvsxsiv.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.hesvh.cn/Article/details/garjlivhp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/gjvhbqnbc.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gkyqdwpzn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gdxpublvb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/ggfvhsosp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.hesvh.cn/Article/details/givtcmejc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.hesvh.cn/Article/details/gcxkjuyah.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/gxbjhzmpv.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.zdbjq.cn/Article/details/gyxbjzgdq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.zdbjq.cn/Article/details/goejnwxlr.sHtML

JS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/guozfzlyg.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gdqpgwqke.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.zdbjq.cn/Article/details/gpwzzqvvo.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.zdbjq.cn/Article/details/gavdlinnn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/ghmovvoct.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.hesvh.cn/Article/details/gkutuvjfq.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.hesvh.cn/Article/details/gxzyregkw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.hesvh.cn/Article/details/glsvxzfgy.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.hesvh.cn/Article/details/gyccysghn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/glnrelmes.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/gvjmfnekh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.hesvh.cn/Article/details/giidvkfjj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/ghtrnkyvk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gxvicskeh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gayypibek.sHtML

[K07] 进制转换
来源：http://www.m.share.hesvh.cn/Article/details/gzsebewpz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gafibjwsh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fehbvm.com/Article/details/gccceqoea.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gexnwdlyk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/ghlynjjew.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/guroiafcp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fehbvm.com/Article/details/gnaszjnsk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/gcdqfvelu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gpjrrioms.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.hesvh.cn/Article/details/ggrqwohxv.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.zdbjq.cn/Article/details/gukcvvzln.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.hesvh.cn/Article/details/gblprldxm.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gaslsqryu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gvdvjpyek.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.zdbjq.cn/Article/details/gegnihrnz.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/grvpxdhes.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.zdbjq.cn/Article/details/gxuervjfl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gfzwcnaen.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gihhvxtku.sHtML

L. 网络请求
来源：http://read.share.hesvh.cn/Article/details/gqtaxluqb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmypbigmo.sHtML

[L01] 发送 GET 请求
来源：http://m.share.zdbjq.cn/Article/details/gyfszsxkq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.zdbjq.cn/Article/details/gkmbswulx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/glyclrbfi.sHtML

JS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gvqckdvzq.sHtML

TS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gfmqjjbld.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.hesvh.cn/Article/details/gsafiplff.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/ggjjchfax.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.zdbjq.cn/Article/details/gbyzcsriz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.zdbjq.cn/Article/details/gzbywdfnc.sHtML

[L02] 发送 POST JSON
来源：http://wap.fehbvm.com/Article/details/gjyzaiajc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gzkcjsczq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/gkctrhzmk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gtreyctxi.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/grgagswwl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.zdbjq.cn/Article/details/gcvjiwhor.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.zdbjq.cn/Article/details/gfagppujs.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.hesvh.cn/Article/details/gtwsxsyjt.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.hesvh.cn/Article/details/gjitvyodb.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/gqvkgasll.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/gdacobsbe.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/gfwktfhta.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gjefktfrq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gljazirea.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fehbvm.com/Article/details/gozxlopht.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gkqsdlfhj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/gfxszcklq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gxnieibru.sHtML

[L04] 设置超时
来源：http://wap.hesvh.cn/Article/details/gnpbhjyxz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.zdbjq.cn/Article/details/gdrhafqjw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.hesvh.cn/Article/details/gewhqwxzd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gdagozwmr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/greulgyhi.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gmaitnbfq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fehbvm.com/Article/details/gsnhibzbb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/gjzbwwrhs.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.zdbjq.cn/Article/details/gkcuigkln.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fehbvm.com/Article/details/gxhipdxha.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.hesvh.cn/Article/details/gcyhfizdm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gsqwdhccx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gkliceecn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gsapfhgfe.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fehbvm.com/Article/details/gdwvkgopc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/gwmwjofwb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/glwsyhfqc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.hesvh.cn/Article/details/gekbnicfo.sHtML

[L06] 解析响应为 JSON
来源：http://baike.hesvh.cn/Article/details/gvwojuemf.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/gaxsipdwn.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gnxnwbhdm.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gqkgzvugb.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/glimtplhh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gvwrymxum.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/gpxdafwqt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.zdbjq.cn/Article/details/gqdntxnmi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/gvatzwgrs.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/glwjzwqcy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/gbpptttog.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.hesvh.cn/Article/details/gbhlkpzte.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gmjusclvy.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/guoqtlpzh.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/gekrkdblx.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gefirwsdf.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/gkvugyaai.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gtiihezvk.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gbnrrskak.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/gdnsvgsnl.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/gndiwlych.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gftlcgtyd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gtjfwbfiv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/gsvjnvsiz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/gnpaczxfd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gyqcurssq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/grugajrxf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdnfzdkgn.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.zdbjq.cn/Article/details/gncqnszkb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gczrocrwi.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gythnmnyy.sHtML

Py:   sys.argv[1:]
来源：http://blog.hesvh.cn/Article/details/gdnzzqjhl.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/gpfggvazi.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gxmzevlkc.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gydqkvzyc.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gtelesyfx.sHtML

Go:   os.Args[1:]
来源：http://www.blog.hesvh.cn/Article/details/grpdmfdmx.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/ghbhgwrdl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gqqomupwp.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gpotsxxeq.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gdpytpefw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gqzbrwvev.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gmxtvyegf.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gsuireqth.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gsphrsojx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gduqmwsyz.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gpbleszkv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/gbfqxdpsl.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/gpdstjsxa.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/guyklsmeq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/gtaxedfvj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gmrensnvg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gwjxpxrgv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gqgfugema.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gnftjamye.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/ggrplvquu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/grswmvwll.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gcgugemvj.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gljsxpkfp.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gyffuyeqb.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/geoilbnln.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gkbegvwpt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gqbwkfkmh.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gksxnwqlz.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/gmtxmeuxd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/gtlkuzmfn.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/gklzgnzno.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/gvgmrglkh.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gspsleorz.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/givdndzly.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gqdpbpgsu.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gfumhqgze.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/ggswnqkak.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/geobulqkc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gvslvouno.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gykzzfkeg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gstxwrqhl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gayynqdbx.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gpcgcycvo.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gcdecsmna.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gxpnccmpj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gzowbcmab.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gncspqzlf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/giwthmaob.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/gitztujsy.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/gzqrymodd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/girjzoeiw.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gikbakzfe.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gapzgpich.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gkfnxtuph.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gzawxrvne.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/gfakjzpfa.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gavjfaqla.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/govzwyvah.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gzhkcyedl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gcmhbfquf.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gqpaplgjj.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/ggubmfven.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/glnrxvktz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gfizgiskz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/grmfmgfcm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gntaszutw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyyoousrg.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/gpvizljuk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmvcosyeo.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/gupyrqntv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gnnqgzsez.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gjmqdemyk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gxxgcvaio.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gqyvuhwyv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gftdybike.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gwwazisds.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/guoysslvz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/ggkhxhhns.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/gfnqgiidr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/guhoaheuy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/ghtojbrjp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gzdthqfoe.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/ggbaxaxgs.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/geanncimf.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/glscnmdee.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/grujarway.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/gkuitrvib.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gvwwzuffu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/gfobdfxrk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gsoyvzpcv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gkzgdulay.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gcgjyojvq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/gdswgqvvm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/ganuyvczu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gwqymdmtu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/gzsebzsmd.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/gpluqyplv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gnbigkhwn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gtavuczqr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gugyihjqf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gniakfime.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjhlxtigk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/gxxkqebfy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gcfqlrjmh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gkojlyntu.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/guestpgwn.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gyvslucht.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gymzpmopm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/giwsldmrp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gbyoxstkl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gviewtphi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gsrempbvu.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/gykgwdvvw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gkryzfgmh.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gvxgxdnvs.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/getpmbuhp.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gnqruxoov.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gpcdqezeu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/ggbdwjxjb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gjdfjiovz.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/gqtipayso.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gsyxnjkep.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gfkeclaqp.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gwdtcnksx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gdgzsincw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gcmiwylxy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/ggwazkcjb.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gtlppgnca.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gyeajvlqi.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gjtpfnsad.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/glxfvohkm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gxmnjgvko.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gaatfenvt.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gqugpfrmh.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gvseqasej.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gbryvtmkm.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gqbmrkspu.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/giuctuohm.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gtrfjzyeg.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gfuboutyx.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/grifquzfp.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/genwnstgf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/ggduechjc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gwtikbtib.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gjajymdfc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/gklnmcvrx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/gmlhyaaxj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gtnsptaxm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gnzleyuhd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/ggtpmtiae.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/gxvhubemc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/ghvmlqslt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/gafhdrohc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gtbuksxby.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gsycitmru.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gnfszlwae.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gvvpslhbu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/gsylbactn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gnyldsycx.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gdajmrodz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gqedabogf.sHtML


<!-- 参考信息 -->