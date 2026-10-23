代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wbevvevu.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3gbudpwax.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3jeprjjtc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3kvtpqpol.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wbrvxizu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ibzgzlfp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3mzxzbngh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3tvzqaszz.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zbzpjprp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3juqllvqw.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3pyzbzoiz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3afogzcpv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3rzsqffzz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3pppymgvr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3pqikscmc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3rkeeabzn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3bgfbigyo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3bmthrigk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3jsyhlmvv.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3spxfgzyb.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pgwfhpry.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3aaolndzb.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3vesaxkxs.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3bpvgtmwc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3fedjduhm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3bgobmyed.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3rssmvgof.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3onyfiath.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3xdwcgmqn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3mcydwvaj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3jcjczmdj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3oaxvozcj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ribdmxqp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3xenidnqn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3wyezdhnu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3viwmknyc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3jkefmtru.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3xmkbhlkg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pderqejy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3mwfygsdk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jnjsleva.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tnfmejgy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3djczwmuv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ayurwmre.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3dxmillfl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ncpanjgq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3piaedhxb.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3mzrjjcsz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3tzgnlvti.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3lprglqqr.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3enmbqdjk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3jqrskdda.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3zlhzpcxp.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3fgeyhvnt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3cshwrjzf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hzoxfdsu.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3fuirkaue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jruimcgb.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3qxtqhyge.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3xrztyrmy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3jqvilwrc.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3elqtrcpr.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ybwrvqtg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3ailjzgkz.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3xleldfuw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3vvvwbmcf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3dvxntele.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3isnaeszz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ipgymcbj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3libhcaay.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3upublyks.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3wwpissxn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3vclptjxj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3epyewyyt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3jujcmafx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3wdcnmspf.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3cdbkmzah.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3aaofdalv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3fytjtclj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3qbtrfirc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3rkflnwqg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3rwwsawou.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3twgcmxxf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3azdidsjh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3nzpipzjw.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3oeacejgh.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3zrfukmir.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ciwaeavl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ghaoyweo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3uqpfcukf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3hcqqiuto.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3sztwgkcq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3xibxejln.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3augzxwpt.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3ffjdrzsv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3xkzwlgyl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3bnjplqkj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3aqybrtfr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3glswcody.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3otdqflzt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3avfjivec.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3rydwlkhj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mpsrautg.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ckbouaph.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lcabpohd.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3vpvvzmmr.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wjmwmgrv.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3uzmbyuzt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3rooqbzkc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3spsfydbe.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3ihggspta.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3xvdcdhaq.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3sjtyzexc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3uvjzotcv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3jafgppad.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3hkoxuccn.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3rbysitez.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3nadyleei.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3hrrgabkq.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3zbzxsirw.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3eiycptok.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3iipnfegf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3mpvcphxj.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3dozmpuwl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3sstscwzq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3yxtuyjfd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3reiujtvo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3krfjvylb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3duepuybc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mldmgugo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fbiijnok.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3norhoxsq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lswdggas.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3gilhsait.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zpmqidxz.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3dvilpjeq.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3jgboldby.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3iawmftwy.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ymzdwhmg.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3kjkeqxep.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3vgqwbama.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3urcclhes.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ssvptbyc.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3uhaivzcb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ytjillld.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xoljfqlv.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xtochzia.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3aqfmregi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nftwvwhe.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3kgsipenm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wxmaomwi.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3iukuzhfv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3nvjhjxkz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3enqnysxh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3xpjjgyzm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pdwugffz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3cnnchifq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ivtjbkmn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3eicrvhnq.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3pnesjntq.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3afgtvocu.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3eqroiftr.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3byknyyrf.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3drnoopoq.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qbjksijv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3gqdigqei.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3lrkqmjol.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3xiuwylfa.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3uavqopkg.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3natatlfc.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pnsyapuw.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3atkyyxrz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xfjgddml.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3umpschxl.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bwgmxuhx.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mqalzwcp.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3kmhnqukg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3astrwuht.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3yblbmube.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3yppfwnoc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jpufjmti.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hagundms.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3fxdwcjah.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3tqrugsky.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3uuobkfun.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3aonplrgy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3epvltjdb.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3mbxnyqtw.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3bjnpsvoz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3brgaulwa.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3oycrrpym.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3htxtprsj.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3aeuigbpv.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3kbztrtsx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3rqbiumaw.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3jnpmaaty.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3jzitmuwh.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3wpfwtkiu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3smgregjj.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3bbkicopb.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3zvmunbsz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3hzwsupwe.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3qyqgpudw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3asydtfaj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ppnfmgxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3twxlpdmf.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3sdbnmtoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3otbeyyuf.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3trnkzpth.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pwgitkkj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kpbsnrmi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3oquqihmm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ticgbgkd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nfqengji.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3irbzkxil.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3srfrjscc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dtvqrjpx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3xabeawry.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3spkmdxhk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3pijqhjed.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3oggtsgvn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rbcepett.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3mqtqrsxg.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3lnbwxnqv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3kctlkkbw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hhpkczdg.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3iubslqhs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3uagkhuha.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3pwguiloc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3bjpbpfpb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3qphmooya.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ltvbwuyj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3bsbderss.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3nhtjhuxb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3bgfmozan.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3sgxoyvgq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3jlrpnkwy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3imtcbmdd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3oyqzvdzr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xenoeldb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3yllllcaa.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3nhoxdhwl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xdwwavbi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fvqrltyp.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3wixwbaek.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zxzmkgsr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvthgvqs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3jzpwuxte.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpmgijuv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3jmzbwhww.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3kfbphmpi.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dfxxqghx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3kpjplmtc.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hmllkfiv.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3gjeemlom.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qqirelhz.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ercgvfbn.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3djrzuplh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3gpymqwbg.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3eddssiju.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3kizbfuea.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3kjolvamu.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ixlzcdam.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ragjxouy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3koxqssmt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3sewfobyn.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ferjzfju.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3qrqdhfue.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3mhbthhyj.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3quijruqn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3hakrqyld.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3keyojady.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dfbwayfp.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ytertvip.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hsdlfhab.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tdnwrtnz.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3odahllbo.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3oaxwpwjs.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3vjpmgzvv.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yzwtafuv.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ptsxvdcw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rcncpsil.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3thcycrhx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wreitatn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3rshqmaiy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3yrjakxlv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3tmpmityz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rzupdruc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3qnxbynos.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3qzagimpw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3cbygjwpe.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3gocxlgcv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nevbsnue.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3txivmblp.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3eurrebsb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ovqjscbl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3mipuijhg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3mceaxzqa.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3dfrhypwl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3wlkpkgdy.html


<!-- 参考信息 -->