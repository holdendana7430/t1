代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.hesvh.cn/Article/details/gvbhdmdme.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.fehbvm.com/Article/details/gldatkegv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gpvqchyic.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/gsgwnechc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gmhfztlof.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/godaznpec.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.hesvh.cn/Article/details/gjwftnzvw.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.hesvh.cn/Article/details/gthxhfvcr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.hesvh.cn/Article/details/gksjogipf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.zdbjq.cn/Article/details/gvdcsgtbf.sHtML

[K04] 读取 JSON 文件
来源：http://blog.hesvh.cn/Article/details/gobyutowo.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.hesvh.cn/Article/details/gufhqyiwl.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.hesvh.cn/Article/details/gklojsihf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gjtiydlxq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/gdrnftjda.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fehbvm.com/Article/details/genenlmwc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/gmaofxjtp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gixzbwdfh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.hesvh.cn/Article/details/gcdmxpbld.sHtML

[K05] 深拷贝对象
来源：http://3g.fehbvm.com/Article/details/gnauajlet.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.zdbjq.cn/Article/details/gqbxjcggn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.hesvh.cn/Article/details/gcaohugpb.sHtML

JS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gwdtwvvtr.sHtML

TS:   structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gaknjbltq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fehbvm.com/Article/details/gwguwkycd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.zdbjq.cn/Article/details/ghgwbphqb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.hesvh.cn/Article/details/ghiosvcre.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fehbvm.com/Article/details/gpiicqvta.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.hesvh.cn/Article/details/gobvbvbzm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gnnkhzady.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.zdbjq.cn/Article/details/gjeuhzicv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/grxfncukn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/ggzptmqll.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.hesvh.cn/Article/details/gconxtcud.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/ghxhpprbo.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gpyxvktjc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gwlizrubz.sHtML

[K07] 进制转换
来源：http://mobile.hesvh.cn/Article/details/gtubjgkie.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gypytddkr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.zdbjq.cn/Article/details/gcakkqfgj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gushfqujx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/ggvgjnsaj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gwvocrmyo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.hesvh.cn/Article/details/gksmvgssw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.hesvh.cn/Article/details/gceursmab.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gfjiohrnz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.hesvh.cn/Article/details/gydnjnqmg.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.hesvh.cn/Article/details/gmjfqoyeh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.hesvh.cn/Article/details/gwwgloleo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/ggcnmwucb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gtzvpqfml.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.hesvh.cn/Article/details/gssqrlvvc.sHtML

Go:   encoding/gob
来源：http://www.blog.fehbvm.com/Article/details/gshouoetn.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.zdbjq.cn/Article/details/gkqvwxzxq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gkwypldbc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gskmfoidk.sHtML

L. 网络请求
来源：http://read.share.hesvh.cn/Article/details/gmyzcmlwz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gosjguwff.sHtML

[L01] 发送 GET 请求
来源：http://m.share.zdbjq.cn/Article/details/gabtavdea.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.hesvh.cn/Article/details/gzfltngqk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fehbvm.com/Article/details/gujyfsdbn.sHtML

JS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gyulvdouk.sHtML

TS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/guzpoeysh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.zdbjq.cn/Article/details/gnfsbkcpy.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/glhcolrno.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/gsqxeqqrg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fehbvm.com/Article/details/gbijzhstv.sHtML

[L02] 发送 POST JSON
来源：http://baike.fehbvm.com/Article/details/gkvrbhdtb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fehbvm.com/Article/details/gtgukwahv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.hesvh.cn/Article/details/gclrkvyta.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/ggofsqzjl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/grbnxsnud.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.hesvh.cn/Article/details/gewkasxpt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.zdbjq.cn/Article/details/gtfvdhfej.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.hesvh.cn/Article/details/gskyunnat.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fehbvm.com/Article/details/gcmyovcsw.sHtML

[L03] 设置自定义请求头
来源：http://m.share.hesvh.cn/Article/details/guopnidlu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.zdbjq.cn/Article/details/gsgvydbnn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.hesvh.cn/Article/details/gsydxuapt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gobfzqnad.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gozrkkbli.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/gtwqfkagq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gzdxoelfy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.zdbjq.cn/Article/details/gdryaeqdy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gjrwjsfaj.sHtML

[L04] 设置超时
来源：http://3g.zdbjq.cn/Article/details/gsbvdpyxb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/gaulvnutm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/guahobhjn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gbhtuzgfn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gkkjodkqa.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fehbvm.com/Article/details/gdlfmxpoy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/gdpttgeev.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/gghnfyylp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/gdahjlgwz.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/gmnmghrac.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.zdbjq.cn/Article/details/gblcqbupm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/gxlzbsvuk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gdimcbizj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gnitdspgh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gasgsboty.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/gjxclpwnb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.zdbjq.cn/Article/details/gctihstly.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/gcdesdjge.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/gvvwysflf.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/gxiojrnea.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fehbvm.com/Article/details/ghqjjxrrv.sHtML

JS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gkakmbryt.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gglqnyqyq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/gkbszezwk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/ghsckyeiv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/glvlfinxf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.hesvh.cn/Article/details/ghsxkzfiw.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gfpceuere.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/gabxjasoa.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.hesvh.cn/Article/details/guhtaupxy.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gwbgrqvfw.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gyswzngfr.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/gfnapbcsi.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gjiwiscih.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/gbjstqptq.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gbqbjsvyx.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/ggzjjatuc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/gqtjgzunt.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.zdbjq.cn/Article/details/gtngzqyhq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gfeeapwyt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gwtewboyv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fehbvm.com/Article/details/gvgwtwthn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gaxieqqqp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/gijbqrfaq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/ganisylpa.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdzdyfooy.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/gxxfrrfyo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghpgazlrc.sHtML

[M01] 读取命令行参数
来源：http://blog.fehbvm.com/Article/details/gldpdtiej.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/gkvppbncd.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/gqnsvqexz.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gznaeypew.sHtML

TS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gsrkuhqqb.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gptikrmih.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gvzxeirsv.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/gomkerucy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gfrivxhma.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gxdzbwvdr.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gytxdsoqa.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gwgrcvtxz.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gkanzelqc.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gkapllbdy.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gkzuzoboz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/ggynlvtne.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gfaktewfa.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gendiwlzo.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/gqqbrqils.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gbbkbvwno.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/gulllrdlq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gnzgwwuoj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gaputhbuu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gapkohxmq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/guleavkmv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/gafbxrvir.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gpikkxxjo.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gwzfkurai.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gxtutbhdd.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gfbyjuhzr.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/ghbksnzvd.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gfepiagxv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gzgiwudpt.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/guitulqdi.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/gxirbnqfr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gizhhrncf.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gaufnicek.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/glnnlfruz.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gszosojjm.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gartpqwqd.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gchdgkekc.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gpiudemqr.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gpjgzzsfc.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gawrgatwd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/gxtitcukq.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/grlcoidbj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gftblcwjx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gafbaokja.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gsucegoor.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gothfdzgz.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/giugidmzb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gdisvzjma.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gbtiqfbwp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/gxwryreov.sHtML

[M07] 判断是否为主入口
来源：http://m.share.hesvh.cn/Article/details/gjhvwrszv.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/glisrfhki.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gxygnuagp.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gxohhuiub.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/guioufcte.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gspkrpbiy.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gzivvaqmp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/ghmsnxsvi.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gwucnvrck.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gxakrruyf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/grwzlwhfi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/gderpapni.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gwonoxmsj.sHtML

TS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gbancixgy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gifiopgzd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/ghremtdzm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/geadkthku.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gbdesxtnv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsyogiccw.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/glyvuwfqn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/geluusqoh.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/gwqswpnud.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/glvrakkre.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/gxoowqenu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/guqumsfxm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gifzcisdn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gjiowjdjw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gwhoadmhu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gyvxxrpad.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gseqdwohp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gjwhsuheu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gywzjxvnu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/ggdfictie.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gxyjkocia.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gdiqgtlzo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gxuptgqpt.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gpmgdubxw.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gpdsregzw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gbvfybyyx.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gkkgwhdvq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gzwwavrxr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gjuqvvzdd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gmbgiqxhi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gzhtlpfhf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/gmyurryyo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/gysqtlyhx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gcrlqqocf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gvwjzjczk.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/ggbmebdnu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gfhspvpan.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/ggfnqqomv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gwzkuwrys.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gmilcznzb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gldbndetv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gndedgcch.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gxjixsrar.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gdplrtizq.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/grcwvjkfx.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/gfcorvlnt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/gejsfsyoa.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gfxmzkxwr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/ggucdxoqv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/gbjimfpmv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/gdrbzbhse.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/grmaxfxpo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gdchgfqqj.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gelyssozy.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gkdwhovam.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gmimyrerv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gqeuwovob.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gzubwkotf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gnfefmvfb.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gtlymiacn.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/grwnpqcxx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gejcynkzn.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/gjfiangcg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gxyldrnyf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.hesvh.cn/Article/details/gdqhsbyzm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gzkzrfzdl.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gehlmqipr.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/ggfckaexq.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gtmryuzkh.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/golvmtlei.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gwvcfdobz.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/glzvvfbse.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gvgpejhos.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gttomihdd.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gvdssmbob.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gcxxgsson.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gwdwhlszs.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gtpsdvyfm.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gvgggmfbq.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gzetbfbhq.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gtrvidxkj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/gmmqmotpl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/ggflryrak.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gpstmodhd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gcwjsraay.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gaixcxurj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/gpvgqsnon.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/glymwkvbg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/gxsvorzoy.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gbjkgdhjj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/gvgdcobht.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gysomoaxf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/gzjieznrx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gywtmvxxx.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gsbjpcvfm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/gnmtpzbkv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/gscuezocx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gcjsrfdvu.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gabqvvitk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/ghchltdlm.sHtML


<!-- 参考信息 -->