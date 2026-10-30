代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.hesvh.cn/Article/details/gcaswwygc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/gwrqpqfop.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/gbkejymlw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gudpqgboo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gqylkfalr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.zdbjq.cn/Article/details/giytcoidv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gbtjjugdl.sHtML

[K05] 深拷贝对象
来源：http://baike.fehbvm.com/Article/details/gnmfsdyij.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.zdbjq.cn/Article/details/gawlmyrpb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.fehbvm.com/Article/details/gmvuvplah.sHtML

JS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/ghouxjwaf.sHtML

TS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gpoqqznwe.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.zdbjq.cn/Article/details/gkysbdtzz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.zdbjq.cn/Article/details/goattquuk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.hesvh.cn/Article/details/gfrjyxadv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.zdbjq.cn/Article/details/gbjbvqwhf.sHtML

[K06] 解析 URL 查询串
来源：http://blog.zdbjq.cn/Article/details/gimwosszi.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gpihwrkae.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.zdbjq.cn/Article/details/gqwuxlxdm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/grpfpcdzf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/grnqqlwxz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.hesvh.cn/Article/details/gocevfsde.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gjsshxyaf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gdnvqbvos.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gooylwltb.sHtML

[K07] 进制转换
来源：http://blog.hesvh.cn/Article/details/gmzirkfrg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gcjcmjwnh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fehbvm.com/Article/details/gzmhxsggo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gswqonbpu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/guifjgrwj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gdpnrojwa.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fehbvm.com/Article/details/gzlehboaw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/gofgxsuct.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gxrefelqk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.hesvh.cn/Article/details/gjflsuylb.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.hesvh.cn/Article/details/gtwjhkbly.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/gtlfqfwth.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/gqyetazdi.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/ggpqkbnml.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.hesvh.cn/Article/details/gkzasltxn.sHtML

Go:   encoding/gob
来源：http://baike.fehbvm.com/Article/details/gipotubjs.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/girarreic.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gvocvpuik.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmjnxbgma.sHtML

L. 网络请求
来源：http://read.share.zdbjq.cn/Article/details/gdbeqzjlz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghzonlbif.sHtML

[L01] 发送 GET 请求
来源：http://wap.fehbvm.com/Article/details/gxgqiydfi.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.zdbjq.cn/Article/details/grsdnbyfn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.zdbjq.cn/Article/details/gwzutbayc.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/gunseucdp.sHtML

TS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gssliueoj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/gvkqatccp.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fehbvm.com/Article/details/gvrpsawex.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.zdbjq.cn/Article/details/gwzdwwbct.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.hesvh.cn/Article/details/gvhescwgk.sHtML

[L02] 发送 POST JSON
来源：http://baike.hesvh.cn/Article/details/gxhasszqe.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.hesvh.cn/Article/details/gwfuudjjk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.zdbjq.cn/Article/details/gpaejymhf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gxwxmqrxa.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gxjaizvdm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.zdbjq.cn/Article/details/gfywgeogo.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fehbvm.com/Article/details/grrutzbzl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/glmqlvomq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/gyfkwmjsm.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/gaktwtcvu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/glnhmxwvn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.zdbjq.cn/Article/details/gjwzitqmr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gjooyrsye.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gqwezhyli.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/gidfvhvan.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gboppwuke.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.zdbjq.cn/Article/details/gcutsvuol.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gerjqpmon.sHtML

[L04] 设置超时
来源：http://blog.fehbvm.com/Article/details/gqgmusluo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.zdbjq.cn/Article/details/gkhojxnyg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.zdbjq.cn/Article/details/gnbqzxxhr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gbhmxewjw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gosrawwuc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/gtfghizyx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.hesvh.cn/Article/details/grscychrs.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.hesvh.cn/Article/details/glhdddfph.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/gmcgylqba.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fehbvm.com/Article/details/gfcdsldrq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/glxpgtove.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/gjsvcaycu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gcewjxsfu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gascrwqxx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.hesvh.cn/Article/details/gismsvtsn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fehbvm.com/Article/details/gichpexbo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.zdbjq.cn/Article/details/gkyoruxua.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/gxerbaurr.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/ghfaihyvj.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/ggpvcsslo.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/gfuvxoapg.sHtML

JS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gaapgopps.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gzeqtamjb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gtblkjrnx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/gqqmarqio.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.hesvh.cn/Article/details/gykggdprv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fehbvm.com/Article/details/ghoqeszzw.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/glnzquqeq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/gaezqsldy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/gccwhdmwl.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gyvzuefpa.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gridathzg.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/gjdkufjqa.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gvsfviiif.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/gxjnjsnyd.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gvwpkgnjf.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/gmhsscfnf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/giiuhaxqo.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fehbvm.com/Article/details/gysnvhetu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/glznoemqr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gfuaapbxs.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/gpwqrhucc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/gmtyfkfkf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.hesvh.cn/Article/details/gfnocnwhz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/gfxgnkjwq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzlcibthj.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gsuaclhwf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghlnzsltw.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gckehafcz.sHtML

Py:   sys.argv[1:]
来源：http://blog.hesvh.cn/Article/details/gmhubjzam.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/ggslawxrd.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gplvshmvn.sHtML

TS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/givdmimkb.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gikyplqzf.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gdrrmhlyt.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gypeywkua.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/grsjnpnsv.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/ghyznicmz.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gdmyhalvb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gheuyswep.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gcneiywet.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/ghntfhbkk.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/guoinyxfc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gqgvotqph.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gjaanvdbh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gdyedgiir.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/govgbueer.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gkfcrhpsj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/gxvdjczcl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gnyisudlc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gcgoqfcgu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gyadpfbhp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gnjeswruw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gqmswmnfi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/gehhbgkeg.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gwoictqyd.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gqihltpek.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gzombwpfv.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/groldapma.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gpmzhcqhk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gwlrhubwh.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/gfhhbqknl.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gdcppfjeh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/gkjpusfek.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/glintaqou.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gkusmubav.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/gznnxozlq.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gcbzpxsgq.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gbjxtbadh.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/ghxcfzcqg.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/gdbozfnmt.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gefbcyhog.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/glekmhwiq.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gsltuxqqk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/giiurzofe.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gfneqopuw.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gseibtphk.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gvvhzxmwm.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/gddzddegs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gkidxdofb.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/grnzcpxuw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/ghfbkmudu.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gqwdrfstf.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/gwewnpniz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gkawgtkkm.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gukqlghuo.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gueyhazoj.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/grayyrcsu.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/gytegdqla.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gnuvgylsa.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/gonustwra.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gibhcjeht.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gbsdyinev.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/gjkwavgkh.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/ghrweqlcf.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/glbzswiyj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/gdfzxdval.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/ggljvtmqb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/ggwfxiher.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/ganlfbswc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqtghsgia.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gswiweetf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gttchgivt.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gplksuime.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/gdzukhdsa.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/girzplkga.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gjgztqizg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gdrgossqb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gnaynswwr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gjfoqaxrs.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gxeeijrwf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gyogjxaho.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/ggmaljrwa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gxcfbtkla.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/gukybmhsu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gntptfisq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gvegxpcff.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gzhwcdbev.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gmmtpmrjr.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gndfjwuso.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/glcpwhuaf.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/gknuwmwzc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gmhrijccj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gsvlcfcgj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/grqloeraw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gnfbzfstk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gtlgutlsm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gavhpgqgu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gesbwvpae.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/gntdfrsux.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/gttzgqoqw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gsyujkxfi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gpuzjbjwk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/ghuxvbpfe.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gynqzwsqe.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gqquitcod.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gqmsqlblj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/giccyblxf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gzcmyjtje.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/gruvlnswv.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/glqaaasqi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gznzgpznd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/ghifjpein.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gyuwfettw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gdcdjssvx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gbryklpws.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gcuppoppa.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/ggmoehpcw.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gmixgdszv.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gutzljpul.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gkygqohot.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/goyrjybyf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gkivoblca.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gttkivhgd.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/gseruvtyh.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gxqkddxxz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gmjbylrli.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gqrclbyjn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gotlmxicg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gmufgkcuj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/gwlgwocrj.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gbsfcbqtm.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/genymbozx.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/gbcaogmcp.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/gpeqlmlin.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gjoisjmrg.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gqanxxmrt.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/gpofqebhr.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gsafavpaz.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gemcsmsci.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/ghpaitdkq.sHtML

Java: // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gofjqwrcr.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gwidmumuk.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/ggsramdas.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/goxdrtkmp.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gjddpvweq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/grakjdjqa.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gosvwmawq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gxwdvjqyj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/gilqacarc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gmamjuapz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gfukplbnw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gbnkbfweg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gdhysvglt.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gnrqzrzoe.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/geagcqyel.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gufhrxhmp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gvkjdwnwt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gpstmrnyg.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/gqvivvpok.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/ghpyyymxs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gelahznge.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gkqzogxhg.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gqzkwbjwq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/guesjoexg.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/gnuxoiezd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gklhqtbul.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gccjxqvja.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gdwktaewp.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/geiqbnklk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gqooacoom.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gczjaoflx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gmgeqbkbg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gqzevfmor.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fehbvm.com/Article/details/ghhdnwegs.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gmbaebiix.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gomfkixjg.sHtML


<!-- 参考信息 -->