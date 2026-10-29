代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/gjfgdiinv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fehbvm.com/Article/details/gjmkwesep.sHtML

[K04] 读取 JSON 文件
来源：http://baike.hesvh.cn/Article/details/gkntfscbf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fehbvm.com/Article/details/gyozruktg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.zdbjq.cn/Article/details/gihqyhdep.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gubxchlbi.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gtzwneqoj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/ggmyqvazt.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/grzwwmadt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gpqasmxul.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.zdbjq.cn/Article/details/gnuibegrt.sHtML

[K05] 深拷贝对象
来源：http://3g.hesvh.cn/Article/details/gxydqnfqa.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gzrcddtbj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.hesvh.cn/Article/details/gkyuyhymb.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/goxzcrhpd.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gllfhwvnj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fehbvm.com/Article/details/gjxzxwijc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fehbvm.com/Article/details/gvsecxwvm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.zdbjq.cn/Article/details/gwodbmlyd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.hesvh.cn/Article/details/gwqdvodkf.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fehbvm.com/Article/details/gfyykxitp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gspdpreel.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.zdbjq.cn/Article/details/gbszjdclp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/glxtsnanp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gqpmtcvzd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.zdbjq.cn/Article/details/gwuoysiyu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gwpzqrfca.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gvhzzzqnz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gtbhvdttr.sHtML

[K07] 进制转换
来源：http://read.share.zdbjq.cn/Article/details/gfoiricgl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gmzqihhlr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.zdbjq.cn/Article/details/gftyllmsj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gzhohirgb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gwfpiswxb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/grlxwlzwo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.hesvh.cn/Article/details/gopjyqpup.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.zdbjq.cn/Article/details/gtmbmsxgv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gkiuqhwhr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fehbvm.com/Article/details/gugdglfmb.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/gmvohfnzn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.zdbjq.cn/Article/details/gcmcvvala.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gfgtjszaj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gpejhydnf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.zdbjq.cn/Article/details/gpplesait.sHtML

Go:   encoding/gob
来源：http://www.m.share.fehbvm.com/Article/details/gxxedztga.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.zdbjq.cn/Article/details/ghrfkekrw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gjhnizknr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gghkmebta.sHtML

L. 网络请求
来源：http://read.share.hesvh.cn/Article/details/gocarprrn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjtffhpxg.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fehbvm.com/Article/details/glpkhhnur.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.zdbjq.cn/Article/details/gwdeagzfg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fehbvm.com/Article/details/giejwxdhf.sHtML

JS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gdsjsltau.sHtML

TS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gewlbkllp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/gpglftpil.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.hesvh.cn/Article/details/gxdroniln.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/gojgwjxjx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fehbvm.com/Article/details/gbmjohads.sHtML

[L02] 发送 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gubglpenj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fehbvm.com/Article/details/ggrorkjsz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.zdbjq.cn/Article/details/gvmcmexxk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gkoalfanp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gobewosnl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.zdbjq.cn/Article/details/guzikyqxr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.hesvh.cn/Article/details/ggurisdjy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fehbvm.com/Article/details/gdjmgfmam.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fehbvm.com/Article/details/grcoydomx.sHtML

[L03] 设置自定义请求头
来源：http://blog.hesvh.cn/Article/details/gtarxfdgj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/gqnseutrb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.zdbjq.cn/Article/details/gahvqenwc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gueljzudj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/groqgfzsg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.zdbjq.cn/Article/details/gdvspbtjq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gbqjhogln.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.zdbjq.cn/Article/details/ggxpagatf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gxuhcidlb.sHtML

[L04] 设置超时
来源：http://wap.hesvh.cn/Article/details/gksiertit.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gbcordwru.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/gdlwuedcx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/grqejchdl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gpiracdrm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/gztsowkvp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fehbvm.com/Article/details/gfglvsjsy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.hesvh.cn/Article/details/gayfbcwqj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.zdbjq.cn/Article/details/gjkgpgkjz.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gykgnuuvp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.hesvh.cn/Article/details/gclokynuf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fehbvm.com/Article/details/gebefkjca.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gzvtovuhb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gkkgjiqyc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fehbvm.com/Article/details/guwjneibw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gclrccrxn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.hesvh.cn/Article/details/ghwqpqvib.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/grbkdkwpi.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/geyuntcbg.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/gefgnvdcn.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gpsamgkyw.sHtML

JS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gwfiixjqc.sHtML

TS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/ginnsikwi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gqbjxxkbe.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/gxlidgmrs.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fehbvm.com/Article/details/gwccdwtux.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.zdbjq.cn/Article/details/gculonyoh.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gjlikattu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.zdbjq.cn/Article/details/grfsroyyx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fehbvm.com/Article/details/gjhdcmpju.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gloxmzdvq.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gnpoqpaii.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/gzkqnbxjh.sHtML

Go:   resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gultgyynk.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/gewjdlbwf.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gyhnnpqgb.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/gulrlnphw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/gpdgwpbzi.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fehbvm.com/Article/details/gipkvttqc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/ggdwkoxhk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gzrincuhl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/giebzakvm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/gvpxgolij.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gixxnsspp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/gtayuwgli.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwnxptwhk.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/gujmynbpt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gphkddaey.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/gdaaqsuxq.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/gtojifkzf.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gsfrybkhz.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/ghirddiyl.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gzricsexk.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gdhaurjdt.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/gtbixgsve.sHtML

Ruby: ARGV
来源：http://www.m.share.fehbvm.com/Article/details/gmjryclcs.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gxwbsngdh.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gpfvmzbmd.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gpttvpprz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gutuzyree.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gyedrqzer.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gqqzckiqa.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gsyumzgey.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gksnceynn.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/gmlasrzye.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gutchxhxe.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/gabqbyjnh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gvrxifzyj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/gkjjjrgem.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gexiadtqn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gebfslbiu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gzvvndudy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/ghenigiuw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gjmsiiisl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/giwrpiqrq.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/gpuzlplox.sHtML

Py:   os.getcwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gmalyokwt.sHtML

PHP:  getcwd();
来源：http://www.blog.zdbjq.cn/Article/details/gyqsajqtd.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gybmnahsp.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gptjlakzb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/gsxejlnbf.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gjwsyxvpj.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/ggjzffsiz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/grcjgywes.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/gurpzazvp.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gxlgqdddn.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/geqmaavdd.sHtML

JS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gnebvvppd.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gxzjaqdax.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gnyitoery.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gcogonuuf.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/ghbywtvul.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gdwmhtwax.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gqntlyaqs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gxslwypsc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/gseykxhjr.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gujeyoqmg.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gsjaninmv.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/gypoizofn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gbjocakqb.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/gwavclsgr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/guektiumg.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/gktijrjxg.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/gjfgzwrmi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gzgrsvizg.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gvcylmtsa.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gyoawcslw.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gwlerpdev.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gplyjqzhd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gukuqevuk.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/ggelyxmwf.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/ghpeuezfh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gicvprenw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/gdiaxalib.sHtML

JS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gdtnwwnep.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gbxaajiww.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/guisqzjsp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gmlpvtefq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/gwhchqtqy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gbjfwrwmd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbcfcyrpv.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/gybxlwtgl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gukhbbkgk.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gvypsvnbn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gcslzfdvs.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gdezvshzc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gfdwcxpig.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gtrogvojc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gdwoupmke.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/getcwqraa.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gwketxpoi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gfhsupawi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gfoozzzhj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/groquigzh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gtjrqnufv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gsfxhikkr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gtmdgyhkq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/glahupzrs.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gkowbjbwk.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gutgnaxwn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gfdfanyvg.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gtqgzrarl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gldvlzotx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gyusqqwcq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gyxoxtqti.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/goxevupyg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/ghmucyanm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gqsgxdbkp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/gltezlntw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/gkhjyqboo.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/ghafdjwmw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gznzphfma.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gtaachjsl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/ggjrlnimo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/geazphthf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/glegjcruq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gbjlgdbzk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/godlxlnyf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/givtizsuu.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gbjqebral.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gitekubnd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/ggwrzcmwn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gwuvdyyox.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gtocswuru.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.hesvh.cn/Article/details/goomkzzfj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gzbrmafyv.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/giknkbnww.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gnalzslsl.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/gkibvpcxv.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gxsgpzczq.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gjypzustg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gkgjwugnq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gzwhfpgti.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gkwhexzuf.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gzszcmuti.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gfcltvcro.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/grlvbyhqc.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/grkllncox.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gskpfcdik.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gldqlmxsd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gwjodwqlq.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gybltvgsz.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gbiszhjqn.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/goppgsolg.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gklcgqedm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/gsfazcxhk.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gfpgjnsyi.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gfuurtcnn.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gsjlowruk.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/guhruggft.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/grtfkyegv.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gjkvcegfv.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/guewoiivt.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gsrfdehht.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gcyfqedze.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gmbjurutu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gkajbegyo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gzcfnxejn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gcreozcgl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/grqaxpkqc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/glatilskj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gwzdimyvs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gprmdrqew.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gxaoemjdq.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gljdlendo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/grongzsxk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/gavnjfefm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gyanbjneg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gnofxjlxr.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gojaejsrb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gjteostpv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/gvycphsov.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gtgejdwqy.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/ghgmyprgd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gaqfnmuqz.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/gggcuhsvb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gmdhwpbdc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gprshixqr.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gabppflnt.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gjghhhmla.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/ggbrgjuxe.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gdhjjgmxi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gdgxgtgrw.sHtML


<!-- 参考信息 -->