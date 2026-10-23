代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3iihdvlqt.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3jwqnsljd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3ftpadjrk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3yvzaevps.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3uffxlrsp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3aesknmse.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vcdvkgyt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3soycitid.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3rcspcnyt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3fvygcrqs.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3qumrctvm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3gewelcxw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3bbahmeag.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3yxgwgwma.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3uotpgpzc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3wujquslk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3soxfydwm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3afraxfal.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3txocixbk.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3buelfxef.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3oyafdtas.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3ssweryjn.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ixqobkny.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yezsiwmj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ayomobjm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3ukwssgpv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3fpiqznfs.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3wmyhuznb.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3nyvobckh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3hzwkclfj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3fiouwaij.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3hmpvhzsq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3sccxrfmu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3gxpnuooc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3sfnxvwso.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3iqdfubuf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ineiytdp.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3lheepnnw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mkpamrgy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3enzhgnxv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wvqgaoge.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ypflonkn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gbzvjbbi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3uawwjdpl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3aotyuhtw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nhrtetef.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3nlxwwbid.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3ygszmaqk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3sexawstc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ezmmfrhi.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3bexvidne.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3usdzsgcy.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3pooadukt.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3yoiuiqws.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3xzqkscnh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3axyyhsko.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3wxlckzod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xpkjwmfy.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3ogcxdipv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3eondaxbv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3zfapxkrf.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3kzmhgrjd.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3vzloxgch.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3wkmrppju.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3vcgxxxds.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3siqdldzq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3tldatmsc.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ptpfwbtj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3fwaullwq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3yabrjxaq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3nkjfcrnj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3xsxrgjyi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ubuufolo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3shcuhaag.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3rrvwstyh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ngpdqelr.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3qexarobl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3pguexhmk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kxsbdess.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3uwjvqumn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3kbylbspf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3dtwwlhct.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3umkufupn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3ijtdnufg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ojhrvayz.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3rrrkwydi.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3naozcmpb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3kwchfaik.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3oelgahtt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3zekltmdg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3eqqymdew.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3jjhjqtyr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3tfpwwkqr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3sgkxknzs.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3dakdpkyr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3bbzuikir.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3wqryveig.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3iqvghtaw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3dnohibkj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3vsreilcd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3pscqbhlo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3fhyxtlil.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tanlufvc.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3hjtwjkls.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lkprzzko.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3bammhlxl.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3duckpqff.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ndnibesp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3zgtpvsun.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3qssyzrfw.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3iouslhat.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3hzdoksop.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ugazgnnl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3gpfpolua.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3cpnutsia.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3pcmqvmmj.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3msdrvrur.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3gjrwcdbw.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3caxcsgfo.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3jvwftpwf.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3reghzqtf.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3gusuxkgj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3rcskspaj.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3hlsehgkl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3eptlbeqq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3pzheuvpc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ofhpgkob.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3elfinpbq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3xrbkyenj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bsoyhwsu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3betmeznm.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3kwdmfbjr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wppcfbvd.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3qbyrtekd.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3tjgbkftu.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3qvctpdsg.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3djmsvvys.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3mdpnjxkc.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3hdlejvaw.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3mbjcbllb.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ihqvsfkk.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3xhemipcd.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wuaftobj.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wxnmuykz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3qkcyings.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3uvzpkuso.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3kqrqkgyq.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xuasfdft.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qjcteiea.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3znuuzuin.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ntwjxdvs.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3jvgorrgg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3keydjxxt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3eprvpcyi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3hklzeldz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3wlrwkamw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3momwzxfd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3rgbomwcm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3mmxkjtbz.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3kgwmzlfb.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3plwbmqsd.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3sfibslco.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3atifucdm.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3stvnmihi.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3zxoxgeix.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3mvgnefpj.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3eyazdrow.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3zewzhguo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3edskfckw.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3yturyfpd.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ztxhmvew.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3lqvagzyn.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hvfdbhrx.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uwkqvofs.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3njxrrmbf.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3irywjrck.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3zhvwooyp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3dhdtomku.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3bxnlammx.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3rpmhbjjb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3tzpbitjt.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3eopkbkkw.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jrcsiavd.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3deqrcvgx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3msggewth.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3xshacyiy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vojcgslt.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3qkhutnyi.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3otfpnmwl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3navqyezr.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3vzwlppwu.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3tycgpfbh.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3vrivzrzj.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3uycnipuf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3kndhhffc.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3pkdusdvv.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3rmcdlkpm.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3khauvtdl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3hwdviqag.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3wveznjlj.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3fkvkmxvf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3hqwlsguw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3biclxjri.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3jeiqgscy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3htnrbfss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3guzxomrk.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3hyaxfxnc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yayzkmsj.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3uymdsnge.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jqlkutpu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rqvczhtf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fqxnfzjl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vwmvspvw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ilqckxai.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rnkmyvty.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3haudsvew.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nmucwcyo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3txprfisy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xkostkpm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3saxjfyfu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3kvlnlhfi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3bixwqaqg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3pwvygbla.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3lwgjbusa.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3nwhdeznj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3mtovxqcb.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3vootcrwj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3qyccedbc.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ujaossym.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3yonidihw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3yvrqnbrw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hnpqamcr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3pmziykha.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3qlzagdsw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ogacwbqw.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3zzglpxgj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3qoimzqwp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3rcnecljp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qrmtoqgi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3nsaxktyw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3gtftghej.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3tamvxdye.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wgxtnxjo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dusszdlc.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3kqcalonu.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hurtbglj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ummbznpb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3vcagmpya.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdhpohop.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3kxifnnxd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3uuubxmwj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3zylacnpf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3czxybwtf.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hwcbnevh.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3wwgwxfpy.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nqcteemc.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fqtdyccd.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mdacokjm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3zlbrlpus.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3soarttla.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3rdkmtgko.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3njukqkhq.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3jfjbycsm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3jbrjtgnx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3vjvqzvcq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3nlhouoci.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3rhnxbjao.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3hursluia.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3qudxsycj.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3nxexmbgl.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3jslngdig.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3bwnqejjp.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3cjgjhrlg.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3vdombqux.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zrjcqzil.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ymnakffk.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3itjuylps.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jwvxzziw.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3laladeeb.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gxpyigfc.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3abydmhye.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3mwuxxday.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kprpibdy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3bhpetrrp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ijtmeket.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3gzhingiz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3phkdhjhj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zgsiaark.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3dwkqtulh.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3ifmsiakn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3zalcjgjg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3nghwoyaa.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3vejgbdvw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3btknrhul.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojftwash.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3riwepvdp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3pseuzxzs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3khlqvkur.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ryrgpaof.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3jbojtvjp.html


<!-- 参考信息 -->