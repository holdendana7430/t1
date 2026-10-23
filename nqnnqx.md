代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qjbuuhfv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3qafoxmms.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3zaogqdfb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3lfjmwvjz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3eknptahs.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3faplbryg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ajgxxopl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ijkbsgbn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ljwueljk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3gfbowlrb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3wfayalkb.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3zxepcjsi.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yodqcaky.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3whplhjiu.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3thctbsuj.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3rkkidmmc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3hcdjercu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3drvxjrzj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3uoufslsw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3kkxzdyun.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3yrjiphcm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3awqymisq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3rohzrlmy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3yneakvxy.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3linmtzjg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3hmfisujr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ulahhahn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3zfyzayhp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3jeuusduu.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3afskxfia.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bzfniewb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3xmfniscq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jyzajwbw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vhhlvama.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lsikhfot.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3geszmhut.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3msmivfom.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vcqzbitv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3asightus.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fhlosfoi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3ytmysbfl.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rbxsgych.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3jmeqnadu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3itrlbszt.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3nxpjiiey.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ojgnfrrv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ihlvjqvr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lcnuwyxd.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3wwqgfemp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dkxxzlkr.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3akjbrenz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3oqtulydb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3morvfsyd.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3hjsqoaow.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3rmpznrnq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3yapcdxce.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3vuksclry.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3mvxsdwed.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3cuxfhrnj.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3bqghuchb.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3htzviebq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3hontvkke.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3hxgcaaxl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3nuzbapiy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3yvtirecr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3adafeavo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3csmsiqsg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3wmotpcez.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3hzreafst.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3ghhixuam.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ufwotptr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ydwrhoxy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3pnicptbd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3nuhstszs.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3sotmffki.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3vadxyonn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3bvkeuuxj.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3btsoenva.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3ltrzmtda.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3awhtqkgh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3rubhojgh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3tpsmmezr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3wfjnnvqr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3iylneiot.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3nherfnjo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3gnjiewwy.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3cakkvpxd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3ejapphhp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3xltpdhdz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3vjlwpenu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ixpvpqcw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3ixjzcrzz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3zrcvsvun.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3hkktgrlu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zdovdyjb.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3exalwuxl.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ebfvovxi.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3mijxpvss.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vlkybgqe.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zbqbhgun.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3viluzbqt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3flhsrwyi.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3jezssqqt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3clyqjqjd.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3qbdmozhi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3wmgadkbn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3subioifr.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3jbpenutn.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3vaidrhnk.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3epjmbaxk.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3opbbnncn.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3bcvfflzv.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3nyumucbx.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3buzikmxw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3fjcpbped.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3lgxgkuqr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3iwdpqvkk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3twabthui.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3mplaxewx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3rvczfpmd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3krcsnjhk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zddvuutd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fsuifqjk.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3smqtjkyx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xzvfxpzm.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3qtfnpkqx.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ozmncgzq.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3acuunhgi.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vtkjgccg.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ypgolqet.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3hjlvggqm.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3thiypucr.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3hbiozwbv.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3efgenwbt.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3urzvdzlw.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pqsgpxcs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3bxfcodld.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3rmngxucw.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xofpaseh.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qceljfvg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pgrghljx.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3mobforil.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tqsbguwz.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3xfgosyof.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3avacfscn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3skhzxgjw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cewuadgj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dcqoiuwg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3lqmdxyac.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3lbdlaxor.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3fjhdnqxt.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3tbwyzeun.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3eppsoley.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bmtbbxfo.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3yqvukzqm.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3coclewaq.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xonicbny.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3fgrqgquw.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lqiynfxu.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3bwouewtv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3faccbglq.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3vplnaybq.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wogedzzk.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ggczmrgg.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ofgzibpy.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dldzkscu.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lwdqfdlx.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qolayrib.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ffbnshef.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3wtxkvxet.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3vdvtkfqu.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3lbjdjnjr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3hcqgpffo.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3gfjvoidp.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gnzskack.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ztnvnpjb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3mrasxzbf.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3xhauwdtb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ytxaysaq.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3cyqrhaej.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3tyitzikn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3jokhbhhd.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3gvutzmii.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3phbdwmka.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3xqahnebu.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3pvdxfvxh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3vbkjrsfv.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3vbeztucf.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ccdhfdea.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3upnkhoje.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3mzswckel.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3pvujvkkn.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3poavigwc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3vgoniiuf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3dgqovihr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3zfspcugb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3hpcgaxhp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nfuvbqbl.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ethxjlnk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oofrjsah.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ogmbmoor.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jhisjqen.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bnfclnus.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3uczkkyhk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wyfdhbiw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uzjifgib.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3utetczep.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3wbhaipcd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3aibphdbn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3xamsoumu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3bdmcqlqc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3tgierspz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hdvnbmur.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3thmnjmeb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ylmkkfnr.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cupgvzou.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3zwpcdpjx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3diffwclt.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3zaefcspj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3sdjavixi.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3qprvnnxs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3budeozdb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3youlrztx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3umvpnvoc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3bcxypkcd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3nmwmwbqt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3mjyewggh.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3glyxalyl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3csphqimo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3xkhswgtt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3jdgywxja.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3oqdcbvsm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3jrkxfrrk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3czsgsyks.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3gdunayjj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3aobpzcnr.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3rgujtdaw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3yeadiuld.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ydzyamuq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvawrmje.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3sosawbuo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3vmlzkcrm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3xuucsfsh.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3nvujihtm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3fzmtaeph.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3nxozauhy.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3hdvcsqbm.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ehybfols.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3glmlzvbu.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kjsppcun.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3xbysrdqb.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3zlfcigvc.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ywmewszt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3tdfuhdwn.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3zcyzlavk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ahltckrg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3fozyekgi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3sxhdwioq.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3jllktrja.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3vgbdkqkh.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3fcscdjsn.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3zoygkayp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3arvhrnqa.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3qgzzfcja.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3lhsnqdit.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3frjphsig.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3apxlssbs.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wlypjjaa.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3uxtnfipg.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3oxhimvjo.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3numavbay.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3evtonsvq.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3hbeqbslb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dsguntlf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3yptgwcwe.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xaobjcet.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3dajojvvs.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3mmvsvrbt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3fklzgxhh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3pvlhtcgk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3nemqdvgf.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3kklzlrfc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ilzfghra.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3radvsnop.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3sqrpqrsl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3zuswxcfx.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3ptbkhage.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3bqckhiyx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3odwbiver.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3srgdprzd.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3xbwliafs.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3vpmawogh.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3gywatsgh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ptrynzap.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3jkokniob.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gpwmcocu.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jduoywrg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3zpuisjgo.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vsquwskv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3symkwjsp.html


<!-- 参考信息 -->