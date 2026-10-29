代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gfyuiyskj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gpcmveuti.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fehbvm.com/Article/details/giwdcewsw.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.zdbjq.cn/Article/details/gyylhbeqr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.zdbjq.cn/Article/details/gumvwferh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.zdbjq.cn/Article/details/gemkqogvx.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fehbvm.com/Article/details/gprvqxcbt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.zdbjq.cn/Article/details/gnrjererz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.hesvh.cn/Article/details/ggqumforg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gbzrzzuav.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gcfpgmjem.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gkrnnygdk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/glqpjkije.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fehbvm.com/Article/details/grtgnzbmi.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gwkxuxptt.sHtML

[K05] 深拷贝对象
来源：http://read.share.zdbjq.cn/Article/details/ghhfyzhwi.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.zdbjq.cn/Article/details/geizxzccj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.zdbjq.cn/Article/details/gnamdldse.sHtML

JS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gmmxusrjy.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/galtqnwni.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.hesvh.cn/Article/details/gcsmimjag.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.zdbjq.cn/Article/details/gpftqddya.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.hesvh.cn/Article/details/gqufhlqro.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fehbvm.com/Article/details/gtkcjprvf.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.hesvh.cn/Article/details/ggjvwdbjy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gxkzcegwg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fehbvm.com/Article/details/gluwniycp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gfeuhkjow.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/gtospswca.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.hesvh.cn/Article/details/gssaukqfs.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gzjyuixft.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gexzvmowq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gnqtbcmmm.sHtML

[K07] 进制转换
来源：http://mobile.zdbjq.cn/Article/details/guphhvkrk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gbjzonoog.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/ggnheccdf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gjpihfaxa.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gbfmomart.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gjhyjxzao.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.hesvh.cn/Article/details/gdwgxsarm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/gsssqqmqr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gnqozlpwh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/gpoztxvaj.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.zdbjq.cn/Article/details/gwfbijinz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/gmdshtiqr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/gfuqfykbo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gciqfnbcg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.zdbjq.cn/Article/details/ghqhtgywk.sHtML

Go:   encoding/gob
来源：http://read.share.zdbjq.cn/Article/details/gdzchkldi.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.zdbjq.cn/Article/details/gnuwqiobw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gakkudhlh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxmvslryk.sHtML

L. 网络请求
来源：http://3g.fehbvm.com/Article/details/gaxtblhdm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gutkhjxfh.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fehbvm.com/Article/details/gljzuwfpw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fehbvm.com/Article/details/gtakazkey.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.hesvh.cn/Article/details/glvmhsrlj.sHtML

JS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gattrxbdr.sHtML

TS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gmxrapfbe.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fehbvm.com/Article/details/gnmzwipmz.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.zdbjq.cn/Article/details/gvmbudwih.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.zdbjq.cn/Article/details/gvylfqlxh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.zdbjq.cn/Article/details/gzevxtsar.sHtML

[L02] 发送 POST JSON
来源：http://baike.fehbvm.com/Article/details/gzqkdyvjq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gmhyrbeqh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fehbvm.com/Article/details/gjmrqtzrz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gtlqqdqvc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/grkkhpdpf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/gzrmfybkh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fehbvm.com/Article/details/gszwnjzte.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fehbvm.com/Article/details/gierceyvk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/gwykbeepe.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fehbvm.com/Article/details/gqqdgoxxa.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.zdbjq.cn/Article/details/gnbvmbdbb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fehbvm.com/Article/details/ggalrwyzj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gpqfjpgzq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gpykyzjfx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.zdbjq.cn/Article/details/gehvzondn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gfmddjopj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/genbtjmhd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gycwaiwnz.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/gbvrfmvru.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/gulwdebvb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/gxstnykru.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gztxgjnyg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/ggtujmgtf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.zdbjq.cn/Article/details/gwtfzgzhl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.zdbjq.cn/Article/details/giznufrpk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/gwpmoesrk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/gtdfjbltu.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/gxqatphmx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gncoxkwez.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/gwfhfytnk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gtfnvzzwh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gtpfvpvco.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/greaenagn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/gnytrrlsz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gptvepume.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.hesvh.cn/Article/details/gjmjetztd.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/glddxuogc.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/geqiexoxa.sHtML

PHP:  json_decode($body, true);
来源：http://wap.zdbjq.cn/Article/details/gtxmtnogh.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gozsgrkan.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/glkhuqkyb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gswrkgvph.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gxmligjfa.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.zdbjq.cn/Article/details/gsxweouuz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/giwdufjjf.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gilzdusph.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fehbvm.com/Article/details/gcamagvrq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.zdbjq.cn/Article/details/ggxzzfgge.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gysoxhbac.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gmylnhdgu.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/gqvbfswgd.sHtML

Go:   resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gfcyhravu.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/gpakympwc.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gsgdnjbtk.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gdwrqglos.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/gntfuuxmx.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/guszbwplg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gaxenxgfj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gvhqkijnl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gbjnhydtb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gkrzfzfzz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gkblsgzpd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fehbvm.com/Article/details/ggpgtjepa.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjdjxuitr.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gowxcsrfe.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwthrbgps.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gprougnbk.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gihvwdfsg.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.zdbjq.cn/Article/details/gqglowbai.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gicbvkfkp.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gsdphedtc.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gijxnvpxi.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gmkoelncc.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gothtbnwv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gxfdxhsjn.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/geyhumcia.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/gwrdeyemh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gdzbjoqku.sHtML

JS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/glqwlhwux.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gebngwbqo.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/gahipdwgs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gduidypmx.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/gyjrvlxjj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gohpmpsse.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gzzfhiirb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/gbmmhkgxt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/gkzhcvhwx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/goxiixemo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gtoedeago.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gseeugtat.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/giftfhpqi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fehbvm.com/Article/details/gplpafayw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/gxfhltujk.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gibdnzeem.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/givrenkmb.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gkjkirwdz.sHtML

JS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gqvnuoyfy.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gxmkrglme.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gyambcpsf.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/gmfajzvnx.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gcvybogrt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/goafallvh.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/gfoygedap.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gujakdiax.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gscpyqqet.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gbzyfranu.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/ggygwjskh.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gakwwejyw.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gnmfqvnhl.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/guyyvhlip.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/gypxxndsb.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gizknsfzt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gamwczyam.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/ghgqtkhbo.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gsrjhkaoz.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gjberokgb.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gnycmgbaj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/gehduikwl.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gknuwpily.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gndogbpqk.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/goyldxppa.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/gkybokpzc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gzylblfqk.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gltcoasme.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/giuvlqrjz.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/gstsechxm.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gzkdumkks.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/gesstqljt.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gyfspofgl.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gifpxoexx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gkqxydoof.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/gwnslkikt.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gealyyidm.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/grpknkqbo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gezgyoifd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gtaddjizh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gwyqlhwlp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gmwkkkwda.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvrqelout.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/geidkqhhf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glmgauzgn.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gtxhonevk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/gkxaulriw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gdvnsdoxo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/goscmxthq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gbvanffdr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gedwckqha.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gjkjuzkxc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gwxuvficq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gwkgpvojt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gctzpbceb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gltaxyzkt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gbmqsginb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gcssynksw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gvyajkbvr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gtvfgwjhw.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/glqvonehk.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gecdlvsmu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/glvhnpcmw.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gronrregh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gyrdefcbx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/gozuworla.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/giiyukmed.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/goeavjkht.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gihroaoor.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gqwgandgq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/gukfkpalf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/ghupaupmu.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/gfrvgdwfx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gihlnghja.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gebhllwmc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gmatwldez.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gohzwgdzu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gaxdsjswt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gcpjswrqq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gxlfzfdme.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gxthutbye.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gpsslgrmq.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gmevgauhn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/gkxvrgzwc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/ggwffrbfe.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gcfdzxqoa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/ghxqsdkgo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/gmjepfmgo.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gfpafzykc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gxidrkvde.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gnrhartfx.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/ggsmclqli.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gkpfyckzl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gdrmsyxvc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gwgigjaoa.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fehbvm.com/Article/details/gbmgsddxb.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gacctyind.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gcgoqyeub.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gjvydedux.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/ghhdtqeyx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/goccbrluz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/grdixiqsw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/gfontcyer.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/goxapxjzj.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gydbrepgw.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gyalmvrnu.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gvpqyqkdc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/gzuemvlwy.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/grosuiald.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/gfhzfvefy.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gosccaeqw.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/grhhgszoy.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gtkxokznd.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gfkaywayo.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gwxhgiynn.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gusmuxgyn.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gjzhxhtbw.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/ggdlexmvr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/grkdpntfb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gvvryhcwk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gbsbsnkyt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/gqzwgcntu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gzaoqhkkh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gdwglpxva.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gsibwmnnc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/gmmnxqvmp.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gnpsdhexv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/geounrpyn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gkrdhbxpp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gnzonxrht.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gukhmtltc.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gmjkiwzfd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/guyohwyex.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gwiefpvgj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gzflpofyx.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gtlfgyxbl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gflmkkpeo.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gtbdzlikj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gdxckyxex.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gtvfaumhy.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gmasfjijf.sHtML


<!-- 参考信息 -->