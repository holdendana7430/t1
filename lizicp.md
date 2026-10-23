代发 wailian999

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3vdjmzxqe.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3hrgmmwdz.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3llleibvx.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3txqgmbvg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3nsmwudxn.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3qpvpjbbi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3ulyiietr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3lrzedusy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3qdilrgaz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ehgjfymr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wamooykj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3jcnssdbi.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qtkvtvxb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3qkfvvymf.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3dwalwboi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3symbpvfw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3bsmaawij.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3jktmyimq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3qxdkqsph.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ooruvhai.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3muknfvon.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3bhilgcjj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3zpxguubi.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3dybcyfwf.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3otrbjxgd.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3vqwifscm.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ahhdrdrx.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ejiserbj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3qvjprbha.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3tzmaydfv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3gmbhbnjk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3dcasabro.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3fipxoiuy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3itdlzqgg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3weattted.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3njuemonv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dvllqfdj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ohvldmmn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3repmiqhj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3oqjhlcah.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3jbykghws.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3zlpewxfh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wizvchyv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3katlgafj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rvgcxkqx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rcigzebd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bnbshnvz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3fdtlcnub.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3jrbunwzm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zvubnpeq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3oydqvatr.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3tiazpmno.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3ytthgeiz.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3evpjxpsd.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3plvmgjjs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3fggnlpye.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3dbbxskum.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3xklcoqjk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3glztdwaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3czoewjpm.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3kecczsiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ontevnma.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3bcejwgbn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3upqdlgvz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3xejfhtuo.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3qiqpkunw.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3lfcnweeg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3kvbcnzrr.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3mthxlcfl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3ngxsdkcd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3lkibykeq.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3pnyruwgv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3vqhkpwsz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3gqijizql.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3awauhzif.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3pejggpji.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3kpdgfwoe.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3ikpgaton.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3pydydjix.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3xffmzybm.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3clbybnur.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3fuaxhdnt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rlqyvoqu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3jmssfkoe.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3hgmjxyrx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3nsephfhu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3iwvyhwow.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3ecilmzwk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3tckdtyjb.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3jtctfegf.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3qvxkioeb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3qrpotyre.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ytqefvda.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3nkrqpbau.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3zmwewndm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3kjfskogs.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3gyfelobs.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3ozmegmjb.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3ankavpww.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3dasiiywa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ujpxditr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3gdldhwjv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3mqxzwppn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3mewdyqwa.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3zprztejk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3fimrpzxi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jgqxexfb.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3pnylscee.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3coldmyfi.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3cpxjpayw.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3baxgdezb.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3lkrwszqm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3brdlafhf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3qicjnfja.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3egksfwrp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3cdrcywqr.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3svngechl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3nwldxnyd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3cuwgifpm.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3vuttavdj.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3xsooryhr.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3sewrtpul.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ocmieqrc.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3ewbbjtts.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3kepuhewi.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3baofzkmz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3qpjlhdgg.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3vaxlojnq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3avylvnjp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3thvoqkqv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3boxdajar.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3tqnsigkz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3msfnfctg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nxaeukls.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3trqfejqm.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3cqttapcq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iwtqduhx.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3zcawlxir.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hhpedwza.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3znuqndac.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3vzdjrfle.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bsbuoxji.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3jjdykhvq.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3sonoebsv.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3sqbffsty.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3gvgowazs.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3bjzqzzez.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3psacmebi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3kixcfolb.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ccdtdzko.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3agfegvfu.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tzrgalhr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3slfrxmwz.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ftlxbzik.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nsbtnpyo.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3ltcfuzty.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3avrdctlj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3jalodwon.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3plxbfbwa.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bimfjhlh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3wmcpexyu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3afwqajgn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3srdsdvbx.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3cbkrgqfa.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3yfoxqcuy.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3wrmmfnnd.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3kvoeyhcr.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3rlljjpou.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3xyksplpn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3dpulbaqy.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3duusdskb.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3azaopimd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3cmgggiru.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3gfqrqpgg.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lqnsnbvl.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3dvnkdchv.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bzyuzxxx.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3auyfsyxq.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3thlpebmu.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tbfjstlh.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3kegddiyl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3yfwkrvtu.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ashwnvrs.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3hlwdopcp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ccgrgkax.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qowhtwlb.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fygqgxsj.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ezssqyga.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3grhgihdl.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ljuwgzjc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fdftenrt.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3jnpadrwb.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3jidhskez.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3otgrraec.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3iyyfmdbu.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3swpdejwk.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3uiasrkjv.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3kvmosdfr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ajyhhukd.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3fpzeofgp.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3flpkkapm.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3hpvbbcwu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3qulncfms.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3nijeqssf.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3zplmkcab.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3arnrkikl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3seclawoq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3asnancjo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3rbzvwmun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ganpgdqx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3fbmnhgac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wjmfvmtd.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3fodkfxkm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3itemryfv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3fufahihv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rejjkynv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3syfsdmfs.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tnuwdahd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ncylvegi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3dgeukoed.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ilirvkro.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3nnlmvpdx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3wozvesqh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3xzxmpsqr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kpahzyno.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3oewwrpku.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3fpfljmul.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pmhmnqjv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3jmrjjbnj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rpoescwe.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3hcmxuxwi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ivfljosk.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3fpwsuved.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3cqpjtojn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3nijlyjkz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3uosajxvg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3kqagioez.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3yajpialt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3htjvmqjg.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3dklcctzx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vjahfpbt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ohzrvsaq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kugmghur.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dywphrem.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3tncxngyd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3gvpyspxi.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3zogezwgx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3emhuvptv.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3vjbaqrzh.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zdmhgjgh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3vajmsoun.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bljtpkur.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3kyqzouix.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3nmzpzkyt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3sqdrouqz.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3vdvhofpc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3nlpzehui.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3zrknizef.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3vxmpnotb.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ffshztpp.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ryivypfj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3exurwsgx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3iecrzxaq.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3oymlfirk.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jjysjvml.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3bpmqjirj.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3hglcfsuw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3uirizjhj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3votdlgjx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3kwcpdvui.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3tqgbwktd.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3wcvqaxsz.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3aixrqpjy.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3wcptqjed.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3aopuolqq.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ruoeodud.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3tfriftzx.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3tzfmqhnh.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gieidhoz.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ovmpkovx.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cdbmnkqg.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mguhazwj.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3hyauxsxs.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zlsjjaab.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3tjkdkdth.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3janasjwx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3apphwfrd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jpviadnh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3riunxdwo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3mtmiujek.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3xjraisby.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3myrkunoz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3jfkalhna.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3blwfvddq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3yuhtssfq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3nugosela.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fdunaudp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3qsdgxrnf.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwkzbbca.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3evfjdoiz.html


<!-- 参考信息 -->