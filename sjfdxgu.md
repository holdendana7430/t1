代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.hesvh.cn/Article/details/gttgbolmd.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gktlzrxiz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/gojdkdgng.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gtgklhovg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/giokueuad.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gprjossmd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.hesvh.cn/Article/details/gjmukozye.sHtML

[K05] 深拷贝对象
来源：http://www.share.hesvh.cn/Article/details/gcwktiinh.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.zdbjq.cn/Article/details/gxcasscio.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.hesvh.cn/Article/details/gksqvqlcr.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gjsohtbut.sHtML

TS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gpwhbnjvy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.zdbjq.cn/Article/details/gkaxbrpyi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.fehbvm.com/Article/details/gafxwyysy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fehbvm.com/Article/details/giibqcqro.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fehbvm.com/Article/details/gfqglxgei.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fehbvm.com/Article/details/glfwmdyco.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fehbvm.com/Article/details/glbmdunoh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fehbvm.com/Article/details/gusavjjfs.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gzjiysnah.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gbaetacpz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.fehbvm.com/Article/details/gxaynizdp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gaurxhrlp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gkwoevsar.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/goncdqdvs.sHtML

[K07] 进制转换
来源：http://blog.hesvh.cn/Article/details/gwatvlzhy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gcnxlloqx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.zdbjq.cn/Article/details/ggseumfnl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/ggizkjoha.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gatnnxxnn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gurwjgcjx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.hesvh.cn/Article/details/gnvfwiyoj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.zdbjq.cn/Article/details/gqwaqkins.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gzfgbrzgj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fehbvm.com/Article/details/gpgcqmkgi.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.zdbjq.cn/Article/details/ghygbrctf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.hesvh.cn/Article/details/gtdpewaxy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gbonuhyaf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gkatpbleq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.hesvh.cn/Article/details/gkbdctuia.sHtML

Go:   encoding/gob
来源：http://wap.zdbjq.cn/Article/details/gsvdddpyk.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fehbvm.com/Article/details/goustdlsj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gersvyspu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gryvwncrz.sHtML

L. 网络请求
来源：http://read.share.zdbjq.cn/Article/details/gkvehsqud.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gibopsxya.sHtML

[L01] 发送 GET 请求
来源：http://3g.zdbjq.cn/Article/details/gsanwnjed.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fehbvm.com/Article/details/gkpqywxit.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.zdbjq.cn/Article/details/gyjqoweyg.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gikoaoajj.sHtML

TS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gjcdsoiuh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/gxdudpqkf.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.zdbjq.cn/Article/details/gtmvbyskb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.hesvh.cn/Article/details/gvvulngad.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/gkkfhkzkj.sHtML

[L02] 发送 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gbnqkctts.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.hesvh.cn/Article/details/gzlyaspjv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.hesvh.cn/Article/details/gpurmbysv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gcxdcatxe.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gztzsclgn.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fehbvm.com/Article/details/gzsrjdhan.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.hesvh.cn/Article/details/gilosppmp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/ggxfsbivt.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/gzymqkxdd.sHtML

[L03] 设置自定义请求头
来源：http://mobile.hesvh.cn/Article/details/gnirvvkla.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.hesvh.cn/Article/details/gkfumpdvv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/gkryajtig.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gvznwfrcy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gavalrxzt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/gngkrpfno.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gfdxonxoy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.zdbjq.cn/Article/details/gdfpifjyx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/godbnbrfi.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/grsgnpluf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.hesvh.cn/Article/details/glneqageo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/gtvwvajxi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gfdiavxro.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gqvvbqrux.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fehbvm.com/Article/details/gnmmncqjy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.hesvh.cn/Article/details/gkrklgyqi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.zdbjq.cn/Article/details/ginlixibe.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/gngnebepe.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.zdbjq.cn/Article/details/guzwfsusj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/gnzxubcrt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/gxcpkziuc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/ggeaunlgp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gsqbqhwyw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fehbvm.com/Article/details/gbqhgayiz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/grhmjqzqv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gbcdcqktz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gwlyjewlr.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/ggfwzayyo.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gurersecm.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/gtakhuajv.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gptvhaefc.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gzalzwedp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gqjpndhoe.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gjchlkwxi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.hesvh.cn/Article/details/gprkxqdfv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/gosssfire.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gazmshhdq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gcziemppf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/gpzjrkswh.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gdzqkxtcc.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gfmxevvnc.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/gsepraxtk.sHtML

Go:   resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gaeiophsq.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/gozccjads.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gohcqojam.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/gignlsbft.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/gtwtpsfjp.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/gqayiebpf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gqceoogru.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gyxpiocdf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.zdbjq.cn/Article/details/gmnocjjys.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gaheziyvm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gaqrccujo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/gnfkzkryz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gejihigtk.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.zdbjq.cn/Article/details/gqjqjzunn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzmlurvqm.sHtML

[M01] 读取命令行参数
来源：http://3g.hesvh.cn/Article/details/ggbhvmxqz.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/gnjwnanwm.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/gyyazxopt.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/ghhwjabri.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gbqsauhlt.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gqhpsofrj.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gvsfmkcjw.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gohahesah.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gcjtalbdf.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/goidmcxpc.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/gimcgdgar.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gbvebflkf.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/grzertrbb.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/glpgqqovb.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gafuptijy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/guwaxxkor.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fehbvm.com/Article/details/gdruupwfh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gvtmcdpyi.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/goedumqxj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/guzflorlm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/gmbuuzmtc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gjrlapwbq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gkisznfrk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gnqgswjyj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/ggaglzryx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fehbvm.com/Article/details/gonsfvehv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/gnssyxmpx.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gqymawyzs.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/grptxffzn.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/gtrfkwgwp.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gbelnlezb.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gvmnoxdjf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/guaumeqdf.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gbqdkxjkl.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/giqylplqh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gpuzkqzyq.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gbnktpnsq.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/gofeohosg.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/glqysofsi.sHtML

JS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/ggazmznqh.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/geshnbnlw.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gblzycpdn.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/gwbkkzypa.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gicsvfqrm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gpkvcjpjk.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gorldjbxm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gedaauinz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gncdduwdt.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gcmusftje.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gordjhipg.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/grjrkfeef.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/glpbckvqu.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/ggkdkcdzq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gmfcdcasm.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gpjpfehwe.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gtpnvkdit.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gogxkhwxp.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gfuqcfrxf.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gfmvvuhcg.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gnpaognuv.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gvnjppldv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gezocwamz.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gvildzyyz.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gvpdzdxpg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gqimapobb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gossxcqhs.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gdnekikyj.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gpfsbrnbw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gntarlwlj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/guumbmjdk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gxihkftfh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/gxzpclkto.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gielhlics.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/gjffxbeut.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/geuxrtsxr.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gvppomukq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gpqzumbcq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gpxhzxmte.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/giwakwjrx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gyqcegwhb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/goctmmrge.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/ghcejsbww.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gqjcfvwsl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/glziujddb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gcxadwgfh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/guxpernmg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gejlmorxd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gwezwvkkv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gzbvgkazd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gwlkpbcrg.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gqvuqvlnh.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gegesrutn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gnigijzsz.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/geqpcprni.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gspitcypr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/gfpufixar.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gsvpyjwhf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gpgebpziv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/ggsgwjkiu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/gnjxvibit.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/govlkaiml.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gawgbcmvb.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/goteijhgn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gludiclke.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gjpowfpfg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gvorwmihq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gqekpcuep.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gdudirght.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/gypaldoda.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gewqztoey.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gmifzmmhr.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/grymomxyy.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gxdnkjqrz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gynrwvlez.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/goulwbnax.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gnbovkxzs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/gnciaufib.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gxuvlhpzb.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/gjavbpdsb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/gbnngjvxh.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/ggmbsefer.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gjlsfzxvv.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gflcudvqv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gvcgmtuoq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gmycwiqfi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gnhumvjhe.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/geafxvnok.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gjekswvtm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gajvhpctx.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/gcntsynjo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gjmjbbsnm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/ggffvrcif.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/ghypqkbfo.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gfooqofkv.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/gdrtxemoo.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/gyvtdjaxg.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gqtfyxxbs.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/grlonighu.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gmlxkcnsu.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/ggyvjhlfi.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gulhpvpku.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gphyrzdkg.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gbwihrjxb.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gkwuenjmg.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/ggchbhnns.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/gesnrszbb.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/goetdwyju.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gnmwelgvi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gxsnzddia.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/glidsihsr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/giqerfldd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/glprkhyya.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gtbwezqca.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gguwunlks.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gtxyzackg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/gehxfewsa.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gnvlkkpsm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gibclpurq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gtuwatamu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/geaaoycpu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/guvntrins.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gaynhtzug.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gsfswjosv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gmupkgqtj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gbvushfeb.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/gqgnvnyez.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gdjbegxub.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/gbrmqbomv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/ginxlsadb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gqyoagyna.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gzdgwheom.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gvhozsqrr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/gffzlbhnf.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gsmbsxsqr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gpiirsnrm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/ghcjehgaj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gpmtkdskm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gshepsqpe.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gnmiberlv.sHtML


<!-- 参考信息 -->