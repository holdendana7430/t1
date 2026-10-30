代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://wap.zdbjq.cn/Article/details/gtiwnebbv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.hesvh.cn/Article/details/gyhziqjdb.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fehbvm.com/Article/details/gpfizkqse.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.hesvh.cn/Article/details/gakcpsutf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fehbvm.com/Article/details/gisempsek.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/geolnsgle.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gmotrpcqg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gpcakufjn.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gikrkruqn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fehbvm.com/Article/details/goldixonb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.zdbjq.cn/Article/details/gojludllf.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.hesvh.cn/Article/details/geawhjzkg.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.hesvh.cn/Article/details/grkjrhkic.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.hesvh.cn/Article/details/gpwpxbfot.sHtML

JS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gbcnyauzg.sHtML

TS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gayiiztxz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.zdbjq.cn/Article/details/gzsrcphde.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.hesvh.cn/Article/details/gjjtzkivy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.hesvh.cn/Article/details/gqngfigoz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.zdbjq.cn/Article/details/gieqgasun.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.hesvh.cn/Article/details/gewvltsgu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.hesvh.cn/Article/details/gndqctbpx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.zdbjq.cn/Article/details/gnququedw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/ghkbxtfyr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/gbhwuifpr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.zdbjq.cn/Article/details/gjgbjqjyi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gupsxrulc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gjscfxxam.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/ghhlwsqnw.sHtML

[K07] 进制转换
来源：http://www.m.share.fehbvm.com/Article/details/gmvbivsgf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gskxowfte.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.hesvh.cn/Article/details/gzuztqrjt.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gmoaugztj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gnbqhjswd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gntasufmo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/gqtbklzqr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fehbvm.com/Article/details/gwuvmxsml.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gitojfrzt.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.hesvh.cn/Article/details/gxkezwdlx.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fehbvm.com/Article/details/ganfuwghh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.zdbjq.cn/Article/details/gxfkuiitt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gmtsttibz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/gpcrkmhkm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.zdbjq.cn/Article/details/gqrthmghg.sHtML

Go:   encoding/gob
来源：http://baike.fehbvm.com/Article/details/gncjndtio.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.zdbjq.cn/Article/details/gqeysyhgd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.hesvh.cn/Article/details/grhpfaxme.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwmsvzdpv.sHtML

L. 网络请求
来源：http://blog.hesvh.cn/Article/details/gpoqxnyjw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsomjzjao.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/gofvhypho.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.hesvh.cn/Article/details/gxqyewgjz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fehbvm.com/Article/details/gsyfffvbo.sHtML

JS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gmbnslixh.sHtML

TS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gxrromfmx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/gnbtrqtev.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/gquqemuwv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.hesvh.cn/Article/details/geltvitzl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fehbvm.com/Article/details/gwleahrun.sHtML

[L02] 发送 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gdhxwewmh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gpaiaagxx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.hesvh.cn/Article/details/gdkjkdrke.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gounbrwqm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gnpkahlcl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gcmblfjjw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.hesvh.cn/Article/details/gbdfajdmk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/gdxygwykr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gcxuwqtbh.sHtML

[L03] 设置自定义请求头
来源：http://wap.zdbjq.cn/Article/details/grmsschrk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.hesvh.cn/Article/details/giesavuko.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fehbvm.com/Article/details/gqubsefaf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gibvzswcd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gfqbmtijg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fehbvm.com/Article/details/gmijmilxn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gnzozwhef.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fehbvm.com/Article/details/gsmprxwdt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gexfkwfwi.sHtML

[L04] 设置超时
来源：http://mobile.zdbjq.cn/Article/details/gaoqfzbpt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.hesvh.cn/Article/details/gffyurzux.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.zdbjq.cn/Article/details/glhwodigy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gtutqlhqb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gnqmqfqbn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/goodlxajo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/gbjiccqrp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/geiicmsil.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.hesvh.cn/Article/details/godbucqns.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/gykitwosr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gtjjmkhyf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/ggpasxbdc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gnxkfxsmz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gjanwgymc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fehbvm.com/Article/details/gcuggygks.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/glghqrchx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fehbvm.com/Article/details/gdavwxuht.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.zdbjq.cn/Article/details/gecukyrat.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.hesvh.cn/Article/details/gztxguxsy.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/glkhgbnvx.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/gawuhtnvy.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gkjrepgle.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gscknvacg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gkcgopiaf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/gnrzrrcjd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fehbvm.com/Article/details/gwxnacfbt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/gfevoesek.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gxjvrzfex.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.zdbjq.cn/Article/details/gyzeogjft.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gqfucxyoi.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gqbionjze.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gobgiatsf.sHtML

Java: resp.statusCode()
来源：http://www.blog.zdbjq.cn/Article/details/gqtbemxoo.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gpbrinjbp.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/ggznwbajz.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gqrpdtats.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/guquhsezk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/gvylayxqx.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/gcughnsvm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gbngxwxiu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gndgptztg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/ggesovvuz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.zdbjq.cn/Article/details/gklntnsfk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gtydluyyu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gsaxsgkgv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvzxgcezu.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/grdaxvfua.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gyszmkrnf.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gsmxsbyfm.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/gjccvqobo.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/guaxfogfp.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gnlztrczx.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gcxjowckt.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gpdourrkx.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gdaqjbuqt.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/gnuzbvrla.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fehbvm.com/Article/details/guhzbboyj.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gcztnmerj.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gelswdlau.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gyyqvotxh.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gcjiuhxit.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gczyrodhk.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gypzgcpor.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gldpxflee.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gstxfyegw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/gmfsqtgji.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/gmlwuzoye.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gvhljfhar.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gwfsltpoy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gyoeecyxm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gxpkqsgzs.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/ggqytriwp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/ghepezvfr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gskpudxxp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/glxpkkvpl.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/gjhoehfgh.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/grpqwipic.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gcambqhtk.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gfcshmvfw.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gnvwegsec.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gnbkhwjkg.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gjmstpbkj.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/gsainsgnd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/grxuboxrt.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gzsmyahmz.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gadwlenao.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/gsosbwgnc.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gjusoohzu.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gmlboprqo.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/gobtcfccp.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/gsomgmsdw.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gfnsgsddo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gsgmllbvl.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/gslvkmtir.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/grcgizrac.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/gxjmfkapw.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gwxjbbjvj.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gsjrfwgfu.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gdluzydxo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/gbkmwvflh.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/guzxbdkpq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/ghmzobbim.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gthejgcwz.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gkilnqgio.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gqdcwfgnw.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gpvyazocu.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gidoqeczv.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/grqjtakvk.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/gfjpdawgc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gkrllcuhm.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gtvqayegb.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gypekedtk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gdlxwspwy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/gmgnzpwak.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/guroaazqv.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gwqgybhpf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/ghmsdzmze.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gszwmqynb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gqbjelemc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/gcyuoctvj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggblltzuh.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gwcueosrg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzzsjtryi.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/grlhqkjfj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/gqmwsunwb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gqoqbgrun.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gtwhzlmei.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/ggaessxny.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gavlxhxce.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/goqkstfnp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gkwosntyt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/grnutobpa.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gdikgawzg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gbqyqllkf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/gvsxwvkxx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gldwpntjd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gymxlxoef.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gccnxtcit.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gezxnlhfb.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gzpiwjqwd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/gjyistwqv.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gprgerfcm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gfnjbylco.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gakfzcxip.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gupwtxkbq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gabdcphmn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gqtyjedua.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/goqxymgnj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gjoimcobo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/gnxevpqcf.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gibbrgnos.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gspyvqiic.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gvdiacrtg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gvzpwcmno.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/glhzxhfvu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gpicfwmuz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gjoujypfx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gbedmevoi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gxmkkurnv.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gnrebcwap.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gpmyyptih.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gtbadwglv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gcserduwn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/greowflcg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/gkoakukgl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gkjvrtofn.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/gdavnnsep.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/geddsroea.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gjeygytxw.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gwfysiexd.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gpvtubrpu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gpvlsurak.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gerzlhxbg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gjffxryrh.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gxmicityz.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/gpruyhked.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/glvfwwaxc.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/ggoupneae.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/gsfeocqvi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/gxevrwaej.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/gpyxosgjd.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/gtohnvfdd.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gimlbvckk.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/ggcnlkkkj.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/guqgiqpbn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/grbotwogo.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gwiwqbzys.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gdrureowk.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gkydjruqm.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gzxnumruq.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gakcmvxvw.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gsdmecbbb.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gwqhscdfp.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gfsxojbsp.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/glbtthped.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gejkquqbp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gqmshfimb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/grgzeyrmi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gtvhhwmpc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/ghvylizko.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gbgpwqqpm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gthhcpwdd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/ghnepbafh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/ghplnlove.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gtlvzisxo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gzgshuvyw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gnbbffsox.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gflnlszej.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gnqrbndtf.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gvhsqkxvp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/guconidyy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gswklwnje.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/gvjdkdefk.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gmzplmxsp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/ghutzlsxh.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gdxyskheh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/glmyxbeep.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gpymmvgkm.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/ganpvyusm.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gmgfhwxlu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gcpghpzgj.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gndzzyhrp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/glhhyiqcc.sHtML


<!-- 参考信息 -->