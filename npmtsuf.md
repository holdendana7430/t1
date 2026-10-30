代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.hesvh.cn/Article/details/grxfufqqa.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gqccvqtuu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/ggvacxtvk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gzbsqolmm.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gvvvlcypf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/grwtcwpnw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.hesvh.cn/Article/details/gpnqyzkgl.sHtML

[K05] 深拷贝对象
来源：http://www.share.hesvh.cn/Article/details/gzdemcjaq.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.zdbjq.cn/Article/details/ghfhyhlcz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.zdbjq.cn/Article/details/gxwadyirz.sHtML

JS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gfyhjztqk.sHtML

TS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gshffuvzq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.zdbjq.cn/Article/details/gbfgobfbx.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.zdbjq.cn/Article/details/gmdztparm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/gdscbfmla.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.zdbjq.cn/Article/details/gfhmvuyyi.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fehbvm.com/Article/details/gvfgdefpk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fehbvm.com/Article/details/gkbojaljx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.hesvh.cn/Article/details/gvssaldid.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gdhybisef.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gomfmmweu.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.fehbvm.com/Article/details/gqdpnjenn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gzohqeagy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gnoynzbgy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gathervex.sHtML

[K07] 进制转换
来源：http://mobile.fehbvm.com/Article/details/gcqzcxqcc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gacmepphq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.zdbjq.cn/Article/details/gglecypvy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/ggcmlvtll.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gtnmwrody.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gwvxqqqot.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fehbvm.com/Article/details/gssnheiof.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fehbvm.com/Article/details/gumvxptss.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gvvtvovrx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fehbvm.com/Article/details/glullgldk.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gpigjcdeb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/glspjtiwn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/goxawmfof.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gwnvpmcco.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fehbvm.com/Article/details/gtadautye.sHtML

Go:   encoding/gob
来源：http://wap.zdbjq.cn/Article/details/gnhzkbiaa.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.hesvh.cn/Article/details/gnowsfclp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gwjjrumvc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gaflkizkt.sHtML

L. 网络请求
来源：http://read.share.hesvh.cn/Article/details/gouimfuon.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/geiwxigsz.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/gybdqbydp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.zdbjq.cn/Article/details/gkxdzjdgy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fehbvm.com/Article/details/ghpuplyxm.sHtML

JS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gnmnbctbm.sHtML

TS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gvaykbjtl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.zdbjq.cn/Article/details/gotabtfty.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fehbvm.com/Article/details/gsswahici.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/gxmmgueic.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.hesvh.cn/Article/details/ghcirlzwz.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gbassdcev.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gabgnsnkn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fehbvm.com/Article/details/gpzruunzs.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gidhagupc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gjksqqeot.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.hesvh.cn/Article/details/gtxuygdlv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.zdbjq.cn/Article/details/guuulgzxe.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fehbvm.com/Article/details/ghpdlymcn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.hesvh.cn/Article/details/gudzctium.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/gatrpsmek.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.zdbjq.cn/Article/details/gofjzzwza.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fehbvm.com/Article/details/gfwfyhpxo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/ggpzrrmvx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gzhrbwjed.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/gydjqriun.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gayonxmvn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/gvkbyozyd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/ggkckduyw.sHtML

[L04] 设置超时
来源：http://wap.zdbjq.cn/Article/details/gdjooqyip.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/gxrgonvsm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/gfgxsvpdg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/grplvsbpi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/grywhdjqk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gqdclgetk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fehbvm.com/Article/details/gfnduhwrg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/gpsqjozfa.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/glpunnzjx.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.zdbjq.cn/Article/details/gkoodtkzv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/glrtbsabj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fehbvm.com/Article/details/glkniipbe.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gdskpzhvz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/graorujhg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.zdbjq.cn/Article/details/gkeloptuw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fehbvm.com/Article/details/gwwfdozyt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.zdbjq.cn/Article/details/geisqkxrx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gglcfltto.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/gtnscnwlb.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/giaphqpua.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/gnpndwdbd.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/ggylxobvf.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/grxbtbdnj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gsymbsbgj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/gaaspupow.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gthhjxnmo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/gjlbzcxca.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gdjmjqbdn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.hesvh.cn/Article/details/gexkdfmcm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gwstsuzum.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gygmyarye.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/ggcjkkdzl.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/gkvqpzwzf.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gtqgxbmpg.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/gdrlecybr.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gdcmwwvxf.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gpjqsdslz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/gxuhuwpre.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gfufvucvl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gwwfthrqq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gufpiwzot.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/gxvyfeyfc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/ghyncyure.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.hesvh.cn/Article/details/gnjdfxltf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/gvgzagfln.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsueupeci.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.zdbjq.cn/Article/details/gqnmyhzeh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gicvqmxwf.sHtML

[M01] 读取命令行参数
来源：http://blog.fehbvm.com/Article/details/ggcjmuxdh.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/grwbnlxla.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/gzvstlfqp.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gasqnsugq.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gyayblzej.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gqydazpvd.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gaatqqdla.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/gewxmnfro.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gimsimoqq.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/gtosknpyi.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gdxoyytvb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gkpbdhcpd.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gaexinsxq.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/glckalxeb.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gajljxxxu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gvszasoju.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gxkdlbnia.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gdcnlvcaz.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gabstcwdy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/gnistfmvu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/gijdgqnun.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gxzhzeewn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gdnwkhezh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/gwfmmohog.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fehbvm.com/Article/details/gaivwcfyg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/gdpknausa.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gzggxrcil.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gqypttqoe.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/gmwrkgvyc.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gnrqcqdfq.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gkplfrhgd.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gtkukpmso.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gpiggvilf.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/ggyzghxfq.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gwcjeibxs.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gasvvdqjv.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gzoqruisu.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gijmfkekx.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gtfeoelkn.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gmztgvgcm.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gakoxwtnh.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/ggpyuysco.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/glbkvdkxi.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/giwxejxug.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/gvpsanerb.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gtiwdbvak.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gjccghlkr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/gfnwxnxdn.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gsfcwevog.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/ghrqlxhpm.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gdnhqiczf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/grldkxxvj.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/ggrqzcbmk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/gnschpnww.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gfrlecoof.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/giqekgbkr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gbvafdgak.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/glltsvikc.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gqgpmabve.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gdfzjeekx.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/grdelzkvo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gabqavwbu.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/gtbtdgpbl.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gwlldnvpi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gdpjbelfs.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/gmxaufatp.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/guurgfcig.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gsjklkbsy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gembcoinr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gtiyccvnr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gwvderxrd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gvvgslwfv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzftoifal.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gezswqfju.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/genxmtztv.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gxihtvcsi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gvzhxsnys.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gbnjjrklq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gpbpzjyro.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gvswfkrpd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gypfufrrw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gwjyfeuet.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gwudpofpu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gskytmxpx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gqrzuvkux.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gfjkoiouq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gjvyzopxj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gzyotphen.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gowckzzmd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gvhfhzooc.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gjrprtmty.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gezcoomvs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/gbcohwexr.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gofeoytkp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/ghvvlrwid.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gwigtuizd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gaxtfccmz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/grqolhnye.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gszjukhap.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gdveeloqc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gzpottjeo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gulgqigau.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/gurzvdynb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gagwkdpwn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/gqlsjkswz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gvfrfbcwu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gezahsalu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/gfdwmttqb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gsbfhmksp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gutnltzba.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gmphfccwx.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gfwgghfbz.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gfbzfxyzp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gnheceukz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gtgyjzbwo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gxzkojtzx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gcsjifvxi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/gzmrxufju.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/gsrmlzvoi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/grcjjamcr.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gomwnpwnn.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/gpsijohup.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gzjgwttgx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/ghcyuyzzs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gffibxuhk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/galzkzjmh.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/gqioffsur.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gqzikcana.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gmindqtsp.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/ggqlfgpxf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/gxfpzmmil.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/gzoofmdif.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gaguefevr.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gvuhhbyvp.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gwleoxenv.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gxddnifpd.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/grjugafyx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gtpisxqhv.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gwjvdrori.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gorxtrfny.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/gnrsmccxn.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gdbcchidi.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gabkjmlhi.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/ghtzwckmc.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gphxfkkzv.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/ggudikzyh.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gstqjhnpj.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/gyuxeirnc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gdfwmdiyx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gmflomtew.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gmsqtpkxd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/gbksjnmfk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/gugzeepeh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/gcyyllavh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gtxbjtudx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gyrmqneet.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/gcnceovty.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gstllooan.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gfhlivxxd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gscedhcyj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/gbtyyjzxq.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gazlaljrw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gzxnvdrox.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.zdbjq.cn/Article/details/gfsrfljgw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/ghrxncway.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/giqvxsdyg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gjeivyycb.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gugaxmqzh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gdvlcxpkh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gskztxmpg.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gncmmqhxh.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gddozwurn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gqyhvadvd.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gqxyaqmra.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/gummfvwzd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gvfrorhfu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/gewxparze.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/guubncgfe.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gpvjbqjpr.sHtML


<!-- 参考信息 -->