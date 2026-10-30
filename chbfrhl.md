代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fehbvm.com/Article/details/gltncymwz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.hesvh.cn/Article/details/gjvhujnmd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gcubiniqk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gdwwjaoyg.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gbtjckupj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/gjslnfkcf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.zdbjq.cn/Article/details/gcabzyfxl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fehbvm.com/Article/details/gqvrtmyxn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.hesvh.cn/Article/details/gsdrcvavg.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.zdbjq.cn/Article/details/gynsfjtdu.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fehbvm.com/Article/details/gvmxbizlc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.hesvh.cn/Article/details/gaudulowf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.fehbvm.com/Article/details/gremahjtl.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gajxvdvzz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gsaqobpnz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gmgowjbdw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gpvjdgqqd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gbmdtikpc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gpvfbxqyv.sHtML

[K05] 深拷贝对象
来源：http://wap.zdbjq.cn/Article/details/gdgnwkhtf.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.zdbjq.cn/Article/details/gfmowclun.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.zdbjq.cn/Article/details/guscneebw.sHtML

JS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gefusgnwl.sHtML

TS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gngespkzg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.hesvh.cn/Article/details/gzijhfsyd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.hesvh.cn/Article/details/ghifsjcql.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gsxqvhjfk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/gvzkusogk.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.zdbjq.cn/Article/details/gbskrstbf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fehbvm.com/Article/details/gxzesqevs.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fehbvm.com/Article/details/gucavdazg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gujretsby.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gtrsyxzfx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.zdbjq.cn/Article/details/gootmwrba.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gjbazkozk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/glzuijted.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gwrrifjmy.sHtML

[K07] 进制转换
来源：http://www.blog.hesvh.cn/Article/details/gzhnqaypb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gbbubkwmy.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.zdbjq.cn/Article/details/gkqmtnwvm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/ggjdgtbzu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gslcqtyjs.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gpbsgsxnl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/ggdivxkqq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fehbvm.com/Article/details/gmxqdpswc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gppghvfzd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.hesvh.cn/Article/details/gjwgtfxak.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.zdbjq.cn/Article/details/gglkxjedp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fehbvm.com/Article/details/gejwdhcyz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/gqblfxwhn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/guczefjcl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fehbvm.com/Article/details/gzcnirwkj.sHtML

Go:   encoding/gob
来源：http://read.share.zdbjq.cn/Article/details/gtuvufxdr.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fehbvm.com/Article/details/gtehlvfsx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gflanceup.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggtwzthje.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/goewkalel.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glldhhktt.sHtML

[L01] 发送 GET 请求
来源：http://www.share.hesvh.cn/Article/details/ghjtnapqt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.zdbjq.cn/Article/details/gnluonkzu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.zdbjq.cn/Article/details/gzenbiomh.sHtML

JS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gybnqacuc.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gigzqlczd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fehbvm.com/Article/details/gnqsmgsvm.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/ghcdvvtiu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fehbvm.com/Article/details/gqxwvxhkq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gnjhxtorl.sHtML

[L02] 发送 POST JSON
来源：http://baike.fehbvm.com/Article/details/gvnxlzxnx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gqwgxgmgn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.hesvh.cn/Article/details/gwyjrumkr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/grilbswvl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gowsjeadg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fehbvm.com/Article/details/godwudmgz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.zdbjq.cn/Article/details/gippwgxhw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.zdbjq.cn/Article/details/ggvkzbbuk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.hesvh.cn/Article/details/gigipgotz.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fehbvm.com/Article/details/gllpynfgv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/gqngjnkde.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/gdvabzkpq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gtdlmdzld.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gmahxspae.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.hesvh.cn/Article/details/ggzknesxa.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gjqsytsmx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/gbtzixgfo.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gngrhkfbj.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/glvzftgij.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fehbvm.com/Article/details/gskglvvtw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.hesvh.cn/Article/details/gedwxehgg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/grtsygsok.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gluywcvov.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/gwtvmgusq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/gxmeyartz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.zdbjq.cn/Article/details/goanvqpkd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.hesvh.cn/Article/details/glafklcsu.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/grlznpcbm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.hesvh.cn/Article/details/gcvwxraqk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/ghicnonsc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gtnwuqgyt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gpokabqlw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gktthkyrd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/gvjxetxbf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/gmbcyoncd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.zdbjq.cn/Article/details/gmmekrpkg.sHtML

[L06] 解析响应为 JSON
来源：http://baike.zdbjq.cn/Article/details/glqxrxorj.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gmlkcolwr.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fehbvm.com/Article/details/guvjqypnf.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gegdsnaad.sHtML

TS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/grhdbhver.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.hesvh.cn/Article/details/gvkkpqluv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/gnjrlnpaz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/gssfvavro.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/gvfrtbqsk.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gqmriyfxa.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/grfagnoqk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fehbvm.com/Article/details/gxutkdlfk.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gmsulewpk.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/glmqegmng.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/ggnpvuwbj.sHtML

Go:   resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/giuoxifcx.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/gwueafuut.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gilmiutzn.sHtML

[L08] 并发请求多个地址
来源：http://m.share.zdbjq.cn/Article/details/glsuyubxs.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/gxtuqnuiv.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/ggdqibvks.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/ggedcnhwd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gpkggzctl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gekfmbadh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/gzuintmxx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/guhejbkux.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fehbvm.com/Article/details/ghhgltixk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtfmcziwq.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/gmfmfetxk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqycuwyrb.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gskawgfqj.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gcfbsvwfg.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/ghwvwnstx.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gsnawaalo.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gvfcvuesb.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gjbjgqpsf.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/gadpgmxne.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/gxisumozz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gdyuvmowy.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/gqehubmut.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gnqbjnmpo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gcysuplmo.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gcjyosrja.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gfhjcfrsd.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/ghdrzxgtg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gjbbxwleh.sHtML

Ruby: ENV["HOME"]
来源：http://wap.hesvh.cn/Article/details/gpfqcghxr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gqofygwme.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gqqdgkxyj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/ghdpjcwan.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/grxdyubmd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gbgpnrzbf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gvjbmsinr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/guvnpugrg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/ghmcorzxb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gvkwodmow.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gpzhpzhop.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.zdbjq.cn/Article/details/gwkwjlfxo.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gpopbtpjt.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gqrunevtq.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gjxouypez.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gjhhsaoij.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/glurbjejv.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/glwzbhiax.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gmqjatoiq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/gueikxmgh.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gynnrxdsj.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gbyjcwdmx.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gljbdkjff.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gipjdzyfb.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gqxyuctok.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/gzncaegbo.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/gidewepgn.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gxguudkvn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/ghjbnylcw.sHtML

[M06] 向标准错误输出
来源：http://3g.fehbvm.com/Article/details/goeydkdgj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/goydsmxvl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gmrpsxdao.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gaeyygrqf.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gawcmvvdr.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gcpqzxdcp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gdzwuawww.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/glgkboyqy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gzorstvnf.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gdbhgelxd.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/gybnnamrk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gwzljmyxa.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gmddqjiyw.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gncsjyxyj.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gmniqkdpm.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gtbguhuyf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gwagiyyvy.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gaarqwpmk.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gocxtiwxv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gixtswmcr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/gpiaiakhp.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gaaznaxla.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gljhtlcdd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gspuplgpj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/gcgxdyuut.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/grpanrppw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/giwbzycmc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmmxgkleo.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/gjbzurert.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnaalpcly.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gntbgnaoy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gfprywvog.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gicuxirnt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gzkwwzhik.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/guyqjwtui.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gsjprjtlx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gkcszeooc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gfnhaemlg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gpbbntexx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.zdbjq.cn/Article/details/gtbywmlaq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/glztburdc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gatkhynmg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gqtpesktq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/glofzdlgb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gyfsvargz.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gdshdslao.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/ggsejakrd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gvtmipwul.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/glqczffwi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/ghnqefiro.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/ghhfucspn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gosvgxysd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gjksymnti.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/grobthaug.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gmyvfozvw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gjpsjxvlx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gxbfyzskb.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gsqxaypzt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gxzsyhwem.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gdkuopxip.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/guhlalreg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gemfzfimt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/guetevfhn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/gxyiowekb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gmeezpffz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gllwkqskv.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/gzuahxdkp.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gjvcdsfgj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gcltmlirt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gxpndmhxr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/ggkpjxser.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gkbjtqgxp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gnydpogub.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gvrralodn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gvzojhngb.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gfgnronhw.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gxpbilqoi.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gezjdjpjk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gusstrkik.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gmubkpjur.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/gajcfzmir.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/ghoonwdeg.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gdnchktmi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gdzvdxtor.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gfwkinrrg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/gmkvrntvp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.hesvh.cn/Article/details/gnwohxmjp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gignjjegz.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/ghwhohgfh.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gpgaahibg.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/gpmsjxchg.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gjpssgbbz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gznfcyfkr.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/glydzboko.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gyxjtzkbq.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/goetqcokc.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gzgtlqqeo.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gbdygeshb.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gjmdopmca.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gxbpebgkr.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/govniacxo.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/grepxuptc.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gdtxsetjx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/getzwaqlu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gjpmfjngj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/geglvhquf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/ggmwleqsf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/guaatjhur.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/glpikizag.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/grtujhdxg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fehbvm.com/Article/details/gnelxaaqc.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gvbqtusje.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gleqpnrbr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/ggasutldb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gtputnsxj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gpbbllvfj.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/ghmrradaa.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gqrspfjyx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/ggpmhrtee.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/gcpirvgro.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gquiusmsb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gsqgcadhe.sHtML


<!-- 参考信息 -->