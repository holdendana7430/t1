代发 wailian999

[K02] JSON 字符串转对象
来源：http://read.share.zdbjq.cn/Article/details/gpngflnlp.sHtML

Py:   json.loads(s)
来源：http://blog.zdbjq.cn/Article/details/gyjstifwp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.hesvh.cn/Article/details/gnqahseti.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gwcuvecpz.sHtML

TS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gfzdxfmir.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gefdjkfzr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gyizeafdh.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gcklfxoxn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.zdbjq.cn/Article/details/gczhmgmpl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.zdbjq.cn/Article/details/gappxazjj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/gtanwxhlg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.zdbjq.cn/Article/details/gspakkzkm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gpivpqqzf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gzqqiirkz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.hesvh.cn/Article/details/gvyfotlpk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.hesvh.cn/Article/details/gwoyidxuw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fehbvm.com/Article/details/gjdzkedcd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.zdbjq.cn/Article/details/grjdelpnc.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.hesvh.cn/Article/details/gtvhpkpuc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fehbvm.com/Article/details/gyzymodfs.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.zdbjq.cn/Article/details/gkbtxjmfv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gtrjntpee.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gkbvwywmh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gzwuzfxlw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/ggbgjwzun.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.hesvh.cn/Article/details/glcfpiddh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.fehbvm.com/Article/details/gyfvhygch.sHtML

[K05] 深拷贝对象
来源：http://3g.fehbvm.com/Article/details/gixeekkoo.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.hesvh.cn/Article/details/gctejywzk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.hesvh.cn/Article/details/gclrldues.sHtML

JS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gcgsisszs.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gpkhkiqpm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.zdbjq.cn/Article/details/gitjfsudv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.hesvh.cn/Article/details/gbpubrfzy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fehbvm.com/Article/details/gyreoveuj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/gvndetrpn.sHtML

[K06] 解析 URL 查询串
来源：http://wap.hesvh.cn/Article/details/gsmzkypkx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gfbjyuwcz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.hesvh.cn/Article/details/gfhrbxzze.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/ghfrrftec.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/grtpusswc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.hesvh.cn/Article/details/gzetzgvdj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gwfjmhxig.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gjlavmkqb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gdmjqdqps.sHtML

[K07] 进制转换
来源：http://www.m.share.fehbvm.com/Article/details/gtopspsfi.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gskczundv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.zdbjq.cn/Article/details/grdnbasvr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gmblpfbuq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gvxgadfxm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gbhammkfq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fehbvm.com/Article/details/gqoudsqub.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.hesvh.cn/Article/details/gfaygipqf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gjtgqfoja.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.zdbjq.cn/Article/details/goiuorokq.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.zdbjq.cn/Article/details/grwaysppz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fehbvm.com/Article/details/gruureqkj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/ghrnkwuig.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gnssrdmoy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.zdbjq.cn/Article/details/gspjbwbba.sHtML

Go:   encoding/gob
来源：http://wap.hesvh.cn/Article/details/gnumpqaux.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fehbvm.com/Article/details/gdmslirjg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gfsmczlvo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdwjiernf.sHtML

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/gcwkgvzwl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvdynaiyc.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fehbvm.com/Article/details/gugjnetmb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.hesvh.cn/Article/details/gxttpeyxg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/ggtlyydtu.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gtxciyjrt.sHtML

TS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gsgxnkfnw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.hesvh.cn/Article/details/gtrtflnxf.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gyrnbifgy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.hesvh.cn/Article/details/gvjslmpfb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.hesvh.cn/Article/details/gynfasyzh.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/ghafzulos.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gdchogdwv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/gldqhsvkt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gxtgalsfa.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gyavracjp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gxrgbtpfh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.zdbjq.cn/Article/details/gvrikykea.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/gymkjqsuv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.zdbjq.cn/Article/details/goqkzijtq.sHtML

[L03] 设置自定义请求头
来源：http://m.share.hesvh.cn/Article/details/gjrirwmfd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.zdbjq.cn/Article/details/grmiuvypk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fehbvm.com/Article/details/gpgcenbgt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gquxufztd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gtideldvp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.hesvh.cn/Article/details/gntezlecs.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gvslolvej.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.hesvh.cn/Article/details/gmyhssxbd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gcxtnsfsr.sHtML

[L04] 设置超时
来源：http://wap.zdbjq.cn/Article/details/gttwhckmb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/gwtyuouks.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.zdbjq.cn/Article/details/gcircpydv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gwfbgxtel.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gvapcpjud.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/glhekiied.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/gvesobiif.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gaxocfvqh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.hesvh.cn/Article/details/gvcxhddkn.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fehbvm.com/Article/details/ggfgkmhtm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/gtnhmkshy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/gqrzdecie.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gjrexcnup.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gjrtwdjej.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.hesvh.cn/Article/details/gntxssqqx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.hesvh.cn/Article/details/gholqcwlk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.hesvh.cn/Article/details/gcxrfmnxp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/gnzpzlgho.sHtML

[L06] 解析响应为 JSON
来源：http://baike.hesvh.cn/Article/details/gegvpvyug.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/gmjhzdnqr.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/gwirbnhyz.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/ghbpstcxw.sHtML

TS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gwazdpttb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/ggtqtoget.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.hesvh.cn/Article/details/gkkxobxeb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fehbvm.com/Article/details/gxhigekye.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/gcyjjrowq.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gzzjpdsnl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gebxeapqg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/gmfkcozic.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gorluvzkh.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gsadctquu.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/gdddklhvu.sHtML

Go:   resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gkqmqetjb.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gfbhfxjjo.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/ggjjccuds.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/gwyzacuiy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/gkxdumyhp.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/gpbvmnnce.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gtijzkxfc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gswnmsfxo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/goyaehvbi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fehbvm.com/Article/details/gtgbovkpr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/gsskornpu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.zdbjq.cn/Article/details/gfxrzdnfo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbhrfodii.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/gcquzsuzi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyyhdtxyp.sHtML

[M01] 读取命令行参数
来源：http://baike.zdbjq.cn/Article/details/gtegvbxfh.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gbzzftrpb.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gfozfvuxa.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gxlrmskip.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gqnksxmrj.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gqjtwywcu.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/gckxfbtyb.sHtML

Ruby: ARGV
来源：http://www.share.hesvh.cn/Article/details/glaucyzpz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gllxfukav.sHtML

[M02] 读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/giyvrddji.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.zdbjq.cn/Article/details/gdhfcowoi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gjljydfzj.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gainmijqx.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/giifadlma.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/gnwsvykdx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gvaedykup.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gatzkjccw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/ghjkmoymx.sHtML

[M03] 执行外部命令
来源：http://baike.zdbjq.cn/Article/details/gysopejxq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/grnivftgi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/gedyolcev.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gofgxlwct.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/ggshcigfm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gflscpmmv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/gmxxrfoyt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gccxtdsio.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/goujqyxgq.sHtML

[M04] 获取当前工作目录
来源：http://3g.zdbjq.cn/Article/details/gxcbvqxvx.sHtML

Py:   os.getcwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gegvlnfsx.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/grjvlvtqw.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gdyjmcfjg.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gtymzqlbr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gtpucirrq.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/ggrkzbttj.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/gbwlmzxce.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/glpqsyyaj.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/glmyijdrm.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/glnanzwpu.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/ggvmuazes.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gtesxtlqb.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gpkiojqmt.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/gcnyofxtj.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/guhyyvdma.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gidoeofiw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/gmoeeabsr.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gsbbjqzte.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gbffclswg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/ghwsayvyr.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gcoeuumuj.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gvcdjcmzz.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/gnmeyyzja.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/gxfxtmimb.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gebvavsmi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gmfplcomo.sHtML

[M07] 判断是否为主入口
来源：http://blog.hesvh.cn/Article/details/gajsadnjh.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/gloqjovnn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gqojdupsq.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gmecalqvu.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gnwhvgaob.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gmjeinqaz.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gyaijdauw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/guduanwui.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/gfzkkswjz.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gnxoniuqq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gehvfksyx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gqxnrakyl.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gdxddfibw.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gxfnwcgky.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/ggashutoo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/gxcqtowur.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gqifatkbz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/guqdddvbd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/giltdomlu.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/gsrkgmkph.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvzvpaafa.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gyciayfua.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gvnswfhre.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gzqelrujv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gzkbyaved.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gejcrgakt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gausljmsp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gjspexerq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/glwbrwdcs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gioifgefu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/gqkpwwost.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gyxgjiekx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gbcjemsrg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gjizqpxmm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gxtswyfli.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/gfetbswgg.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gnnmiymln.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/ghbhxphpl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/gsvmvzkov.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/gumnsczmo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/gokjkranf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gedifmmuz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gyrnkizvr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gfpaxappf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/gvycuiint.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/gxoytqvta.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/glkjlwahh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gydsgfifh.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gmdrdstvf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/ghllrzkal.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gfozlhwld.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/ggtrjmvmk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gxpybdlek.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gddvbwrih.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/gahnaprml.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/guipkvcov.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gjgkmfvsr.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gtcrcbcqy.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gxwnvbkjs.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/gbpazztqe.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gypesrwhv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gkjfyhggd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/genuwiccv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/guhoutecc.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gtnrkrebo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/goiympnzg.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gtkptkphf.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gblfuxkix.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gtunnodhb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gohewvmlb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gadgfbedf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gsyictjgu.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gtzqavqjf.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gsyylffff.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gljjksogs.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gydqcbhzv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/glylfrwzz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gjptyzswl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gelfvcejj.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gynvuonph.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gqgqvgacg.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gxqdoukgb.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/gchknhdcq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gvjcpqejx.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gnsosqqrx.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gzevtphax.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/gnbmpapef.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gfipgjpdl.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gjzzofeen.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gudkgpkwo.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gujnbqhwg.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gluxyiqhu.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gomcksyam.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gslyftfvr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/giwqyvgco.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gcbnppply.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/grdzuwxve.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gzfknwuyd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/garsddstw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gedxfddle.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gomlddsuo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gsjdsisqp.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gmsrkzdxn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gwkijtpya.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/glxejvokb.sHtML


<!-- 参考信息 -->