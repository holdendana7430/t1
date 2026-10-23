代发 wailian999

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3qfggymxc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3fqjejufn.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3lrzwmaqs.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yfdxsrmf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3kmtuorkv.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3gfdnnvwr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3aegktnmo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3pdftfunt.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mgtnfhty.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gofpvxpy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3loujyzdd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3wcuskepc.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3imyirsvl.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3ioamzawj.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3pkgasrnb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3dhvpidvo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3bqfgtkrd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3bzjrzouk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3xppczepl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3kmysweub.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3lsqobkcl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3kwyyixkc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3jalnqobs.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3rhqepajg.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3emmvkmjt.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3enibiegb.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ltxtcjlq.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3kxqajlcn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3cdhrdejw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3pqhbxfry.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3uunqoujo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3doefqkdx.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3cijmhnyu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3nlhaynvj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3rjclikms.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3yxvcnozd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rvazdlgc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3yyvfvzeu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3dkhrzawi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3hzdoehtq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3iuvxykji.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3eaxklhaz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3udvjfevx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3imsiiles.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3donpoczh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rmncyhqz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3sacewlql.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3ephhmykz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3shyuhdqm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xrttujiv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3hbubobgs.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3pylozxmp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zbuokbjg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3mmvlhpzk.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3wfkrduew.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3tdorjchf.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3dnpqkfjb.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bpycbqvh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3oazemeev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ifzdocpi.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3qfcckczr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zsbusait.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3mreafwog.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3vlcbvkxe.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3pdygqkwt.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3jatcvkkd.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3blunssov.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3tdiuxthv.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3yleuikpl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3jtjbkhlf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3aqayxuuk.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3qwrohzyd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3jwieegmq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3howzhhkq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3jyppfdzo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3pmfsfqgz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3lwpuzvin.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3ryenwbqe.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3lviyekhc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3iizycczd.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3uxtdtzwe.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3afhfwbvr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3zkjcgvxb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ozbusfsz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3rxfregxj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3sbuohvdo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3czwozfgr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3nnyqtzfn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3jtkglaew.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3sedlddjw.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3pcmjsamk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3qijzwwdt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3vihkhttt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3gvvlzdak.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3zzxrigir.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3jjemamlw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3ahbiykeu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3upyqtsct.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3rsapjnfn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3chdqyftw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3nisamnai.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3dddoarym.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3pfcznhkv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3vgmouxtd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3utirjzpk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3znspopmi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xcmsomyw.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ogijrvhq.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3hdruatyl.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kxorunpe.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3xamlrouo.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ofcadrxr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3pjctpqek.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3xivhzmgs.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3gntmgioc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3uljjpokc.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3wshauwtl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3kcazcqbs.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3lfjyzrdo.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3jngvlphb.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ulmbrfhy.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3pzekhmpc.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3kqrdmpim.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3efhlknpo.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3izirnsbe.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3pchtbpwk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3zghwxoxw.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3sdgbnyff.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vytnsebn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3dohqytzr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3wzcmxfjg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3oglnuqtr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3zffuumon.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3vlxiijio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3btvassrn.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3pxtyjcoe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ljagmvzy.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3bqnpelbp.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vwplzszq.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3qyzryfve.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fsjhldhj.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ljdownme.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3vwyczgdg.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ecwjxety.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3zxbcmwwl.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3fezabljc.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ymkgwnse.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gzpstzvu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3zcacppli.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3niqkgsom.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3emhbztnz.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ecavcuxt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3uzbtkjku.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3owvqatsg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3watvnlkq.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3yfnuzokk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3jtwypyid.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3bqgryrzr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3tfmpaiiw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3fhpxercw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3uyyiuank.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3yhwraioh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3dhvosmdl.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3iajpadli.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3bdizueku.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3vshutvbe.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3qihbqxof.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3zmrviszt.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3plqipexa.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3payzwfks.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3tfeepuvt.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3tophyakk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3trqggiov.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3prvspszc.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yinaocuh.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3rpqbmupz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bozmyviz.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vxyoesdk.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3izqpvgtn.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lkodxpem.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3nqcnywjf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3jsvxjxvs.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3iiollauo.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3etmcimvn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3uzpcdhzt.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gkkjlfrh.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3eyevjidv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3snmbiynn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3udljyszy.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3figdwdua.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3swyehfjt.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3vcujiwbg.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3emuqsmyx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3vuvymeso.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ormpfyto.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3jfxknwjp.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3knvoasgp.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3wceebhbj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3yjoadayt.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3calzbsit.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3oagufodu.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3swfobqor.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3hhglegba.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3djiltvcq.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3exvvodez.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3vsuopxbc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3wrkvowwe.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3gacdiuki.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ftnuigpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eqepgumg.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3urxgeokn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3skwpvuio.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3xylgumrp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tkvwvyzc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wdlvedqi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kjdehfyg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3njiqborr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bwlhamap.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lkyabckq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ngglklts.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3psvndnlr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3nyjphwig.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3fxtmqtad.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zgcosawy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3urdwouij.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hwiavkms.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3kwytvvcl.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xknkxtml.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3sgtpaetj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3obktdbcf.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3tljihtee.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3myhxiccl.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3ngrocoyn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ouvqfxlx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3jfbcjvfa.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3iqljzlta.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3tvsywtlz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3itodrpkb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3cufdssby.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3wkkitbcm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mmnosxhw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3fxibnkrl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ywfbsskd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fioqpivn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3brjvwzxe.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3ojvvpmdg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3avjrgqop.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3efopnqnp.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3knquucch.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3kxrnyboh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3jorejhar.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ftsfcpsb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkbyvbmt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3cknzqenl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3vrldzlkd.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3fvfclkdd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3mjyfrotz.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fgnfprmj.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3citzeaiv.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3czliibko.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ydcnkjzn.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ielyzuhd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3yramrjub.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3quzxjxdd.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3osxygnnf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3sweeiafo.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3zyqdrwsc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3wclcmstg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3nmygqvnn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3qdipqcnx.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3gvkubodu.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ppturkgq.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3vhcamnys.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ibhlsfmm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3uepnlktd.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3fzwqyhhe.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3llxvdegm.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3mjdvwwis.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xjkaerqt.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ccaycuwy.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ioqyrpri.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3miiecmsy.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3otxxvbof.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dstznjwp.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3bklvioic.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3jnkgecxy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3mdyzyxho.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3pyabaymd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3uwbcttjg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3awdoatbx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3bwissxni.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ajvrofad.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3xmlrcloq.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3wxfqftdd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3cspmxppr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypqtfjiu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3cwzhbyaa.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3xgnozuvx.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxozpqyd.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ptuhwpap.html


<!-- 参考信息 -->