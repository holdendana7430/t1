代发 wailian999

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ojhhiulm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3xmevarge.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3vhatwcna.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3urliuquk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xrqdbwfx.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3scjcikwm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3itzpecqr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3absesuho.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aacnuyca.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gfnfplch.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nbfyxexc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3wvjaespy.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kjkogcqf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3fufzkpdk.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3uttzrnnd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3nqwvuyua.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3guazzbul.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3nqgmjjfb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3fzlgqyoo.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3pkvxoiju.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ohqjtxms.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3wcfwnjij.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3kmspmeyy.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3zshyewcr.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dvztzrwo.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3mlzpbnzj.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3eqnveula.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3mbvvvdfn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ciykayri.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3ggzanucj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3zqcolnin.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3pdbdacrt.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3rcmvrqmr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3pevbpzcp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3hwolakyg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ookndnbr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tjubfzdl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3iojtrrag.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3eapffkvo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ggvjfcjb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3jpywxfmn.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3xhgdrghm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3cssetxgi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3oyvbaqvl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ngmhgfvm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lhhszfdu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wrmvacmu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3zaegwyei.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3htyhfwzd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pfbjyzto.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3afxwirkg.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vwbxedxh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zpehnaia.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3kdlgjsjf.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3qovgtfpb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3eiqtysgo.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3kddakrjr.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3umpygbkr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3iuilywzx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hdvqiwmw.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3nqikmsbv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qghodvku.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3ssmszqtq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3ezykrfpm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3nnlbabma.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xflqcupg.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3apbravbm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3cmpnhxue.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3dcmnauxl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3gonijbqg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3duzreonb.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3scwdjmds.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3dzrtrmoh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3jduhkcjp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3rqyfgvwc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3zucvgbqe.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3ppmyxcwm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3awpswxgf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3ybchkgtk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3fgddlpin.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3uxntrnom.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3fjtptuqb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3efcxouxv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ywmombrm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3asvszljl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3oyuhguqu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ojjrzukv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3fwmjfpet.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3vxhtonfz.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3ugysygxy.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3zauviczg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3vqxvetkb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3fhqmhqmm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3lkptibks.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3ogxbgrqm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3sgrakcix.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3bvmckcjy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3eeuhdbvg.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3knikqmml.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3jbnywdlk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3szmxednc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3vzgydbeb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3dydyedgw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3jsyododb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3ktiqmrwd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3lqkzrlqu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ivmpwmlt.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3omxdoqux.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3htvjqbzy.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qqnlqfin.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kujtztyb.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qzkfoqfq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3twbibnde.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3knzbxiul.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3krhwnagh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ktdekvls.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vypuckwd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3vsrvlrpw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3eioivmli.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3elugpzvu.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3wxvodgos.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3bpdoomjx.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3jfaxrueh.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3jmsrmcim.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3xilaehsq.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3vbfzuugn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3qvuiqbuz.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3gmfihumv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3emaznbov.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rqkavgdl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3aijncmej.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3hxivtsne.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3oqyaikcd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ggczzjej.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xskpyack.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3qmatqbfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dgnmmqjz.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3zblrtlak.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3natyoezd.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3auszvbku.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3huxuhmfn.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kdpaykbi.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3htnlqlqg.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mevomhim.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3dbcupico.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3kdzetdzq.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3sjxyrhhs.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mfsjunpd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3hzaobkxl.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3chbwzvha.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3nfvacbau.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3sytqtspd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xtdegbmj.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3fqhiobmc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wuzlqrji.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3cpgpudaz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3acjkvpyp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3mrmpxsqv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3lmjtnycg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3punbdpcu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3tkgjbtpr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3neogluqi.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3xgmrpcki.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3mqfngbui.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3mitpzgni.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wpahnicd.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3bhtilqpa.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3nquzdycq.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3aiykngqo.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3xkrmypbe.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ktnbdsdd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3enzyasuo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3diqugend.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3eadtbmsf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3axldkwuw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3uxcrmzmh.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hnwnshqk.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dvwgreii.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lmdbetqk.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sdaciyra.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3nwmzanpg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3dphudzqj.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3dqvncptb.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3wglqqkpb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3hxkmkdkr.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3cibbvbjo.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3auszgsow.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dbkqmtyv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3rfwrdikw.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ttzjljcm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3qgpeksee.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3qydpontb.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3dlzvebrs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3cfqvquux.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3vxbhuzfg.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3dqeotouk.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3aljvzeoi.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3infmlalx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3syrkephu.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3luocbjtr.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3jrwtjvyk.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3knspaclk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3hyiwjbeu.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3dygigprz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3xhlowwll.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3libbuzkt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3hvlcicpp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3yqccawfo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3czhkimhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sziaguin.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3byqnpojt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3prtbpztm.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3jlrjvtmb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zivrlhyu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3gawaiowa.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qddezedl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3esqarnsg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gvvpnmcf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jvqxvhci.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3grcvhlgp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qifhbcdd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3qfauyijx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wnmxalpm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3urxffiau.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kpsaxpzu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zmmqmxvc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3mckpaxjo.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lqxzgkcw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3bgdkcccv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3odyrduyv.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3yroupjfh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3adcuabvk.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3bgtsorzw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3bofotizs.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3iwpfwqit.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ryitgjvu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3svksreoy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3dobxwvbt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3kzmxnqgh.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3wktzuueg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mjsldlqz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ctdrcuqd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hokxyooa.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ykpuqilf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3whqpolhs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3azuljzus.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aahsvhgu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3amagjucd.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3cwjvppli.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3dtgewtog.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywapbigr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3famspysh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3rdfbzhfp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3rtuaojtj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3tbzrufip.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yobohygn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3bonbrksi.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3mcmbbujl.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3bziyfqxm.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lzpolahx.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bcwtqmyw.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qqkwdpil.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3uluznrkh.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3ekyyaqdg.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ejjlfvnz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ilmlggoy.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3lmfszpnv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3lrohyyyf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3epvybxji.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3jdrokpqj.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3kyzsznkr.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3yyyyrnhn.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3flpwresi.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3pfcpnaby.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3zgfhblrb.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3hsozcivz.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3sqzvxvnq.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3blbddoue.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lhswskox.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3uelxiqyp.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3adyzmhts.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3sdjkwmus.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3pivxdaih.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lebbpciz.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3lgjveduz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3asecmzro.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ukyyfxcq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3allmgagg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3lgltchqh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ofbkzccq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3fichdpyu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ierazzql.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3vselmhct.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3rbeqrndt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3islecuxq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3etdluvkb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ayiezhuv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3rwukcqmt.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfqnjdwx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3xtnpoooc.html


<!-- 参考信息 -->