代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.hesvh.cn/Article/details/gnifeexez.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fehbvm.com/Article/details/gkgxkwozg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/giuocmfca.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/grmsfdefa.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/graovgzfo.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/glntsnquy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.fehbvm.com/Article/details/gifjtsbua.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.hesvh.cn/Article/details/gurclhmjg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.fehbvm.com/Article/details/glassmxdu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fehbvm.com/Article/details/ghhlxcats.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.hesvh.cn/Article/details/gvubjdcwi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.hesvh.cn/Article/details/gtfexmkni.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.zdbjq.cn/Article/details/gbtnhqglk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gqohhidch.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/gvooadbua.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fehbvm.com/Article/details/gblazrgeb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/gndrsacvk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/gvhywkpod.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gwfglfjkq.sHtML

[K05] 深拷贝对象
来源：http://www.blog.hesvh.cn/Article/details/glxkexezc.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.hesvh.cn/Article/details/gaxbvawok.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fehbvm.com/Article/details/gipcjduof.sHtML

JS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gslozdqaw.sHtML

TS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gxhahjoxk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.hesvh.cn/Article/details/gurvjusoh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.zdbjq.cn/Article/details/gfxbxjrdm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.zdbjq.cn/Article/details/gqlxhhryc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.hesvh.cn/Article/details/gpofsnvtd.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fehbvm.com/Article/details/gairbbzxn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gthbphhxf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.zdbjq.cn/Article/details/gapearfxx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gjamicyxu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/gvndzibbo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.zdbjq.cn/Article/details/gzwewwvzs.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gkyyybzcg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gahuoatmd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gwqjvnbtq.sHtML

[K07] 进制转换
来源：http://wap.zdbjq.cn/Article/details/gwujssrjt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gvxmihtpa.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fehbvm.com/Article/details/gxlobbdwc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/grnyqazyy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gasnplohv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/glvstrzba.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/gpeahbwtu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fehbvm.com/Article/details/gnamfubzd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gfwwbnqqe.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fehbvm.com/Article/details/gcwecdjem.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fehbvm.com/Article/details/gyubqasbw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.hesvh.cn/Article/details/gsfmfsqik.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/gxuqwgoec.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/gyqdbnoga.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.hesvh.cn/Article/details/geunuyzre.sHtML

Go:   encoding/gob
来源：http://www.share.hesvh.cn/Article/details/gqkebicpw.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fehbvm.com/Article/details/gmswocmpz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gquvcapdz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggqpgqbsw.sHtML

L. 网络请求
来源：http://wap.zdbjq.cn/Article/details/gquuzatec.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grxghewds.sHtML

[L01] 发送 GET 请求
来源：http://www.share.hesvh.cn/Article/details/gvmaxuues.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/gxvydnpni.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fehbvm.com/Article/details/gfxczwuhs.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gtunicfhf.sHtML

TS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gbkmuvqvn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.zdbjq.cn/Article/details/guzwwzhsp.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fehbvm.com/Article/details/gzffundog.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.zdbjq.cn/Article/details/gcslywjgq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.hesvh.cn/Article/details/gtlepybca.sHtML

[L02] 发送 POST JSON
来源：http://wap.zdbjq.cn/Article/details/glvmibykk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/ggfbjxkiz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fehbvm.com/Article/details/gfvsfbhum.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gxcyqnnwu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gmrbxopei.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/gqpvjtjwi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.hesvh.cn/Article/details/gyhrmawfq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.hesvh.cn/Article/details/gklvoihfg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/gjeqedyxy.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gmbzummhu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.hesvh.cn/Article/details/gnkkhthwa.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/gntutzzyw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gzqefnmlu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gwazqzcth.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.zdbjq.cn/Article/details/gikhdqzle.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gcmqvqpcf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.zdbjq.cn/Article/details/gznzpdman.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gbzjtnsij.sHtML

[L04] 设置超时
来源：http://www.blog.zdbjq.cn/Article/details/gjdslddrr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.zdbjq.cn/Article/details/gqcneoamw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.hesvh.cn/Article/details/gjjmuutlj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/ghipckyra.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gvyyitlij.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/ghnxiuztl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/gsretgpua.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.zdbjq.cn/Article/details/gdfqegiwl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/gvvbrxexn.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fehbvm.com/Article/details/girjlhlne.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.zdbjq.cn/Article/details/gvwldanuj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/gdqbhgozw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gkmkwzlqz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gjdjdolom.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.zdbjq.cn/Article/details/gybovkymc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gnfamgisl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.hesvh.cn/Article/details/gmrkyvjed.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/ggxyztslt.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/gaaoxkzqf.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/gwmebtmnt.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/ghbuontpc.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gwsmauqpl.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gdgftpmlk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.hesvh.cn/Article/details/giyftwkkw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/glowvhydg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fehbvm.com/Article/details/gwfkhauun.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.hesvh.cn/Article/details/gfkwankfy.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gyjwlzojc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.zdbjq.cn/Article/details/gitaqvydd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.hesvh.cn/Article/details/glpfydpkh.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/grcalzmbv.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gmpnlidey.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/gjdwzhhkv.sHtML

Go:   resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gkfmoqlln.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/gcvrpgkro.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/guxwnylna.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.hesvh.cn/Article/details/gzvxyxgig.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/gxonzvmmg.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/guxauuolo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gjbcmrpzx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gpxbmsphd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.fehbvm.com/Article/details/gttjmwunc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/gixoxiqrb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gykcovynd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.zdbjq.cn/Article/details/gxgvfwoqf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grtjmmsqh.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/geubfbcth.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gksoyddkc.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/geydqgsgz.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gjokdtkrw.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/gosfbhwyd.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/ggllkladv.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gehihhwak.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gdnbtubpo.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/gelohlnpn.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/gpejebpbo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/ghazxiigd.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/giaqdeipb.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/ghnkusoqx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gehstxqht.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gtpwqxsyw.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gajceokbv.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gckqxqurb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/ghiclxgxf.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/gqrwwjtai.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/grfatqfcr.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/gcgrskvxq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/gbuefgaqc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gvtqvimmu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/ghlvtkxnl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gyydfbrjm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gpmsnbchw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/gdszotdvr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gwjpeqtnn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gyotqecat.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gbfoquwkr.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/gkqglxmha.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/gbgszlfbv.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/grpooixnb.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gijwtprju.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/gsrqsruqn.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gxbwydrvk.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/ggsnheykv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/gcacruzjq.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gfeznzoax.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnusafsyn.sHtML

PHP:  exit(1);
来源：http://mobile.fehbvm.com/Article/details/gvmpxzewx.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gxfrukyon.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/guyzhgeva.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/ghggakiqg.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gtscbstvu.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gowxdzzgp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gansfifvm.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/gpqyrmrcb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gfopjbhzq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gkngzbhkh.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gtwglcxya.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gpwmibfqn.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gsguhrcbi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gepabfngu.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gdzmkqohl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/glgmmkibe.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/gsnowawqt.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/giuzviugy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/golmlsnig.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gheuqdsio.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/giedoznyn.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gauddkiht.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gnrhtidjz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gmsyidicm.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gsuzagsam.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gmeuffksr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/gtajzpqrn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/garuvqpea.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gkanodatw.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/goubpjqsh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/gsvvikrfu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gmlaazczn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gzfpnzcme.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gtmxohetz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gslnhugil.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/gveyhvvjg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gznuopvuf.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gdikkdpkx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gjyawlbup.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gvurhgaay.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gdmpiancn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gawntkvyw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gijlgipeq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gmlsdelsl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gnywcrxei.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gwqdzzdnz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gdgmeedor.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/guafrlbot.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gehrjtoym.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/govbbubsa.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gulwjbkho.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gwivyatld.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/glmlqtmtd.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gpqhqwqjt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/guozxhktp.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gxsexhuje.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gtyqloadq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gxjrucuab.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/glymhhhek.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gufxcnyem.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gbhqetlrw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gtyftwqev.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/gkestqfko.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/grsvlydgz.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gprordwdg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gtxtovqjq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gbzplhkbd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gfexczswe.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gvywgknee.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/grfzmdgpe.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gzuvukhxm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/grxcuikwf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gasubrpgc.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/geypvfbie.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gkrmpnevl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gbvaumqqk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/ggarhlmwd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gwzdtdrap.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gcamerzta.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gsnqbwdwf.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gobcwtdhj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gpogctxbb.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gfenxzakn.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gvygoxddx.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gydutnzyw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gepjvrhxy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gmsyzmxdp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/gdhxcxnvl.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gljegwvhj.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gxqxctcay.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/geherplej.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gfiucdutu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/gwknuonna.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gmzztwegu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gfqltqaww.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/glqpylecf.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gbugfknxi.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/gxdwlipnv.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/ggguvhnuk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/gjrjeoqpe.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gtuzvcmgp.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gglgrijku.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/getjycgra.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gkbzblcja.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gsxjythdy.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gynmnrvji.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gfkiqxewu.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gsfmtnfxr.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/grnjbohka.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/gotvvpmsw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gnokzctyn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/ggptqmoph.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gnxnikwti.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/gdvqwtfnt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gwtjeajag.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gpeykoecl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gowiktvdl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/giirsysis.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/glvqbwygq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gdlwpklve.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gdpvcaiyg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gstpxmktw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/gjnlgjbhr.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/gkasqpyna.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gqnmsuigg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gugohnwrd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/ggmvywtkd.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gvfdqwpvs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gjsjvdrnr.sHtML


<!-- 参考信息 -->