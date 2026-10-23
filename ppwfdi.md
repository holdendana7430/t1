代发 wailian999

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3plmgwmvz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ldragffd.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ybhiirjj.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pljozttf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3bmpugpat.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3mlbiavnv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3mkmhgbzx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3hbexxzlx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3kbxehjcn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3krjkjpfm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3sewkukpn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3ewszppoq.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kcekzyyv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3yliqsohp.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3yroryyeq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3pzplmgdo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3fcwavcvh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3skwmhvfh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3oltzxrja.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ibmsumnl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3appzrvsc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ptkajlhd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3tkxradso.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3vbugnzfe.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3hxbuhufp.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3ngmlgusv.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ucohsxvv.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hspqczsc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3cfhmugli.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3kvtwqwrz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3xacvmobv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3potdfocs.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3omxxjsnw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3pwnzpsvf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3filndhig.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3umvydaev.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3mttlfirp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3zbapklrx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3vjmmtvfp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ptfexjvq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3visejhsk.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3zmeulpxc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hqncoxyc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3ufioorye.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mlkqtjnk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3okxbhett.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3potfribu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3qznstpde.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3hvlmajal.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kcigtxtp.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3mnlnstll.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3roirofpe.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3hehxlhxu.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3gxbnsoka.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3azzzcczx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3plpmmlck.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3ocuewxyf.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gpscfggz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3hvkwkiem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qkymfpdh.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3dyllsfqb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zjpzbqhl.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3xejuvdpc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3xvdnxadj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3jbutrdpc.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3uvrwpcgl.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3lxbiulck.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3zjbgwdoz.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ccfpvwjp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3mauucjqp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3oqjvmoop.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ptvvlqot.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3jcfizccn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3hjkcfsrc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3oowmoqlw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3bxzspvtp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3sqoeiqsr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3bfdnlfod.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3qnrwivwq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3vsdimvjq.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3zwybhpoj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3niaiymet.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3vayksfdm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3udsoawat.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3jthtcvmu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3oinctbrh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3iwclzytk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3daocwbmt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3hpaulwlr.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3pladomgh.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3khdgczfd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3fpgjncpo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3cidllipr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3pdotqpoi.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3unfjucmv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3lycqythu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3ctrejwcw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3zxsxyzhh.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3iwzkjleo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3zzctoyik.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3tazkwymi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3rsngjaqm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3uombjvev.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3rtikxwhv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3oirmugim.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3lxljdvyg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fjehesru.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pzojnaxu.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3fvnptuza.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vfvovymo.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wmkthfko.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3herissci.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3omyxqdrj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3gqvsnwrs.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3blxqyghi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3bpgzkjmn.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3khewhbpg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3ezwdoawb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3lbkgsnyw.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3vckheztd.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3vuyidcjc.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3hdfjwcuz.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3undtupwf.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3xbojbbyu.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ggojwrwg.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3qbmlmhnu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3wcyjqaxu.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3lstifpbb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jyrhytqq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3lzxudkwl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3cwuxpncp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3vatfhtuu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3yixcwxrz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mdvuongi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3chfbiwol.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3gpkbxlbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bxbshnrx.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3jenymlop.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3moghrfwb.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3yxgjjdvg.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3aletsvlx.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3hzgjbsjb.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3phdwikul.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3zvpbizhh.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3hnbzcozc.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ylfwgmnv.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ljozgeal.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jvvugvlg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3uybrgwyq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3blxlujhc.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3znakzzvh.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3objkcvmf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fmlxdovt.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3zffklvjn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mmjupjee.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3seexeqaj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ghvmmlga.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3vkopycym.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3havhkmlx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3hkwibjtr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3yehxhbyd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3fuqhhwhg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3lpbxyttu.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3dhxaxbtz.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3rozggauj.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3mtmaistj.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3zhohnped.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3znxsnace.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3pytgkeam.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3yxuovhnq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uaekchkg.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3quzwpwlt.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3wurlcvxw.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3mdfwaptf.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zafgitir.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3xzanmhmt.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qtgoiivw.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ghxqohaz.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jcqoiqoj.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rmzbahgs.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3yhffudza.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3swbilgho.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ndixjcze.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3waesmubx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vokycmza.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3fqjxfvcn.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bbqeihvk.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ipescqra.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3xbiuyjbq.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3etqjwaqe.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ijdhzqwo.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3jkagguia.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3jqqigkaf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3cusygzuw.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3mwzmnopm.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xulyzwry.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3abgzmtxw.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3qgrxjxhw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3fcyheigh.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xohmtsrg.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3xtossjvh.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3hfdirddc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3cyshttnl.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3nbhsxjwf.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ganqqqsc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3xmpgbyiv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3gdagzbbl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3yovtkqsw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3scsbixns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aydykbxp.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3dvniaepk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3egxxcaci.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3cqvpjsla.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3azdyhmpa.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3iqbezxfj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vqythqee.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3oveplqdq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ngcwvxau.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xmvazuxw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ufbqojxu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dwiegbgc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3ipixcfcs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3eupzszoa.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3bcniuxrk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wimbgles.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3uwaqfdvu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3fppyoomn.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3obfpnbov.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3irshayaq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3czseruus.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3oqkbsqoa.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3jxamfxvn.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3haiiqtql.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ivcemror.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3zazueqxp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vfqzpptp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3bqjtxbds.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3oeaphbvs.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3saccqwqi.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3cimfglya.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3qvpxwejg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3rzkilpky.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3owgemygm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pcadlmzs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3zyemxpnn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3rbbncfru.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ltwtvdsz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3tyquoksy.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3fjcgoazw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ndunaeyx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3rnotucag.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3urktscxi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mcixqrep.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3amsjwwdc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3wnwaznhd.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3sylxpkof.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3eripffqj.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ncssncaa.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3esylrqxd.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wavkkkiy.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xfriuvjz.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wuisozsv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3aocggvuc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3bghojnno.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vbfckwwa.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ipdlrsza.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3bwyrprml.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3twvjfxyb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3esdortjh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3unrkcoqx.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3blnkztxs.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3jdqaawul.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3dqdpldaz.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3lsieytwd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3tdqrxuzs.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3oydhrbzi.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rhhosxgz.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3liytfghb.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zvrzufgl.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3uugwlpys.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3avoecbns.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vwfebgen.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3rqnvbsdh.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wjtimiqj.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3hsgfrfsh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3rceeukbd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qhnoaqsk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rqmkfweb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3otylmfvr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3eyxgxvuv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ntxxmbjw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3drjdfgym.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3btdasbnz.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3pcmgazhq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3hqwwkyuf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvtrcfht.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uovlziys.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3hlijjhfn.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3unfozehz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3zbvzubuo.html


<!-- 参考信息 -->