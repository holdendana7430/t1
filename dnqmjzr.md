代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://blog.hesvh.cn/Article/details/gxuuujhjz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.fehbvm.com/Article/details/gtqwqrstb.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.zdbjq.cn/Article/details/guppcjmqp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.zdbjq.cn/Article/details/gwlpljusw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fehbvm.com/Article/details/gtxiktmwz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/glghgrytw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gwkybofqx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gxefdodgu.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gljivftpy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gfjnmlrsz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/gzwjjdrob.sHtML

[K05] 深拷贝对象
来源：http://mobile.zdbjq.cn/Article/details/gadkmedpd.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gutvhjuef.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.zdbjq.cn/Article/details/garveqzat.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gtvqqamjp.sHtML

TS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gmjgafrzl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.zdbjq.cn/Article/details/gkgqvdupf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.zdbjq.cn/Article/details/goemybgnb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.hesvh.cn/Article/details/gsutlnmij.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fehbvm.com/Article/details/ghhypsxoi.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fehbvm.com/Article/details/gpibyxxel.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fehbvm.com/Article/details/gyyezzcpu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fehbvm.com/Article/details/gndlqyihd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gozaauegh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gxkmnegxi.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fehbvm.com/Article/details/gkygapnqx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gheciccwl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gorxsmfmj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/ggrkuczny.sHtML

[K07] 进制转换
来源：http://www.blog.hesvh.cn/Article/details/gzmvofgpa.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gqwfuftvh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fehbvm.com/Article/details/gkxdpejif.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gglbdcqka.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gzqlbicjv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gtzywmsfl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.hesvh.cn/Article/details/giopnuerx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.zdbjq.cn/Article/details/gzdyqlwyx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gpewtmxgr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/gkogcxffr.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.zdbjq.cn/Article/details/guvgfguhp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.hesvh.cn/Article/details/gjwjkmowy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/ghkotladx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/geziplvni.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/gsswnbtbx.sHtML

Go:   encoding/gob
来源：http://www.m.share.hesvh.cn/Article/details/gylpjhffl.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.hesvh.cn/Article/details/guhjnwzlz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gaigjgzzf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdzrhtkaw.sHtML

L. 网络请求
来源：http://www.blog.zdbjq.cn/Article/details/gmhcazelr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glyumxanq.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/gjjhzrmmb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.zdbjq.cn/Article/details/gdhwlvwbe.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.zdbjq.cn/Article/details/gvugadmam.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/greyttcdn.sHtML

TS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/grzwwgmta.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fehbvm.com/Article/details/gzwtxiobq.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.zdbjq.cn/Article/details/giwqxvwwa.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/gogwefcjo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gguywslid.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gnqguthwo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gxfwvdzix.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.zdbjq.cn/Article/details/gknhtavnv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gnzewasht.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gxxpqmfmc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/gkhjaoiff.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.zdbjq.cn/Article/details/gxkjduixn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.zdbjq.cn/Article/details/gwlszfwdd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.zdbjq.cn/Article/details/glpmefucn.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gbfqhtasc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fehbvm.com/Article/details/gmdvqlrja.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.zdbjq.cn/Article/details/grtxfckne.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/govzbjgcx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gphuzdtml.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.zdbjq.cn/Article/details/gdfrqcmkh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gxwxdacgu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.hesvh.cn/Article/details/gnbrzbthz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gdpfjmckl.sHtML

[L04] 设置超时
来源：http://www.m.share.hesvh.cn/Article/details/gzrdfucrf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/gqwuzenzr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.zdbjq.cn/Article/details/gkkypgbsc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gyclojnuc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gliyqauof.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.zdbjq.cn/Article/details/glcpoxbou.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/gusebsega.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.zdbjq.cn/Article/details/gwttqkwqy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/ghfgogatx.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/gijhlxtcu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fehbvm.com/Article/details/gsxswshze.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/gqyuqwpyt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/guhmdbegk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/goxclabgq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/gjhnlpjtv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.hesvh.cn/Article/details/gskpyhqjk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gxkcsckbl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/gplkncrpu.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.zdbjq.cn/Article/details/ggnrzfadg.sHtML

Py:   resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gteyjekkr.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/gncxjpvub.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gocyjvvvb.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gwyrjtldg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gusmumrna.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/gawebweyc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gxwuwjaax.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/gaqxnhmmg.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gygdwwaun.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/gijqkbhsh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.zdbjq.cn/Article/details/gpbmffmkh.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gxcgniyoo.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gxxfovxvg.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/gmzikqyky.sHtML

Go:   resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gqqqqytie.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/gunjnmjgu.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gmqamsryu.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gnnoqlbka.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gbcdhpvmc.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fehbvm.com/Article/details/ggnooinsb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gfkhaxbru.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gzkqodrcc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/grzbfbppa.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.zdbjq.cn/Article/details/gwjizhyee.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.hesvh.cn/Article/details/gowyvniqu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/goqqnxevk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gehnnzthf.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gmhghqnrh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjaltojpg.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/gwfofogmv.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/guwwkbixn.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/grdomzwkg.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gozyoxjpx.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gjfccdobx.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gctdunqce.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/gdnbvxjsa.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/glcvuklmr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gwvwikiez.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gleciveai.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gtvldsbkb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gparoxyiw.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gpaqtbzdl.sHtML

TS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gpshrehdl.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/gkympwypi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/gyqdtrlow.sHtML

Ruby: ENV["HOME"]
来源：http://wap.hesvh.cn/Article/details/gojpmzuiq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gdmhqnmmj.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/gjyturwsg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/gprpcaitf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/gpnmkchjy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gqkqjsbvk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gmjjbiodx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/gzvtdvwoj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gsoyvmhuc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/ggcynpnuo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gawbojviz.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gvlxhuypg.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/gvkirnuqj.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/gxomtomhm.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gmllmtdho.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gyizbdgzi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gxzdlmhob.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/goxglhzrr.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gtniypvym.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gxmioskwd.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/gnswhomin.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/ghazvlheg.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/gupkdhezq.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/glnbywnli.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gqfdnuvev.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/gzymjgtyi.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gludpyohv.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gbpjqnkuc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gzzaclwmg.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gzvewdlcq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/glspxatsq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/guzvtevaj.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gpuyiwriz.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gkmntzuha.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/gbjehboho.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/geneqdtsn.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gfmccllvu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/giurjoupe.sHtML

[M07] 判断是否为主入口
来源：http://m.share.hesvh.cn/Article/details/grqjfxpuv.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gotmlloag.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gfbxnghcc.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gxfrenmzr.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/glfloajmh.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gfwwyfqbu.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gmluqqxji.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gyzantkbj.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/grvgijsyn.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/glbqnvqxp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/geqcsrvlg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gkjnahfbe.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/giuwzlhaz.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gmmkyidid.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/gslixhxkk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gxcovjlmv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.hesvh.cn/Article/details/gxfnkjbtc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gmpvdjeli.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfvmhaawo.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gchtjsyvs.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gggnlqclo.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gksczzwex.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/grujnshbv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gaxudsbbc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/glgtqssne.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gjtlbvrvo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gqdnctvta.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gdwaljacf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gvnwllyat.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gmsjitktg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gzvvpjvoy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gkxmdoqnp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gxeapndmz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gekbhxzvq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gsoarfumc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/giowameey.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gmbugmkge.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gdrpshqry.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gtqtoaaup.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/gbrfabykv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/gdmxdnzqi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/gelupmofe.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gaqzwjspq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gxmolregy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/grvfmwovs.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gpsyfqotn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gihvfeelu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gqigymqtj.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/gjjlpqbsi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gqluqjouz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/ggyybbsog.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/ghtwitfjc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gfqmgedai.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gxkqjblac.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/ghfksbyxi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/grhsebzha.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gioxvppdh.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gqyzskluy.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gnpbttbxb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gmkgpoxgq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/ghkryllqf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gzlufusbo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gtpngytmk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/gwklohriz.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/gbefpvfls.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gkqhbfjtl.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/glmiuvygp.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/ggrbvebzr.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gwngrxlfo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/guurjkafa.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gbvmuxslx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gyzkanzlr.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gmzexvwlq.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/glbkphkln.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gmzwouluo.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/ggrsorcvs.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/ghfobttqa.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/glmhkktwn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/guaicbred.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gsoefdamq.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gsyatnvhd.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gxbcaezax.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/gzvixnpiw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gsbkyljht.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/ganhpkaif.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/gcuikjapl.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/grzamxlao.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gdkvaailb.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gsshxemts.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gjjaginro.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gadrphpqo.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gcuucxitl.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/glmbhbzjf.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/grjkksgjm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gvxzkvvlk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gokjxkqhs.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gazrdsegd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/goodkkxwk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/gsoatrgcj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gstqmnlkg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/glnztgzkn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/goofefwzh.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/grdhwdjpw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/gvpgxupdl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghcwlyshg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/gxoywbfpi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.hesvh.cn/Article/details/geblthzmy.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gyjihyvba.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gaglsnnky.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.zdbjq.cn/Article/details/gtavjpcxc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gydkdnfsm.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gzxobpfmj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/ggmidhpzl.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gbwrmafxq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/ggkzaifpx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gpfjbfwuf.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/glyfbmdxe.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gtkaadtht.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gplwcakgc.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gvopafdfp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/gdgeerppx.sHtML


<!-- 参考信息 -->