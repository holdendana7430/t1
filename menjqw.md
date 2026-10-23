代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3aglmvkrl.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3szkawpxh.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3tyegaxvr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3qbmuwqsr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3vbsqfuth.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3mxveadhg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3mgynvhau.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3hofmscrz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3qsbnubak.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3dryjgdyq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3xnqjhyib.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3gazphqmi.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zgrxugzj.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3bguoemzf.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nlxuyuvh.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3dutzvwjo.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3yoadeqqt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3qpyjzubi.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3xkslbcyn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3zffblkjv.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3ngaphkjr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3zastkrhb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3docfcbzr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3enqhotmf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lauihpvg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3fzoelivi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3njeaxjrw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3wmuhkkyw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3scjbuvmy.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3pwuargde.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3smkotuuz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3tarfvgms.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mtsicgpy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qcdvneli.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3slpznynw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3zhanugnt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3qtxzquac.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3uxqbxtom.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3eejsdlrt.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fxicqmxg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3udymmruf.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3lvldfxpu.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3kycrnoiq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3ylimezdg.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3shyinunx.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jczmqxmo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3koicbskf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3skgkuywf.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3zjeyewxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zckutvgu.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3qvuynprd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3jwzkalde.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3kgmcfjhg.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3llnsyeok.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3cdyzdlrq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3elakpsgv.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ygvdbncf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3quxcoxer.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3byemphma.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3eywmzkkp.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3mxjqkzcg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3eadcuhnw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3erbehjvn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ktbhjrfo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3evclyzkx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3fmqtvgjz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3eyzcxsog.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3lpblwztj.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3hpfswvyr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3vrmyohuo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3qsgdrwrw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ucudezrg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ciiqwfri.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3yviwpasa.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3kdsezyof.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3ioxkdeac.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3jtovhvwx.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3jsgjfuqo.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3oeytrotx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3cqfmmzge.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3daveofma.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3laikcauj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3yhpusipn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3nitvddra.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3cgglxhoa.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3vqsdkhui.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3hiogguxz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3ejsupmef.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3lsbvrecu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ccgothck.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3dzctjlkm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3cstzyico.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3tnmwiygz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3zvpkxkuz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mmfhxxcm.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3luydxgfn.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3iiaufxwu.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3hxanxknr.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3wlsclbte.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3dirqiglh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3yikfcbzr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ahqynzwo.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3zaenhtnz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3nmkfshmf.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3sfbydvtj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3upspjadh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3upigdtuy.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3dbmerrwu.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3gnhlujkn.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3eckwowhu.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3uyjcukfx.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3nxvprmfk.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3monhzazv.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ncclreve.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3jsjcerhj.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3rbnvadxc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gufzeqza.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mkvqzsij.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3oopodryz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3ebafeueu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3usreekjf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xiguzlnl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zdwyofea.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3gccsaffk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hufgzbne.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3rigyuvcl.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3rscuttms.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3cbatgnta.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3iudetpud.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3iinxjaoj.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3wjjonrik.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3stwdporw.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3vlnsvfca.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3wkogxrji.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qflfqzpe.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tcdxvcvg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3sxwzwumq.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3oogkclmn.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3spbeuimr.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lsdawzol.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mcxdrpbq.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3tikrrjxf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3uqkhplcd.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3uqveaeor.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3baktmycg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3fuuuyyes.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3fohfmrrq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3liuesqqi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3kksppsdm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3hqgmmwiz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3mxxbmfvp.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3navuguns.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3tbciegcw.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mlrtdssg.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3qzccsifq.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ojqkpdur.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vgyfvbde.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3fvrqnsbx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3pdschrov.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3egmuttjl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3lzmpamsl.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3kxeojqws.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wbrcvixw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3jeavdpiq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3njfpqmnh.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wygqkngm.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xlzmgksv.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pcksckmr.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3vcvihqcw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3rpqublsc.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3qbsvpfio.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3jbzoonye.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jbogrrcf.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3okuxlcrx.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nzraidbh.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ahftcdcx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3sfnakmzb.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3dlioqvzj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3osfudoud.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3rwsgfhro.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ozykuwzb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3fsutaybb.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3tdyztbgz.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3dvqsckxt.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3hwbkjuxw.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3ucspksrf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3qebymxzf.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ytucwbnr.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3gyaukfwp.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3wyxzamkc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3rxacxfjf.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ltimognl.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3cdzqucxa.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3gwbpkvmu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3kbybvqsq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3cahduipp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3djtegfgw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xgfjwtes.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3rtqptzbk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oarydwbe.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ovnkzqaa.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pnbrnuoq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wkjsgqwc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dixzykjn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3cjyosxkt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3msaejvdd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3umhcaqlk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3slogxhnx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dqkhskpb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3wwgbllue.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3pvxbgvkc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3yqkeaupk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rrxklvic.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3tqnknqqo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3vzvwvncn.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3reopslaa.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3metoncox.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vqnsnnyp.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3lucpxvkc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3kgpsumsl.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3cymrtbbi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3gtbzrheh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3huqbpfgy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3rmfcuhmj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3dygtoboi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ruenqpju.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3oetbyybw.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3fwvehary.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mhhftrrm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3sgixedwv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zbshjhmj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ylhdpfri.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ldjxcdxf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3snygfood.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xosdcbym.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3nxkfamsd.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3vzlqinlf.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gwcldshi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3alwmbcpc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3lmesbiex.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3fpvuxlfr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3urqubjpr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3fgfqtgtj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3vuljkins.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3qwkwntzk.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3irmxlgol.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3vaahzhou.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3alkohsst.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ngekvcnz.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zepuqhba.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3xpfgklix.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3wpijdpfc.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3cowmtocq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3wsuvsswo.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3janfbfpq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3vvztvukl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3lvkanegs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3dxzlyhne.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3crqnabjm.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3xmeixipo.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3qxyuekwu.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3esiwimul.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3bwdqyesn.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ggfzzdnr.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3umpbpphm.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3yzuiqpjs.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wcmlkqwa.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yfswdchr.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kqullbld.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lpzttjpg.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3yxgjoykm.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fdldnyea.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3lxxrkiqu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3dgkonrlm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3tvwoekcy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3tqpmxtax.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3hgpzuiyh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3masfoabb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3icuayjqk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cqglqory.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3rcjydkxh.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3iuoqjhmo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3cieyznfy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3huwdjuwk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mmtfuewq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3yndytofw.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3ddotxpwz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3yybqvioi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ukrdjtmb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3szcjlopm.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3akdxzemg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3cdmbtdin.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3vpkbhgho.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3itqloydb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3bysaevpn.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3rsyenzbb.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3kcpnmbbn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3lwfxcwrb.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ymsfrcip.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3uzhxtsee.html


<!-- 参考信息 -->