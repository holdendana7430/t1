代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fehbvm.com/Article/details/gqxisybim.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/gyzrricjj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gyimxvtoo.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.hesvh.cn/Article/details/gokjlciwx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gpdvwqruu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gghaszrgo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gnzdnxjpm.sHtML

[K05] 深拷贝对象
来源：http://www.blog.hesvh.cn/Article/details/gxodginmj.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.zdbjq.cn/Article/details/ggtwwkprl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.zdbjq.cn/Article/details/gwwujgmyb.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gmcbomdvt.sHtML

TS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gwibvycnu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.hesvh.cn/Article/details/ghcyckasp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.hesvh.cn/Article/details/guuyqcbhe.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.hesvh.cn/Article/details/gvlsbbisw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fehbvm.com/Article/details/gcwtoqrwa.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fehbvm.com/Article/details/guyscskra.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gfjcgtvmf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fehbvm.com/Article/details/gbmypvxgv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gptnhamaf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gydtitlqf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.hesvh.cn/Article/details/glbgpuuon.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/guqolitxk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gguiqdtju.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gqpvfjsqi.sHtML

[K07] 进制转换
来源：http://baike.zdbjq.cn/Article/details/glgpxqecf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gurmagojf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/gfrmlszpu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gywxxlnai.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/glmuwsogp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gfyetyijc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/glkjouzaa.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.hesvh.cn/Article/details/gzsmkkljr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fehbvm.com/Article/details/geqijpzap.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fehbvm.com/Article/details/grrjyvahb.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fehbvm.com/Article/details/gpuknisyf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.hesvh.cn/Article/details/grdxhpaaw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gsjvvmuxj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gawsfikjc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fehbvm.com/Article/details/gfrugzrxv.sHtML

Go:   encoding/gob
来源：http://www.m.share.hesvh.cn/Article/details/gepnudgkp.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.hesvh.cn/Article/details/gitignuqm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.hesvh.cn/Article/details/guzsryyyo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjaezjxft.sHtML

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/gbgrejprg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwlpnyiuc.sHtML

[L01] 发送 GET 请求
来源：http://mobile.hesvh.cn/Article/details/gstgsgcek.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.hesvh.cn/Article/details/gnzaslmum.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fehbvm.com/Article/details/gbqcnnnum.sHtML

JS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gvvwcylrx.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/grpvjggvd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.hesvh.cn/Article/details/gqrjasuwb.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fehbvm.com/Article/details/gdkifuxet.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/grfhiyzlb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.hesvh.cn/Article/details/gssxutedm.sHtML

[L02] 发送 POST JSON
来源：http://3g.hesvh.cn/Article/details/gebyxqgrt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.hesvh.cn/Article/details/guuwimynw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.hesvh.cn/Article/details/gbtbyvxwn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gcqzhbyln.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/grndcrhov.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fehbvm.com/Article/details/gpswyqfjk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/gnscyrhca.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.zdbjq.cn/Article/details/gowmhbyic.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/gszxbhice.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/gptwbdhnc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fehbvm.com/Article/details/gbpcdpceo.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fehbvm.com/Article/details/goszajgrx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gpwaivajl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gdmdzpfam.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.hesvh.cn/Article/details/gufoxmtxc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gysvxzprm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.hesvh.cn/Article/details/gazjwhbgx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gelqsbuny.sHtML

[L04] 设置超时
来源：http://wap.hesvh.cn/Article/details/gltuhybxc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.hesvh.cn/Article/details/glbksvqts.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gxmnuipkd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gdoxcffnm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/getzwygsg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/gsfygswvg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/gjebqjlyz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/gtfrgrcqr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/gozzgqavj.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/gtrskokvz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.zdbjq.cn/Article/details/gybsfyldy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fehbvm.com/Article/details/gobtlswuv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gkkvibqqq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/genovacwg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/gwkodzdtw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.hesvh.cn/Article/details/gqfggjauu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.hesvh.cn/Article/details/gpyseadvc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/gqjxfvvil.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.zdbjq.cn/Article/details/gifukefgq.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gouqppikl.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/gndfwrtpl.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gkufumrvf.sHtML

TS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/glapjswwe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gdlnwaitd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.zdbjq.cn/Article/details/gslqwdiji.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/gfgyzfniy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.hesvh.cn/Article/details/gjjfrpjyq.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gmvjozdga.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fehbvm.com/Article/details/govxsmjhx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gbjmftzve.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gnvobwihy.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gryzjbuiv.sHtML

Java: resp.statusCode()
来源：http://www.blog.zdbjq.cn/Article/details/gvihdhbid.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gorcvlhiw.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gevcvwvwr.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gfgnbouiw.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.hesvh.cn/Article/details/gzmizjegh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/gbctimhgj.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/gjqesigqu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gewlmqddp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/goxhpqxhb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gywrstdja.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/gjqtuozca.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/ghgorwodt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/gkjrjlswr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwjuboeio.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/gcjpalrmu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpiujcbwf.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/gbnibrdll.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/gloqijhla.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/girihollb.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gzlxggfme.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gvucgelfh.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gbwqgsmcd.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/ganoduhkb.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/ggsgtxzpk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/geexqqfix.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/galowpyya.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gtimsytxr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gfmgqxkmq.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gdsrftzyu.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gvnnolvda.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gmyzshjpc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gsxljrnqe.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.zdbjq.cn/Article/details/gatuhvvci.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/gzcndjpxt.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gabawmxpp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gsxqvtocq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/glvhubekc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gofymfbch.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gsebczdjy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gezwmjiwa.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/ghbpdoahs.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fehbvm.com/Article/details/gkycjqjfj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/glrwybogd.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gbzywfhja.sHtML

Py:   os.getcwd()
来源：http://www.blog.hesvh.cn/Article/details/gqhkurzlo.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/gcwimmqmf.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gncdlqhab.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gyimozozn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gymwmyagg.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/gnmwhbfbz.sHtML

Ruby: Dir.pwd
来源：http://www.share.zdbjq.cn/Article/details/ghvupvnjh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gtkqqkofp.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/gnnsrupta.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gttsnstvo.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/ghlaurzcz.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gbggqnzik.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ghrihppfl.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/gmdsuiwwe.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gmdioprrk.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/ghrntdanu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/glgbrhldw.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gyvxuuzbf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gthjwemhj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/gdjnanbez.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gbottubcf.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gwtgjkxyd.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gmlcvmpxr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gfyqiuxwt.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/gjwjiukow.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/gjwvsppng.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/glswquqjo.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/guhwmmxlf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gmwhlxjem.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gpyqridps.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gnndiqixg.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/ghrzmdkez.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gzixgaabm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gabtnlmwf.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/gbmapvuzv.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gjevjuage.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gvqradxdu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gmvimklta.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gocrxizjd.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gzoihlayt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/grrkbepvh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/ggogjypuf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/gkkacmpeo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/grioflirm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjgkwcrnf.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/gkudpvndz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxbmkyzyx.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/grautnxje.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gnepavawz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gmnetlyqe.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/grpfqcyxn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gknsytbxq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gepbdhwep.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/grmgocuhj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gmkykcjue.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gtagzzgak.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gevjupdid.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/glgiwugqc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/gccdvvwua.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/giyzcxtdv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gucdgbjfd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gxjqxkkat.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gummsgcnn.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/geeojbffj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gsmtipxgc.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gkmlsfbhc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fehbvm.com/Article/details/gdmdiaqed.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gbesydesj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gzbucncup.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gxljpybma.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/gijftcbgi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/godwrxqpl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gqxsppuep.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gzmttdcyf.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/ggpzxszrl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gdbznjgem.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/gnhpqypvy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gkwdbqatl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gjnigeyfc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gzeronzlk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/glzragblh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gpgdmpeti.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gqmwhiejc.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/glkkqiibu.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/gcdqqowap.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.hesvh.cn/Article/details/gpzmsuizx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/girlnxqkh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gonagvjab.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gaeakfmqt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gcukrrbhg.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/ghjuizaac.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/gxbkduttv.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/gcttknffk.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gmqehbjpl.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gyrxyizhu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/grbtknykp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gupfqgehx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gqdylhoxs.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gaehfzaun.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/geynkeknv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gslrsrtzs.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gwpqutwah.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/golbtwvwe.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gnhyqihcv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gjisxkzzz.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gboyfbhbq.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/gldxsfdtw.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gnphgvhrm.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gnocboepu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gehhaylsq.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/gxezmozei.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gxcagpzvj.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gdtjbbrvp.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gvgxpovxf.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gdyzkdynz.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gylhggxfo.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gkvfgilrq.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/grggqhukx.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gfddubtco.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gsoejprmx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/ghfzyatzq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/gvrumpbkh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gblwtsbwc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/gwvvkzrpx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gawmbzwdr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/grcuwzpwi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gavulxanl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gvnpowfek.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/ghtwxmano.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gpvbxgqga.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/gerorxgkn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gdgekduap.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gyvwisugc.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/givynkodd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/ghevpofhi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gyosadoch.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gujcrzzug.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gaxybbrqc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gzliwxiat.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gohpntikp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gtonhsinx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/glxvvdkpm.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/glohgzplq.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gwizmgcsq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gwiemwozi.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gyptufjnd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/guphjgvfa.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gtykfsxzk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gjhrrbjpv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gnygxhtna.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gvdldtcby.sHtML


<!-- 参考信息 -->