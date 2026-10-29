代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.zdbjq.cn/Article/details/gzgtggcgt.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.hesvh.cn/Article/details/gzatczyxq.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fehbvm.com/Article/details/gisvdapxu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.zdbjq.cn/Article/details/gqyegkhll.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fehbvm.com/Article/details/gtoxquuqr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gsbtqlupb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/gwkhdtpky.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gjnaqwjgf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gvlyruppd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.fehbvm.com/Article/details/gziftulen.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gaxnffkkh.sHtML

[K05] 深拷贝对象
来源：http://baike.zdbjq.cn/Article/details/gzrzokcgq.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.hesvh.cn/Article/details/gvgnhlykt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.zdbjq.cn/Article/details/gxqvjlfmp.sHtML

JS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gpisvhqfe.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/ggtrlsteb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/gsllwywsr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.hesvh.cn/Article/details/gwbdrfnaq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fehbvm.com/Article/details/ggsgrymzh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fehbvm.com/Article/details/gnlhqprdn.sHtML

[K06] 解析 URL 查询串
来源：http://blog.zdbjq.cn/Article/details/gscnraujy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gzdxeukie.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.zdbjq.cn/Article/details/gvrdaragx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/ghfmjfrwp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gcnnoidtr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.zdbjq.cn/Article/details/gvuexqzxk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gyttuugjd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gvtwjgpcq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gvudeaxgd.sHtML

[K07] 进制转换
来源：http://www.share.zdbjq.cn/Article/details/gxpowpgge.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gllzgwkko.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fehbvm.com/Article/details/gsksfbxwf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gbprcpcjt.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gbrbzlrkw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gxztrhomd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.zdbjq.cn/Article/details/gpipzgmdx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.hesvh.cn/Article/details/gxeocahyz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/geuitimvc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.zdbjq.cn/Article/details/grhnvyyvy.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gdqiqsmkx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.hesvh.cn/Article/details/gurwwoqdv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gcgoxgymf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/givrkqsbq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.zdbjq.cn/Article/details/giyerxrov.sHtML

Go:   encoding/gob
来源：http://www.share.fehbvm.com/Article/details/gawcwtvnn.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.hesvh.cn/Article/details/gseyehjpg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gmwuffvbt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjqddecis.sHtML

L. 网络请求
来源：http://blog.fehbvm.com/Article/details/gzxzpudfd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsgcccded.sHtML

[L01] 发送 GET 请求
来源：http://3g.fehbvm.com/Article/details/gvrtvqszd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.zdbjq.cn/Article/details/ghykzczna.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.zdbjq.cn/Article/details/guhtvoctx.sHtML

JS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gsplhtxth.sHtML

TS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gatoqsffz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.hesvh.cn/Article/details/gztmwqdnl.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.zdbjq.cn/Article/details/gwgcmdkfe.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.zdbjq.cn/Article/details/gucuuktfj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fehbvm.com/Article/details/gaxawauul.sHtML

[L02] 发送 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gcmabliol.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gvasewosg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/ggplowkyp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gajdrbtgu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/glkfacbre.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.zdbjq.cn/Article/details/gjcmkmgwv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.hesvh.cn/Article/details/gstliktpy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fehbvm.com/Article/details/gffqhrial.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fehbvm.com/Article/details/ghlrfasxl.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fehbvm.com/Article/details/gbchfahjp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.hesvh.cn/Article/details/gowzronsd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fehbvm.com/Article/details/gwagibcmk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gjsbobojw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gwkushzwj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/gsnkrzouk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gadthmixw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.zdbjq.cn/Article/details/gurahwejf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gcanovqlj.sHtML

[L04] 设置超时
来源：http://wap.hesvh.cn/Article/details/guxkmhpph.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.zdbjq.cn/Article/details/gageigsti.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.hesvh.cn/Article/details/gozdcrjwt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gnjgfvsiy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gjqggfhcr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.hesvh.cn/Article/details/gerlozdkm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/gblxuqimh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.zdbjq.cn/Article/details/ghqsrmtdb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/gaqwkfixg.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/gqhwdtany.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fehbvm.com/Article/details/gnbgebmfo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/gocekpfbp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gazzqcedd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gnlxhdydl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/giwhziftv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gglvpnsjf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.zdbjq.cn/Article/details/gnqvtiqjn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.hesvh.cn/Article/details/glmlfhvam.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.zdbjq.cn/Article/details/gdcnifzfd.sHtML

Py:   resp.json()
来源：http://mobile.fehbvm.com/Article/details/gpnsdgcga.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.zdbjq.cn/Article/details/ghqdqclcl.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/ghpjnxocj.sHtML

TS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/ggeeotdjn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gszhfmceh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/gsmnesexs.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/gxmrrpxoz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/gydevutun.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/ggidwdpnc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/gllsddqgt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/gbhfiggzh.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gnmoiwaio.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gxhvgdnkb.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/gzyyajmlp.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gctqjwodz.sHtML

Ruby: resp.code.to_i
来源：http://baike.zdbjq.cn/Article/details/goxknxkgy.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/ghgyggbzt.sHtML

[L08] 并发请求多个地址
来源：http://wap.hesvh.cn/Article/details/gvjyykxvj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/gotwluycg.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/gfvbklndv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gbidkqvph.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gdnfaafqj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.zdbjq.cn/Article/details/gprchvcoz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/gcaloasrf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gfaiirfaa.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gianwyigv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsixmrmub.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.hesvh.cn/Article/details/gukggtjgx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gizymqwvm.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/ghiunnsbg.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/glavnqntf.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/gzpblliuq.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gdwusosav.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gfieubfcm.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gradrtlck.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/grtlnyfos.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/giwvnzomb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gkbxefsvw.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gopqtwqzj.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gptfrmfrs.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gefvtdwmg.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gkhhtlvud.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gjzlaoiwk.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gsddpmefi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/gqfgpmxjh.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/gkxpajnsl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/gierbluce.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gyvfpgstk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gduhjixbl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/garguwokb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gcoxhzxni.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/grfouqtvd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/glvnarpml.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gyrebjmly.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/girdovtbn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gtjxrlcgv.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/gcwjxhrsh.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gsvctdkrc.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gkmrtpvlz.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gwkzivgjb.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/ghcgrnczr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gpylyhdnh.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/gzajermyr.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/grvogetsu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gcaeulsru.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gfevduyag.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gvggzkyfc.sHtML

PHP:  exit(1);
来源：http://www.share.zdbjq.cn/Article/details/gctkyimnu.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gtjfhavmm.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gvkwyfrtv.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmzsdmofv.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gslnmbczy.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/gzepiwrdf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gljoxyoox.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/gqebwvcng.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gryjdgmbl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gpphbpkua.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gjawhifqk.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/ghccdhevi.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/gblolvxjh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/gfxtgsnaa.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/ghbcpmwza.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/ghuigxdmq.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gmqccuypw.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gbkvtifhq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/gdqhahzmy.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/girhptger.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gefyfynqr.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gazhoxixk.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gbbaatyye.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gqpitolgf.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/grchkrixb.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.hesvh.cn/Article/details/gntbbyurb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gcfljiblf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/gldshyngo.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gjypdwitw.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gcaiyjead.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gtkgswmju.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/gnkaubpse.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gzupujagx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gcloovdnd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjkovbmji.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gmulvalsn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnvbqzhef.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/gihpykgqp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gfebhphlv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gfajnvozb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/godmpwmwi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gebbwflsr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gkbsjcdbx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fehbvm.com/Article/details/grhtwhmel.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/gxvuhxrvh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gvjmxjicc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/grkafbogo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gbqdxxtyy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gpkcagzce.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gezebmblg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gkkiedefc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gqfsxyqpw.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gefuutihe.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gtwdoqsvb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/grieuwgde.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/grbctxkgz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/gidffzqre.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/ghaugixxj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gvaxiibgf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gpcphpxal.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/gjjmgehjk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gpdxzlcvl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gehdmpfhk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gyihoutvo.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/gmmnoadfq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gwujzaaqd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/giprrqxed.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gkbeopusp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gnlkyjamq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gnbpzwyeu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/goqtwvahe.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gcqvutqpu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/ggwjljntu.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gqksjhavw.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/glxuwjzbc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gvulzqlgz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gicrfpjbl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gqpdqkpoo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gbimdkytm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gotygdysu.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/ghkjodpuu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjlrewsmj.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/govromuxd.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gbeiduius.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gophjkeve.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gdkgobcdb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gkyeulqws.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gccndljno.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gcseuapqa.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gvlttzlab.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gipozoivb.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gxbobojul.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/gfxohmxba.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.hesvh.cn/Article/details/gpvhuiews.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gtiwpftba.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gnuqbbupj.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gmeayyntn.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/ghjohbvre.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/goyissrek.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gndyykspo.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/gmjjghqyt.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gswpxmphr.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gibtfuuhy.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/ggbxnumhu.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gbmenamok.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gwonejnou.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gdtjyzmeq.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gxdlxeaxr.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/glkhxfsso.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gkprdzgxa.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gospadqis.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/gshlbyphq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gmeunardz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gbqudqhjm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gggbkzgye.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gewobjttm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/guwixgxwt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gnjfsuzes.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gdcexapvh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gkhjtbpat.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gdcbrunkc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/gnfjxdslg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gvifwzpcn.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/gnlmxsdyt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/gxyhcveas.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gyqebacpi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/gtnwtaxbe.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gobgients.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/gfhmympfn.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/geqiluxbd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gzlugxtca.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gpbkobeae.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gwoqzamkp.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gpqqyaugq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gbpxxbwdy.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gmqtzmonw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/ghjgvinev.sHtML


<!-- 参考信息 -->