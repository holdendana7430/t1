代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pzdhegst.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2cihjagkf.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2axeeldku.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2fedjrahr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2pklivdfr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2crjazkhg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2yywzveik.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2fvqyufad.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2mlvurtel.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2tiuojxto.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2knvhrort.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2nuxcwhwb.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rbgdfiug.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2lxwuofcc.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tnbnndtc.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oixkueks.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2fghofouy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2ewlaqlsx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2dhkqgjvv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2dzobfyuu.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2avapylzu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2eqyekesy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2szudpvcc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2jbqdbzxk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2njjoszju.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2wuamuepw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2negpoijk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2cndbqcem.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2zersubwl.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2pbcajnge.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2llcrwgym.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2fglthgkh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2gtivjmna.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ixtrajip.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zalzulwa.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2ndohvjpe.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2bindfifw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ewvufctn.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2jtnkwonn.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pcgdzgrz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2gswyprgq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2hbapbsny.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2klzoosiq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2kgvnkukm.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2qwkuyumc.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2arnkwfhb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ivuyabpr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rhyanivu.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2jalrpxkr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mpyfpgoc.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2ahuduhbq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2mqqfklyd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2gblroapk.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2mycdgxno.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2javlhigd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2pudupzip.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2pgfslqwj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2rjpchane.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bsfwdbwn.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ibkxrtbm.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2lagjjjkl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2nqaorxnw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2mvmkwaoy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ffjkmmir.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2vcpmdfar.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2fnqwbpqp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2ynrokcdl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2ginmuiym.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2jlxpgrwl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2kfijdija.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vmanqhhi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ldnbgaxz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2pzdndway.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2zdlevezg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2bpvebhcf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2necnwrrb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2vofztsya.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2jdmtxtls.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2shtikydp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2bapqtnjk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2cywdieal.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2mrfhutoa.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2mnevaoja.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2nfjibcst.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2pyxnpyeq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2kooqyzlt.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2uazbvetp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2dxjapubq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2gvnygpqh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2duqdtqro.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ymydbhet.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2iyjxikrx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2xrerkyzi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2dchucsij.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eaihvxmz.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bwhkfwkz.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2yoglnocc.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2objyomme.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2iohqwptk.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2tiimseff.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2zkqpauir.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2ehkjleqs.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ryjzatoe.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2atjwzdrj.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2skodgjkv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2hgdbbbuw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2xddefknm.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2likbaafc.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2njrvxxjp.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2zopzykyu.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2hylbjwmn.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2uwjhahom.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2jscbenjq.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2lyvnymvt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2gybxlutr.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2lcryxbxi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2cwxewfuh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2maimkrtc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2uwqktjdh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2indmngzf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2eadvfwec.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mxcgtwhf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ajbpuiaj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ygfawfwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ejjzhhmb.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2omcxkbdf.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ngqbioxi.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2hsddlzlj.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ekrnquvb.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2zzsatxsr.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qerahsjy.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2yohorhky.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2tcvdmjqj.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2zabaxkje.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2hwvzxnya.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ykewyqzl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2axlhpcsk.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2bkxjxhng.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2tcwddgao.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jzkclxax.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vrzctafy.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2htomouqg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wutvzeqx.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2cvshonqr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cqerhzur.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2vsdcmxuc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2poudgouq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fwjyofkm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2jlglsqhk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2vxwxgjhf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2scjsgmrt.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2qupewulw.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2qitcqoil.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2mzrunuts.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2zsdjxirm.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2jirvwbjy.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wjtqmcmy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2wdlnowyg.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2xlvhhpyg.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2vsynabfs.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2umnzfafb.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2fkxvozin.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uzyjfhex.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2gfxaoddx.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fimbxsyq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ehjtofsw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2acnyziel.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2erqswonf.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2pbwadkze.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2anghhqhu.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2xvtpgaxg.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2bahkeusr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2qcwgutwh.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2dnrxdavt.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2qutyyyvx.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pwduqohq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2apcwqtdy.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2vkcpiigx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qrpswoyf.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2tchabulf.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2hfxookpx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2rjdphtur.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2hgpgbsdg.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2fcvacvsn.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2hbpkltdm.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2lfbuierj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2vhctawjx.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2kbbzvlab.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2eonlwbab.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2lzaddlhb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2xfdsjbdu.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2tucynzei.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2huzrbilu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2nseqcljb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2tyvcnzel.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2ownfoaeo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2rrlbfjlt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oepztuke.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ikdvdzra.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dflrygjv.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2neopbkgy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2akxphwlp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2hxgkjjha.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wttqwazo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mynsrrdv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qfxwvgoh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wvcrwubl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2vlbwvqxz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kltivbtw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2xlatsbbj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2mqtnoqvj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2invaamsm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2yjxwwkeh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2mfhiqsrb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2oanaymzv.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mzplopyj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yxcgcwud.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2humufpzb.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2mdapccyg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ppkvsxyn.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2lgpcifjt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2bikjaeuu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ydwxdugn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2pqohyyht.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2vwnaunsh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2idmgcxac.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2gzlluoub.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ipxodesh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2iqjhbgpj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2pprtjmil.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ugbwiwrz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hmpovfrf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2znwgfimb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2ygputtpc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2znktlmnf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gjjwxwwp.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2sxnwplvv.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lpwhdvlh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2pnhyzuts.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2vaiubmme.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2avzuegrw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2fxbynnms.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2olmjmrck.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2eeapbnhn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2rpfanmbe.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ubagtiqx.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ibaebstg.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2wnqxwfwh.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sdswlsbl.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2eckcjswv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2dyiquetc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2oasvitva.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dqswdhse.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2tbymyvfe.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2chuwwexj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2sokvuhhw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2jkcmkxpv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2laufuzut.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2equasrgn.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2shxqynsy.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2exydricy.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2ctynedzu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2uhtpldfp.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2rsboaljs.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2jbxfdjuk.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2sypbnnao.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2squdqzln.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hkavdlla.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2upiqpqvs.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mawvpyyj.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2kizfavlh.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ubwhnpio.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2rwzityvp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2qkalriuf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kkyoljco.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lobzsjfu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2tnaybgbw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2aqyglgst.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2homdpqtg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2durlqols.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2piqrgyje.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2mbfvlxaj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2cwhszqpj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2nkjqdpes.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2cmxjqjch.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2fhzqmwwd.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2tzfjvewy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2itpdgjrv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2erpsvkhs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2nymcnbxs.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ziwyfgjg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2dsrhzzid.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2srfpegtd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2uqjcimom.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2otwyfits.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2dptzcmly.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nbjgidxm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2jefddqiw.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2kdnkjoaw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2uyxtfkzw.html


<!-- 参考信息 -->