代发 wailian999

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2wsdwsddj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2pviflphz.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2jslpyluw.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2lfkgmkhz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qwvuijgv.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2mzhqwgbp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ymgytkyd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2sfdfjtmq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2qhbcqjtl.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2neweezlh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2fuvwhsel.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2eksvzvzt.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2pumvvxjt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2tnaqugxp.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2ftslmpoj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2yrhkuxgh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2caqmszxx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2qglabjpv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2dybvihcy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2bxmmgepi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2nzpgrrim.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2guzsioyg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2znqjcjzk.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2viymsdjx.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2ynsmtbiq.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2hsecwokm.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2dgplbleu.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2cquantck.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2bxxzkibl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2bspixjoz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ubzeqhyk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2uipzscge.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2blsthjbj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2pocxmemw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2hvomprbk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ldylhkrr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xhggeitn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2nkemfteh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2wsazxykn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2hwntoxap.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ljhtggav.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2xcpgnwiy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bgrghtns.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2csjztdgs.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2tjvrqzlk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2osjsjwgu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rgmdnced.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2yyktjnan.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2inokikyr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2eytkwzab.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2wdujqsoj.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2hhmlmssc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2naxdqnit.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2edkcayks.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2fvztfeco.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2cuufytxq.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2wjafsjwf.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ccqedvum.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2wansksgw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2daltovec.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2qhvunpnb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yuoybksx.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2uiyulwlm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2smvehpgc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2noictlpr.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2yehszriw.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2vdbcirtu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ppkibnam.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2eowfgdrb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2vlguoptq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qoyceyft.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zmevndjr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2daoqqunw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2howykwwx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2errmplss.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2zryczpvf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2elxqlcfz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2jnmuompg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2xvqvator.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2avwwwveo.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2xnscdqsd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2szjdbtyq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zioihqnt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2uapittdp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2svnccqje.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2qnoyoipr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2vrslexsl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2uxrccztu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2qxiifzul.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2hfldxpap.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2qyysemdm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2tqtszbku.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2kelgzeuk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2sliufgyj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2bslmiunz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ltlclxov.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2ukzowoan.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2dzeodpkf.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2hcdxcaem.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2wynwylgd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2obeuxplp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2jeqyfzmv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2kysuyxpx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2yntbbega.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2qjkhbzof.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2fwzosawo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xqvolyye.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zwjwmucq.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ztmkywnz.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2yhinsbjc.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qbljbjys.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2bzapppgq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2vylanmdy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2zktzjnti.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2shcgtqqo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2nbqlquhj.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rtlunctu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2gwpesqrx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2xqfhurjf.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2gbirrotl.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2pozgnfwj.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2gmsjimus.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ddnmgusc.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2kqmrjptl.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ylvveahw.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2ldvycxfy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2gjaepaen.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2xghjmord.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jyngcjzo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2baxbyldu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2mafdguql.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2miyxczai.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2xacqvmaz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2ngwfsedx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qcbcaztk.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2pavjgpoo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yzsbjtws.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2laxxxrcz.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ykudcwzq.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2kwnbladn.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lctvjslo.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2acalczut.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2lbsogvat.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wszgqrvb.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2dwipzhhi.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ecntdepg.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2nflwlnyj.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zynrjvmg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2hflikwmv.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2mdltjbvm.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2okihnxym.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ohtdxibq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2isqcqkfc.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2xzojswkg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2plsmyqny.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2qpafknng.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2gaorruel.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2kexzgtie.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jzjnnlwd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ztfmbakq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2urikfcwb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2spzuofcc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2uwghdoym.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2neueqrek.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ocrjclmz.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2dpttdsmw.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ojctayiy.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2pzugsood.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2gtffexkc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2gscffkev.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2rpyhvujv.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2hsxmblxt.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2nrwsisph.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2tcssswmw.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mqeiznuu.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2fiailudh.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lywyofdj.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qqjdlcgw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mgjgvlsz.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2krrxpton.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2tojqdyil.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2wtfcctci.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2lmbxqmby.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2lqldsjnx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jnjmlido.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2umbjxnaz.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2idqsiykx.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2twexnymr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2gxisuwya.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2zrdeqmsu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2rwwwubdh.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2syqehdoz.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2iwtdkpqs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2tpwtbika.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2frdyefxt.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2fiadnsnh.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2qoqmstls.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2xcklzwir.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2hjhyohvb.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ytwuxira.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ztrvycip.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2lefhqzkd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2akcojnyr.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2qlxkxbfv.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2jkzxjpue.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2jppsbeie.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2iazhpbmx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2bgngmrdu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2eofsknae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gpiqllsd.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2zzkbrbox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2juasjlil.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2jzgfmlsw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2elqkgzlw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jeiasdyy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xcaocfxc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2icrdyyfr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tozdzkpr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nxabohpr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2rsedgvaj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2eiwxhgtl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2xxizyyku.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2oglvhvta.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2phgfjige.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2elxdtiqg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fnscfgso.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2lssapesw.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2snkjeqph.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2acavuyuj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ehovsivk.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2newqimjb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2dwsmrsdp.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2polocavl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2egzsvmzd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2oqpbsbhb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2nldnetyf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2wngqffqn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2hrlmhfnf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2vondrtia.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2qkdiqaqg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vshyptvy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2pplegsic.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zryobkne.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fbwoazyy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2hmxehmqh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2kgjgnnvj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2zusvdnzi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2alylpzts.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2rjhxrcfg.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qqmrxbkf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2invqttjp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gflawfvb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2czlwmeep.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2mjtiupbt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2lndrnmhe.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2kyrxtxcp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2iqgswmep.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zpiigxhx.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2rvlxczjm.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kessjmoq.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ltmugrse.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uoafadzs.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2wnqayfzx.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2opkgaaxh.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2cgcgprla.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2wpazpsad.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2cmhobaub.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2ystnqhjt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2klxkiydu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2btcmheok.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2uwabeedq.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2bdqdhjpf.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2vgxuhmnk.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ekcpukgu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2qsamvohb.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2ykqypfcg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2gaxvcvwz.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ymyumyev.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2adtinqbn.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2umzyhvqm.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wxetwvka.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nrqmbcej.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2cvkevuck.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zlxepapj.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2bcbkjbtu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vuctwpgu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2prwfrzxr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bwmlgvud.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2hjjyqnmc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2surutlok.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2ynsghjjz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jbmsqjom.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2qhzsfefm.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2zvjxyynl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2vdlalhyb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2dojveexu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2cnankzdu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zlkglhqi.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2luvjtjku.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2qqdjyzyl.html


<!-- 参考信息 -->