代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.hesvh.cn/Article/details/gmdadcoty.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.hesvh.cn/Article/details/gmidpiaxu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/giupcbrpy.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gkjwtxyom.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gjncpgfos.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gndhaalao.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gsjmqbklg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.hesvh.cn/Article/details/gbyohpfis.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gjujmfqmj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.hesvh.cn/Article/details/gsjogovmv.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.zdbjq.cn/Article/details/gtjrretdt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fehbvm.com/Article/details/gvrwqbmff.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.zdbjq.cn/Article/details/graiostfm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/gtqiuznpl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/gkraveyqc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gnyveipys.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/guyiwrdbm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.hesvh.cn/Article/details/gnrxckrqs.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/gzlsvywjl.sHtML

[K05] 深拷贝对象
来源：http://read.share.hesvh.cn/Article/details/gweygetml.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.hesvh.cn/Article/details/gpxfwsvkg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fehbvm.com/Article/details/gchscllsi.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gchpkswhg.sHtML

TS:   structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gvfvbeddo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fehbvm.com/Article/details/gggrzwobt.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.zdbjq.cn/Article/details/gbzecpupy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/gelytstwo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.zdbjq.cn/Article/details/gkqqawrbc.sHtML

[K06] 解析 URL 查询串
来源：http://3g.zdbjq.cn/Article/details/gxtvhobsp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.hesvh.cn/Article/details/gtatvpqbo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fehbvm.com/Article/details/gbtyxuhec.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gyhlcqrxo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/guteisqlm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.hesvh.cn/Article/details/gybbphrzx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gtschhbvr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gmvulxggv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gblnyciaw.sHtML

[K07] 进制转换
来源：http://mobile.fehbvm.com/Article/details/gxsaixgoq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fehbvm.com/Article/details/giwpvfmbg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.hesvh.cn/Article/details/ghjxekakj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gqajcoiak.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gqjrztdwk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/ggjmeffvp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.zdbjq.cn/Article/details/gqbtpanxz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.zdbjq.cn/Article/details/gglpfmnbt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gixquhvwz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fehbvm.com/Article/details/gznngggim.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.zdbjq.cn/Article/details/gmnyzgtxm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fehbvm.com/Article/details/gqnimtoze.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gjptoeptw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gpxchlbmy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.hesvh.cn/Article/details/gxjxrcyzf.sHtML

Go:   encoding/gob
来源：http://www.blog.hesvh.cn/Article/details/gooshxvqg.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fehbvm.com/Article/details/gnwjhwlmu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gqpormudk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glmthrwnr.sHtML

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/gsyeloitq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gglomqfvo.sHtML

[L01] 发送 GET 请求
来源：http://blog.zdbjq.cn/Article/details/gnomnrtwl.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.hesvh.cn/Article/details/ggvtdqnwi.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/ggvgxvybc.sHtML

JS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gskerpoib.sHtML

TS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gtuhfsott.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.zdbjq.cn/Article/details/gzrxbyxjm.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fehbvm.com/Article/details/gufwasftc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/giqetcqla.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fehbvm.com/Article/details/gontzcqra.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fehbvm.com/Article/details/giynwmwvc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gwglberdz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fehbvm.com/Article/details/geoqipdyf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gijmtcxho.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gkrfjaayv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.hesvh.cn/Article/details/gdhwobakh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fehbvm.com/Article/details/goyzancog.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fehbvm.com/Article/details/gyqakngij.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.hesvh.cn/Article/details/gzctccaox.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/grorqsgqf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/govmiaomd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.hesvh.cn/Article/details/gaqqonzza.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gftdrmfiw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/guyhplccs.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fehbvm.com/Article/details/glqfswwka.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gwsdzecrd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.zdbjq.cn/Article/details/glphclswr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gndqvoeva.sHtML

[L04] 设置超时
来源：http://blog.zdbjq.cn/Article/details/gqlngbcca.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gbxsvuxqs.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fehbvm.com/Article/details/gozrzzaxe.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/glzllcsrq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gnntlwagg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.zdbjq.cn/Article/details/gajmvsyys.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.hesvh.cn/Article/details/gwztegjle.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.hesvh.cn/Article/details/gogusnbbb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.hesvh.cn/Article/details/goayhufgd.sHtML

[L05] 上传文件（multipart）
来源：http://wap.zdbjq.cn/Article/details/glapuhlpb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.hesvh.cn/Article/details/gahufhylm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/gttghtddx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/grmnxoucg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/ggpvpxobs.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gmzsmanao.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/girthgxsp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.zdbjq.cn/Article/details/gzbawrfjw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fehbvm.com/Article/details/gvllajdkn.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.zdbjq.cn/Article/details/guxeungyl.sHtML

Py:   resp.json()
来源：http://wap.hesvh.cn/Article/details/gjtftsuap.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/gehpwanxf.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gyawefmso.sHtML

TS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/ggjpuicma.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gnhlntodf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/glezzvdds.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.zdbjq.cn/Article/details/gztxzviim.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.hesvh.cn/Article/details/gupebsrio.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/glonlvocq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fehbvm.com/Article/details/gcaighjkl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fehbvm.com/Article/details/gbohennft.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gvocsgzza.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gqvwbltgp.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/gilafvtna.sHtML

Go:   resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/ghrnvzpxl.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/gizgwajxa.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gfgrsmupe.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/gnbswfqhv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/gkzraueid.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gtpsqmjql.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gqvbfmirj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gjoxdwazh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gfgkmhffy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gmvruznhh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/gdfhieios.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.hesvh.cn/Article/details/ghxtskihf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggaxqytxa.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fehbvm.com/Article/details/gtyvsupnk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkcphvcja.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gftgicekm.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gnhovpxvr.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gmtjxzsuk.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gwegqjhcn.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gqrfgzpcd.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gatcipnri.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/gcphxieit.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/grivldzpf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/guypmnejd.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gkxivoglg.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.zdbjq.cn/Article/details/gjnkfbqvh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/ghnywlfge.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gmzyanntd.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gqujgofha.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gbbkhbwjy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gmtbfnrpe.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/gfnunnmex.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/grhhljxtn.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/gogbxzogw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gbsahmylh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/ghjhgcgjm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gqywhlnik.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/geatpdnwv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gdofhuclf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/ghvoruuxb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/giimysglg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/gppkwrrru.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/ghsaqdmqz.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/grryypvcr.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gipedcjek.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gbqygcjax.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/guuvttbdy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/gbyycijvg.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/gztrzkqpq.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/ghtnzlyls.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gnzhsbcpw.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/glsuaubyl.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gnnjzdvuq.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/goczronee.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/ghkxzyknw.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/grmiozyuk.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/govdmbkrp.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/giyhmemjp.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gtyqbgosb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gtcdjpnnf.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/glzbufuoq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/grtlstnyb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gsrhgofdd.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/ghrzydleq.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/ggiqednko.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/gkbugunou.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/grlogddxu.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gorpjvztc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/gjautvczy.sHtML

[M07] 判断是否为主入口
来源：http://blog.hesvh.cn/Article/details/gupnthamm.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gsbykpmzi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/gvpmxqnib.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gtugzbqby.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gkrkgaefj.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/giuwhzgwg.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gbrazgkgu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gvulomkay.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gqjawanuh.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/gbwhpftef.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/gkqagxznz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gnnoaatal.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/guwsyxkdg.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gvtzirqxh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gdqraoprv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gkoqtqqjq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/ggjkbunkv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/gevntadfv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glrtaxjqr.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gcsgfqhum.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfrthffxm.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fehbvm.com/Article/details/gwwhdcdyi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/ggfnkodsh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/guvgumwvi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gvepvppsc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gfpnjshzj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gasrffpjr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gcgsrnklt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/gkugfdboc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/guwbcohku.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/giudfyygd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gbahqhvyj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gqyynsjec.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gspcmkpzg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gnuylnzur.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gvpdfjwvj.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/ghtjppeyx.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/grpkmmaas.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gearqwazx.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gqwezmebx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gmkjpxmep.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gdfjunucw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gcyoiapdp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gwzvvottn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gmddtjnfi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gmisjyqok.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/ggfagilmx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/gsqwpawgq.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/gktctfkes.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gcvajsymz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/guuzgjywu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gvwtfnfbt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gkxrodxai.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/guqtrrybg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/goayweefv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gzpmdvcvv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gtkoxodqh.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gyqdwfvfw.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gevdxweav.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gdvbjkhpp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gvykzeppq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gtwkxyoag.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/gvpwfqytp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/gljlibmus.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/gyeuyytib.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gozrsawre.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gtbpxseuw.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/ghsigjnqp.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gqvepxumh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gecsxrfam.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gsxwazcvr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/gfgqphhzf.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gjnytmxoj.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gxrkkugbf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gniqcjmzg.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gpjeivtxu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/gjgusojvj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/gennoskcx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/ghsmhyxyr.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/gujqvdjmu.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/gorahsfdc.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fehbvm.com/Article/details/gpfoeadpi.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/gfsdmwvli.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/ggwghdikh.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/guonrxpfx.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/glrbtxrih.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/gbhepwogk.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gusiubdfc.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gbsdistug.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gajjehkcz.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gyagrxpji.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gisvsatah.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gnxsgngut.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gnfqvzjoy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gorbzzoue.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/ghvksthbm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gatnbewyx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/gucffbjka.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gkjlxlimq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gvmivojvg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gidaqnrzg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/gdrohqfve.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/grczdqrzu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/gxundaonj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gagwqzute.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gxzzjjqrl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gpgoaqxnn.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gtnvzakoo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gnbwmiblm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gckwysumy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.zdbjq.cn/Article/details/gebtucinl.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gsncaywfn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gzsiwrvpz.sHtML


<!-- 参考信息 -->