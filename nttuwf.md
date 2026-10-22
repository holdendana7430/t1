代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2nwvfjmik.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2ukixmpsw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2mrruqcnf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2jyzqxgej.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2wdpfqfxs.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cqjnyyfg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2rykphnmp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2vlkxluyt.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tmbgjbod.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2alethjbt.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2jehyvmuw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2yucvxbrn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2gqgowsbq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2jevtjcfy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2kdpthjcg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ylimxjvg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2eoeexpic.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2inhebhqf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2jgyqnhoy.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2qlqjdtzt.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2wyiwbhei.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2jsoqrdbk.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2hswyferm.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2rrufxckz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2ayymtpuq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2gqnyyknp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2kvxjtauh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2tyswmyew.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2ejuvuwsg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2qmjxuoth.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2xvvnskui.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2oyoveypr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vtdjlile.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2riacpolr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2jpcxflux.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2vojnpfgl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2etvwhuij.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2flfuvynm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2kxdzssah.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2tmjrheaq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kfsdjmuu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zlumrybe.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tgzzzgzm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2urlyoluj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2vbwscwwi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2veyodnep.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2lufduxgn.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qxhfsbfx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2cvbmewjb.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2beotswvu.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2kmblorog.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2ihmnelpf.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2ssnxjbjs.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2hletdsgi.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2naliecjh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdfkcnpw.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2trglkapf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mvbnfsvd.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2hpicgrdj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2lnafbmja.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2plqhaagp.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zvwboovo.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2wdtdfmaj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2lsmjujkm.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2yelaxzqm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2vuoxccre.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2upqgxyzl.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2arofbrvm.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2eimyasie.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2kfliqruc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2mqltskqh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2trcqgycb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ixijkify.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2mmchwfmt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2rxlcfjrq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2oshncxev.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2dirlxdio.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2ypkyfehn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2iootppag.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2wauozduw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2nqmommhe.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2wnonfywn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2oulighny.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2pyrkriun.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2gbxfyvnb.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2twfrzpvl.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2cxbmgwrb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2iqvwcbus.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2xbdfywie.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ithnfpxj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2zstjeusc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2jqwalukp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2gbjdjgwj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2zxjdbefh.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2gsdsaqlq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2fsefxgmm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2mtozhttp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2jvidvcwk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ptqenykg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2rnjyigrd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2aobwpomp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2diabywjs.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2foawvrgy.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wbdyisip.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2zrfzabwr.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2gwsxqiwt.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mgakwgfk.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2hlwulznw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2otbxmrey.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2vfwgwspn.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2gcuavyle.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2acwtrqya.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2vtkjsnqi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2frfkjmwk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2cdfwlfrh.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2pcpphqnh.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2lzhqnpsm.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2zgrzmclp.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2dgoyhutq.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2drjfhptc.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2hjgieemh.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2mxvpavuk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2gzplqqfc.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2byxnmqon.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2cabmyyrk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lrcuvfus.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2gzjfzxyr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2apkgdyfx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2uaieaxws.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2iienodsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2scbznkhi.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2jzlcxxbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uccqmutq.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2mptmwznl.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2nynorcss.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2lwxgqxtd.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2buhuztlj.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ndaxhjwk.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2mktcuouy.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2stnfwzcm.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2uklfbvwb.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ybuwmyvt.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2oaylvdxn.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dnzmffiq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2xmpdikai.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2mmpoeyex.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2wfveurtu.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dffnxhnl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2usnzrrgr.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2whtspdtx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bpnuuzdp.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2mpfwbunv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zfhrnvmv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2pazvairu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2srxsenox.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fuoqdvpk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2dhllhawt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2vtoltjgi.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ssrqmdur.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2nwwctstb.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2qbowlhvl.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2nopsvgdc.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2lphgluuq.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2dgtdhewl.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2txvmfchm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2klcgcwjn.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2cqawrcyc.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2kwoiuexy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2qbfioypg.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2rgqzdozi.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cmesnwnw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2dipozjht.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gvfxajhc.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2axujaohr.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tgpnzzms.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yxsqvccr.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2gujnyesz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2unwerkwo.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2jrqjzlkk.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2tnanzmar.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2wsniuciu.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zblemxif.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hchxowvi.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2esfilxje.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ddrmgkbg.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2bqjkbplv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2voinhpvl.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2hvuowifj.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2dgcpqlwx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ctwbrdrq.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2asupgrby.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2zlmrfzpf.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2rvpjbdmm.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ydzenwib.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2urhrwvob.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2vvdiomgz.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2xvfzjciy.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2cnaxftsp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2fgknexrr.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2nxguoiqe.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2qfbzqbwb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2veojbooh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2dttllrzy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2zcefbdbz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2caqjuzcd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cfuswugp.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ubidcloc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zyrtzfws.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2azgzhkkd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gvsmixyj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mpjqovex.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2kocthawg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wocqgokz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ueaaknhs.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hbmxprde.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2dijhurvk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2iwedjkan.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2qsvtcffl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2cpjnktvm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2slrjwsbb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vhetslnk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bzuekalz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2xrqjoztc.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2katugymk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2pitokaix.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2zkkwsskw.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2ojuntcjj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2cbapzqfb.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2zobawdzd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2xbfppfep.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2vnljjjxc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fkmmnavb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2hjytlhsr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2gybwjwkb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2uuxehlzn.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2qyefzijv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vtqhegki.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2snstoguj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2kbazldjg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xfpihrbp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2prcurley.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2tbwwnuak.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mwigcpgi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jylpwazf.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2iysanbdl.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yhjnxzsk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhavxugy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnloeuaq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmnofkam.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2zlxuvmji.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2onyuzxbj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2dtyiokzz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2pbvhmned.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2xetehlkl.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2csxmgfxy.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2zqebcilt.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oxowwnms.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kqpfvstz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2kprolpwx.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2biudmlqb.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nrawbzsv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2lwriovjl.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2tdzrwqid.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2ioklkvkv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2dlfjyvyz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2plqkcmsk.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2xtxkknvk.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2nbbmecwu.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2kxbhbydd.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2bvaqfyww.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2sbpnlllm.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2ycsrqodl.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tsfyurdl.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ulucevrr.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xeawvcrf.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vnzhvubx.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zcoumzml.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2guhspcgt.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2tckvnbea.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ebaqryyc.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2dxsgrecd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ulghbyaf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2utdowhpf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tsrtlhvq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2dpljybtn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2oobcnrax.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2stxgbdsw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qwrdgqyr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2twnfucry.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2gkdsjlyp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2roylkdxk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2fhvvrqlp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2affenxzy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2jnvxxcxq.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2iybtycra.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ejkrycjg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2dtgheqwu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2zjtkuuic.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wxeyqimi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ajnqhfjo.html


<!-- 参考信息 -->