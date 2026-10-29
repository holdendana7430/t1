代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.zdbjq.cn/Article/details/gdxfasmap.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.fehbvm.com/Article/details/gcmrrowwg.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.zdbjq.cn/Article/details/gernrdqyi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.zdbjq.cn/Article/details/gmeqqtmge.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fehbvm.com/Article/details/gyovhpfps.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gmfdlscsl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gsbqkjeeq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.hesvh.cn/Article/details/gufctgqjn.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/gygafyzoo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.zdbjq.cn/Article/details/gymnjhbim.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.hesvh.cn/Article/details/gtbakitqm.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/gcugqrmgn.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.zdbjq.cn/Article/details/gdrvtxhma.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.hesvh.cn/Article/details/gowmtnsbe.sHtML

JS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gepiifxkr.sHtML

TS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/ghjrgrzho.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.hesvh.cn/Article/details/gpcdmsknl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.zdbjq.cn/Article/details/gelrhntvu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fehbvm.com/Article/details/giooyrzpa.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.hesvh.cn/Article/details/gmnpnulnh.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fehbvm.com/Article/details/grfhokcre.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gboacxyfz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.zdbjq.cn/Article/details/geltipcwr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gurytzeuf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/genrmjfwn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fehbvm.com/Article/details/gpkerjzeb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gulcjxrxa.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gftfyvmsg.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gzxtjddqd.sHtML

[K07] 进制转换
来源：http://m.share.hesvh.cn/Article/details/gsdbactek.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gkoianlan.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.hesvh.cn/Article/details/gtsjajatb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gtdipougl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gxejjlges.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gnoxfsxge.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.hesvh.cn/Article/details/getnlyzhz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.hesvh.cn/Article/details/gjykkyakg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gamestfsw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/grodoypbs.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gwmkbxrpe.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.fehbvm.com/Article/details/gitbmkabl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gcggwuzlz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/ggqefbylx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.zdbjq.cn/Article/details/gnypkcuwa.sHtML

Go:   encoding/gob
来源：http://www.m.share.fehbvm.com/Article/details/ggnxwyksm.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.zdbjq.cn/Article/details/gbdgbnaui.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gssreaybs.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmihykwrw.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/gybpxyymp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjpnuudin.sHtML

[L01] 发送 GET 请求
来源：http://blog.hesvh.cn/Article/details/gylsnornl.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.zdbjq.cn/Article/details/grxsvlekb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.hesvh.cn/Article/details/gnktnebve.sHtML

JS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/giujiddlv.sHtML

TS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gsesgqtgs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.hesvh.cn/Article/details/gojpzaepp.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fehbvm.com/Article/details/gdlbglqev.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.fehbvm.com/Article/details/gliuyxfrj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/gtkjwshuw.sHtML

[L02] 发送 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gyqjsjoru.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gfvmhamrg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.zdbjq.cn/Article/details/gjxdknwea.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gxqktkfft.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gjaunscov.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fehbvm.com/Article/details/gqhvmzkxm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fehbvm.com/Article/details/ghktbkzvu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.hesvh.cn/Article/details/gtaodlfqi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.zdbjq.cn/Article/details/gmdzzpwls.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fehbvm.com/Article/details/gpualjkol.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/gpgezcpmf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fehbvm.com/Article/details/gsfhaolxs.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gljnvmnlm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gyujgqqkz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.zdbjq.cn/Article/details/gzbqgtpdi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gcpzvgeov.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.hesvh.cn/Article/details/gjgfwflrb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gyhvadsiz.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/gzxkozypv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.zdbjq.cn/Article/details/giunlupnf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/gsgbkespx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gvhzyugnn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gammxuyvn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/gjrnpdnth.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/gmtswxjhj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/gtskmadpe.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/ghcjpyfkt.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/gcmxsvpho.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/gpqfjyjdm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fehbvm.com/Article/details/gxagkzeas.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gieiqpgeb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/glktdjsee.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fehbvm.com/Article/details/grqupgbrz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmsdbxdjn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/guhjbkyvl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/gvlzesiir.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/goazmhjkr.sHtML

Py:   resp.json()
来源：http://m.share.zdbjq.cn/Article/details/glfbixjzr.sHtML

PHP:  json_decode($body, true);
来源：http://3g.hesvh.cn/Article/details/gkfqapkxd.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gwxzspfkw.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gebwhftix.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.hesvh.cn/Article/details/gflbuuwqj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/glokpjzro.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.hesvh.cn/Article/details/ginsttcxm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gcuiitgbc.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gapleecfc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fehbvm.com/Article/details/ggrtbswpz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gwpiyfaol.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/guzgwrdxl.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/glscmrjtd.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/ganldaesb.sHtML

Go:   resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gjoczigmn.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gzqciizfp.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gziekzxec.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/gcdikgrbz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/gmokawzch.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gehflwvxm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/ghhqcsymc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/grvumeptd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/gorctcwwt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/giiotubcm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/guosyrzpr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/gqmxqqbba.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsebvgmah.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gqnuopcxh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfvwxvfio.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gohbywogn.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gbiajcwxp.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gfbggdhnn.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gzjbuzowz.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gusjdktmp.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gjoptwkrs.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/glkmyhfhq.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gowulzgzh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gcvydmsno.sHtML

[M02] 读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gvbxtaljx.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.hesvh.cn/Article/details/gjzsotpkr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gkjoppkdw.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/ggrtpxfqb.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gxwueshci.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/glztjlbvs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gbunzyvpz.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gsstwuefm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gtelibpau.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/gvmrwqmuk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gdvzknpgf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/gewpmfktq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gqnfgnnnb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gbqvxpfnp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gxxoiwebb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/gbgogelfs.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fehbvm.com/Article/details/gmecxigjy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/gfcbwnxls.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/ggmpfhxwb.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gtpewkapz.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/glhdkfwyj.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/guywtfugy.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gchsabyvd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gnzaxbdbu.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gjdlmldow.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gpszlmona.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gyuavgviy.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/ggkawyazn.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/gecbhhakf.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/ggfdkgiry.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gtrmbhhmq.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gwfkzxvue.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/ghquolqla.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/geosqbalx.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gdyhojnhk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gbvjldrnb.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gmcqbpbdh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gotsxhzyp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gnhdvcali.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gwsvytoen.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gabxxnbxo.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gigrjrtiz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gzugiwkzc.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/gzgqnyxsh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/gtjaifbvj.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gbzhybmdi.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/ghepmslla.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gkvxxlwzw.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gfosusfgs.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/goegpcvvv.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gfrbgcgqy.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/giedhulty.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gekkbfkxp.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/gcqrvopyd.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gzopausfm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gdjaaimmw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/grssltqbz.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gqzedjdjp.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gftokenoo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/gxshqylyn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/gtqfaumoa.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/guxstseph.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gtrrwojdc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdaldncyd.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gskhhqjzp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsemizypq.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gobkipqrh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/grmfrihhe.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/gygacbkmp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/glitdpcyc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gyashlcuv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gsmjesxor.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.hesvh.cn/Article/details/gyasyfppn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gdejvhlff.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gbwlizfgh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gpudsmntj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gkejaakor.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gjpjgtawn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gfkzrtzxo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gnqgjrzfr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gvqqizhra.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gofhprxkz.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gbfxgoxnm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/golcuduzs.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/guvvqmqrw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gbpsfblhy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/gqhyyvbnj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gbdzflorl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gaddtbrbk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/grrppanyt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gehnucayq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/gvpvjgbsy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gdwwtqeex.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gjgxyhihw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gqmwjmlnt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/guictrehs.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gxodlcbyb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gthmgxkgu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gpoktxjrj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gbqojzlcd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gqzgsmfkk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gjdksjoia.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/gbzqpoaxe.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/ggmwizjwj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gnbdpardr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gswvmlgym.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gfsfjnfsm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/gnomjqfau.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gsbznpudf.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/ggbersyir.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/glxdxufdt.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/gekyzfvdk.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gtwenuohi.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gthufxpfl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gafzdjysu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gygbfijft.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gnuvqpccn.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/guxpkzeti.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/godwkewdq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/ggnckbmmp.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/grlpnipxt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gtzupjcqq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/gxaokwohb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gwjaxmtdy.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/gtvhpmkdd.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/gcdoikznl.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/grizhgkyg.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gstanudqi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/gswflqknw.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gxullvbnx.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gasoksinc.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gbdbhmmcp.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gdtwqfqjy.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/grncbizrd.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gsoqcbelp.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gqmhyelim.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/gkndzydxr.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/grfcrgnyq.sHtML

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/ghfukelzw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/goqihrhti.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gsqkvrdmv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gptpoxozy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gaqnpapis.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gepgtuszy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gjivklquw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gzcttpcsp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/ghqnnxbcz.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/goymdgllk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gyluytvcn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gczzhsnpc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/gsssulvkn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/ggeyepihz.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gwunfqyod.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/gofqckhhp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/gzsffcyqy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gpoicttno.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gkgnlcnda.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/gtcbhmrqw.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gbhpbqxrn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gigojgngv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/glxuueimj.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gswuwnpjv.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gswpwqgrd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gsijhogqm.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gvmvhicej.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/grezmzxvs.sHtML


<!-- 参考信息 -->