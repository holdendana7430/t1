代发 wailian999

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3gjjiomgn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3fnnyjuqs.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3qjgfhgdj.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3eugpvnwb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aquahjcy.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3dfwuecoi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3ounuxnsh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ysfjperc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kdavuqva.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3klhpcmgq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3khjpcxem.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3weezssqc.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nobvdnfs.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3lksbrhin.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3dpdiqqrf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3apwrqbly.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3zgcpzyjf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3gzilhhbc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3mbcekfas.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3rpygevex.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3owvbcusg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ltkheref.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3wjoxhqvw.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3svmosvec.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zcdqaxoc.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3bmamfers.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jemnadnn.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3vmdclxsx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3jvixboic.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3okmtgnlc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3glqjocao.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3zpcliyjj.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3ubdzdyae.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3vubfrscn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3tyfljovr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3bcbjggvb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jdivbfti.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3qqtmlnby.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3qdprgxgf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3gaggjdnt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3rfpurwhe.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3hhhucpbg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ognpfnmz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3yedawtqu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hcvrpalw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zshxuuir.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3exemghdt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3nfhibtxt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3yzrsnoaa.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gpeicdvf.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3afyxmmik.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3uesrbgae.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3iywctnbn.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3yxdjnlpm.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3skhsmppj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3esczwtwl.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3kuncwuqr.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3zhccpudd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3adupzlkj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rauxvaqy.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3kusuisld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rufkxacw.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3xbevuhtl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3hcukmdby.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3srwfqywf.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3yhnjgxmw.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rinpnwxd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3welzvlvs.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3ebpkvdzn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3mjkenkxh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3sxnunefr.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3tdcldakv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3vtuvhvwa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3vktsqttn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3fzoqznkn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3uxkqtvog.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3vkqqzwct.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3hcwvwmbh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3dlzbxigw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3lwnbmmlr.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3rciechip.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3azhuubue.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3slbhvsym.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3dysrhjki.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3skqutwfq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3mpakbrbi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3epyhjwbs.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3clwmehrv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ueztyogb.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3shydkgfu.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3ytionpyu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3pszlggyt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3gxuogsyc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3mgzhgrtr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3nueudcuo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3pzjptlvj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3uumoatah.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3jcdicfhv.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3zoctxggx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3fhjqrooy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3lebjpihu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3kkgkikkl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3kxvumyro.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3jrldbqgu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3azuqetbc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3lngsgfrl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cpdfxqmn.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3xwduqlvd.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3awuohayl.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wecxcizu.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3alfjoobk.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3znrclbwq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3kdamlpmz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3nfaeorrt.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3nutyfcyj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3qmxhpcte.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xognfert.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3bnfuzgca.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3bvrtojnb.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3skhojjcu.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ojjeeqco.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3vzwrkkhk.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3dqtverfs.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3jlfeamdy.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3uaiidagu.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3lghayarm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3yuumenko.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3ymsgkdlr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3dxoomhnf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3pudhfnwv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3kfyzfhxb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3gjbtznut.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3uwgajxuq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3udkapoog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lpaagayu.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3onxgwilj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cgxhurfa.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3kumtdgrh.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zjcjjbfr.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ovmiemvd.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bqielbtl.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3yofxkhcd.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3qgwamfhc.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3lyxmudde.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3evjzrpqq.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3xsjdcmvc.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3fglkstpe.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jfijlpnw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3rajhneqq.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3rhbzgbgc.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3zagtgbfd.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3daysdick.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dgirmcwj.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3cofpgcwh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bgtdsbjw.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3xabeocob.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ecfhrbny.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3vvupifmr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3hsjwfklf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gaavdjjb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3gztxbqru.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3unndqmdk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3gqrcjgmm.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3lpgjohzr.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3dghadrwl.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3wsqtsgaq.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3fylkxrhp.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3knpjtwoz.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3jlrvkjbf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3hisvoscz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3ybscopto.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3olccokvs.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3zbkbkapr.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3uitctlin.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tviluxgz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3gmscqjvy.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zrluvlmw.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fjcxpokp.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kfkklfkc.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ouuhpcbz.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3voumhrko.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3gtgixltt.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3whyttxsz.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3mpyhlqpz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3dairkdai.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bpnjizcy.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fwgcgcwi.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pnruocxe.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3jjhkgvng.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3jjxnzrym.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3gcabrbog.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3likbnjhb.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3zoibcfnx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3xmfjbvob.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3yaetlpcw.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3bwdbgvzc.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3zpcjkkjm.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3pgrdsagg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3fgpupqhu.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3uegjiwxe.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3prtathvn.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3tomuurki.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3qwcsrncu.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3hyoycltv.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3krmhtdtf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3zscglefn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3rvybhtdo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3wdqyvlqs.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3btrqcjfq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jbrbrdpo.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ggphviuo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eljimlyi.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3xgubvdne.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jsgivwpi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bxpuucyi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fyoolfsq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bqrcglsv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vdlpyiah.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dvzywglf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3qyrukzko.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uevjjzez.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3lewvqony.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3tnefimer.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ydgzlqke.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rjnbkvae.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3chtuyzbn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3xistxkrq.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3wzutqdil.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lwksynzr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3csjoyndb.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ngzjigim.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3vdvceeer.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3lhknbsbr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ehmqawke.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3lzbugand.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3imgnypbh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3fpeskoxf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3zogvjpmd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3uaoypdcx.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3luikydyd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3giylppkk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3wtxpiykj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wgapmyxv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ktmtkici.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3gvejkxxh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3vforxqlo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ddmvbkqc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jjkcafmf.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3piqinjbk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wvlcjgnu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3tgxfdvcq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhbocqwo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3hhwekeok.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3bxuebdef.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3qefvuohs.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3ejfbdwfv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3aymaixcu.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3mzskfesn.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3sbclnsqu.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3jpxusaxh.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3eipdluni.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3aoafxkwh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3lmpozlcl.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3iarwftid.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yssjxddi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3slsrlwud.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3tysgiwxo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3bujprfaa.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3dmzsrwpj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ygvmfsrd.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3wszfamcs.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ywlzcpnq.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3ypnwwexm.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3znregozx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3zutwsrso.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3qxzydkxu.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3phpxmpgo.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3hyinhzqw.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fqnnpttq.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zeautbpg.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3sfosavjz.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xydumsxa.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3bbxvyncv.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yheqoakf.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3njvlcqqy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rordgzve.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ebbzgisb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qhdexzyo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3wkzwsuyo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jzmzrpia.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3syvtnulu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cmmbzfij.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3wdneyqkl.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3knmckjva.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3nesnjevt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujdfgbfx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3qcvjvmtv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3qghumebp.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3ynsvleer.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3yoscucjd.html


<!-- 参考信息 -->