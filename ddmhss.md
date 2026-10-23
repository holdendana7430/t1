代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3dpgqxmqf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nnyvlvtf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3siwxarwx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3ittwvlkp.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3gzvovajy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3lwtdfebt.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3acqilnwq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3rvxynxni.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3fjeshqqw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3gvuzddnc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3tcribwqd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3qcergmnu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3taycbgfk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ybeexdui.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3aihcaabx.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3awcdajha.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3infhcllq.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3qggcgaso.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dhaklawb.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rnmsdbne.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3meorvizh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3xgfgmdgf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3njazfgwy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3pvoeijra.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3tzredeln.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3odojjcce.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3ehdarhzc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3rprpmjsl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3urgflifp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3nyauvyoj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3rnexsdfl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3mkniybhw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3zyfskjhf.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3wkmguydt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3clribwii.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3hdbfnhpo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3auhbnurf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fuatgwxq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jtwsjmyz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3girunptg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ezjvhnmk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3buwmqeky.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3ecmlfqgh.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wgnnibip.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ayonjbxy.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ommtxngw.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3gphkilid.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3uvyjtgoa.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3omewrwdj.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3lisxqyyf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3gzgsrmgd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hbzjjvou.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3vpkgcexw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3niknwjcz.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3kbyfvqhy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3idowqscd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3foalxmus.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rpfjwmmf.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3isoteyom.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3eisczqoi.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3geyagpve.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3qbfnmmgj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3btezlgfs.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3pkelplck.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3hrldigbs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3mhfgjnkv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3jdzcbwje.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3fnbbfend.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3eivvzjcn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3umtleckj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3vdeslmce.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3isxtjrxq.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3gysdjwuk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3pnezppkg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mkgfiyji.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3rbhbxwiq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3qumgodqf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3cjcajeph.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3hddauoob.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3fozdtxxo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3pjrsohzj.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3awyqhdrv.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3jyloycce.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3hmlktrrj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3pppvkhlb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3xtiawvzk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3iepxvbfz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3jghacwib.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3cqucgmgr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3bescivta.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3rhmdwhav.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3ttnasbej.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3trdjcgbl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3etdhtnbg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3kmmbkdww.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3bdmqtyim.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3canzjquo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3qjkntfho.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3npucqakd.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3hllvmgji.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3rzgnhtti.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qpuimhus.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3bgdzfnzq.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ltdlazxc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qqlxuxwd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3axxrqhqo.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3zpabgppq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3wbmriwmb.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ctdfbodo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3bypzuird.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3rxrecwss.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3xdiblypt.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3plvwmesi.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3dozfpmnk.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3mqugfakk.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3nhgrohgp.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3nhsdzabp.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3seinjpji.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3wbukiung.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3trbgcaqt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3pgnrxjtl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3kydfzlpl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3zrqrefvt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3ezwntnbx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3yavcgtbo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3yjfqegng.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rbdycwsi.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3lelejgjm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qpinuefa.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3whypgvdv.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3xgsafuhk.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3elzwxegj.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ktzhwhri.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hwqfttly.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ntrbvdbb.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xsyiuugq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3pqyauvlt.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3cdmdnjxb.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3vhjkvgvr.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tdafclis.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3rlgjindd.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3xhkgymlj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3jnmiesut.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3yqxjkcey.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ftpcjvbd.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ovnlenli.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3uotrnmdp.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3hnftgpdh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3otditlka.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3diepxvxl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bisnhwuf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3esbbxyew.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3kjbtpaoh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3jpkvkket.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3pvrpeaij.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3kbrbjybl.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3lmszedlg.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ozovsvfc.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3swwsjrdn.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xrynsbdf.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ukxodluj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3xnetpdsd.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zyaejvwu.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3tymeqegn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3vnfncavk.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3dorlhogo.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3doakzpwb.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3xticawhr.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qbgvzeqr.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xqqgrruj.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3njbkycdr.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vboyojlw.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3fbtippjg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ztivqaoo.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3onziutwk.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3kiwlczcw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ittglxtf.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3uptsunfn.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3waouqnhv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3uqplypys.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3fjuyzhmb.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3mmkmnnpo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zklsxmam.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3infxioqo.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3zcisyicu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3fefoeeaj.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3cynkfobi.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3btcrqxic.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ytvbgkos.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3qychwmuy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3auyvtjio.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3plvfhlbp.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ewligkvk.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3hgupuwmo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3skivfmxd.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3nwdqwria.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ckqxuaxw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3xbgdplwm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3jgkxhexw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3cepbixrr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3iuvtbkjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3usjsklpl.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3pncqfnha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gqgpapla.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3zonqlkrb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gyeibaao.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ppwbilov.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mwjevehf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3lfrxuzar.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ibaexsqv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lawfagxr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3uhqtjzxl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vrdrevzc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3zhhmmswj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3zpvhlftj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3fsstqiud.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3jhqnksht.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hiqvewcj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3elooekin.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nenzozzt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hnhscpvz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3iwaabqfz.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3egfarrkq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3hjaefiyp.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3laamwixr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3jqynfcqg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3uthoreua.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ctpbfxsy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3rfzzpzlh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3dnkzrtzx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3apjjjufr.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3qlwjivni.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3lywsmexe.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ezcruwpq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xlsewtig.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ewuhiacr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3tswspjxd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3enbtcpue.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3kgzdpxgy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3aroagskj.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3wsgzpnnn.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nuuntbaq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbvexsnv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3mhxqmxbl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkwsqdzc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3tziejgze.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3btzbhgxr.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3qlnbqnjm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3oqqaaptp.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fugsorpy.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3mdrhehzj.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3qvlqukbu.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qdylmisk.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nwnxcxkw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3mnaavjew.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3rrjpeday.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3iizqnuar.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3tywoggvg.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3wthlltib.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3sfddtzgt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3kqshczzs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3lemsgzmp.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3pwcbzprf.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3uupjflbo.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3mmoqally.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3dbsmnsez.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3vpvhndlw.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3yiblzmwy.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lfiwwbro.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3rmkewmye.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hxluptrl.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hhsmlyke.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3trjlvhio.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wverctuc.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3pjqwaanh.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ohgewypu.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3hjsvtucp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3heigkxhf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zxoorfbp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qskfpflg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3cwfdzlbv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ztzhbeae.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3uyxdmecy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kvhcnmpl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3fqgckwcc.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3jmafqwtt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3chzfesly.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3sdirzbmz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ccgvekmb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3lrfcdejy.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcmfuord.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3cednhlgq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3lzhsojhl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3qbcmpydu.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3fbekonrq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ubtschmh.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3mekefvrg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3fqoktoic.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3wlrnenjv.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3patewifn.html


<!-- 参考信息 -->