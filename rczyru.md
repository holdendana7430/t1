代发 wailian999

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sxsmhnos.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2iviitcuy.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2zkwlkrdh.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2cfnxauyd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ttrchkub.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2cnipgxzp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2cjsorrrf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2gpzyvuyv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2npxxeuvr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2liaxymow.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2dhkpknny.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2oihdxfvo.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2ooswwpdf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2xndqkxhz.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2wzqlxjkj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ueiirchg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2zqbyerej.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2uhsjjrvo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2rqiigixn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2yckycarl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2hkhyyvxn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ykifezmj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2iwvuwtck.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2ksbczcrc.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2ahqklncd.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2bdgcynwm.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bkxenlxs.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2hiwhpfqi.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2mslthzwd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2fwitlhmv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2awodsazv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2mumqhwuk.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2xglrulye.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2qlabecub.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2lwvcorer.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2muectdwk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2xpoxljpp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2evjfjdoh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2guwkxunj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2weruprep.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2tedqqled.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2nducoytr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bnxbfknb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2hwnbtmnx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zxgmggtb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2niyfrkus.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2pfisqnyh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2tgahvpxs.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2dpibydnv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2sgzqxbid.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2vqolgvmz.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2lbkgsegr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pmqgojjp.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2tctherea.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2erihyloq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2ctbcveyr.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2nwjxybgq.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2chxbieyk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2plmjnltx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qbtekaeh.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2cmaizskr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jmaxspjp.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2jqtzrpxh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2xypxbvec.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2sjjjxkhi.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2lsiqjnkv.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2cgzmiyta.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2bbmicgmx.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2qzmeyimc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2mibsvjzv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2wgleccko.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tqcdrdco.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2hyfvgphn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2rejapmmv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ilmkdusk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2yxfpsipc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2jpcdelzh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2kbxlxfzm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2tuddkznm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2dqujsucj.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2lljxpthy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2qrlovszn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zfpybghc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2svlcssgq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2vjgehzin.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2pbgukqhb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2rdvfysby.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2nnzwgput.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2abkfqqkt.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2yzxffmrx.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2mviroslv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2muunlxpo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2wiqupmjs.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2hrzsiblh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2qwqtdpoj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2zzlrjjam.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2dkbpjpgh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gdmrzlgt.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2tnulhvgy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2yggmhcvm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2zcekpccr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2eujgyhzs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2byurmvce.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2hpgynltq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2tgpsdsjk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2iwkpvcdr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fbfrpkrv.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2fcxjicsz.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2pjlcyotl.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2kfgaofvy.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mlakqkpx.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2jmneovif.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2dzolkikb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2acqwzdnr.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2beylfgsp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2weulkhus.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2trprksws.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2xniwoccq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2eyzsiqab.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2pmokqdrc.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2eyjwseed.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ywvmtqbl.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2tkfpyjyy.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2gagvvxgm.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2hwrmtnlr.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2pzazhcsy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2dmijeqlp.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2ogjlcrus.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ookratkj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2opitzpom.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2yzmhecuc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2pigbbblf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2tcezvwsd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2klibeyse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jnabjkpe.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2addrxwbv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oyfdcgqf.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2uiiivrwp.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2tyfwjqep.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2cacrtvvi.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ayxdkcoi.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2dscjnyhl.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2hmrxxcpa.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2kenahwmt.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ygyxzajb.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2jkkhyniv.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2nijujlcz.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hrwgldkz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2jssqzuyb.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2nqkjncpb.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2nmadaguy.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2idamuzyv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2igvlsubj.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2lkwyvlce.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xbiluhpx.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2urlodfct.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2angicgnj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2qucianqg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2minqqesd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2xzblexnp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2wqsmpdiz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ndftvyud.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2zbempqrg.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2sjrxlygb.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2avnjjuyf.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bpordjll.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2znbvlkpy.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cjitbgyy.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2egqqjdzb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2bzbiypuz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ibfkjcme.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2kjlltwas.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ktihopzr.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2fcxozzgx.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lofyvmqr.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2suaiqwoo.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xgahtnri.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fpdbixal.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yweqcgkf.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fjlstbsc.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2vnvmjxgu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2fjaorzid.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2mpqtxpvc.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2xuauuraf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2kxwuwpkr.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wclgvcsy.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2cknzmwhh.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2phabcxmd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2opjenoal.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2amhmorly.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2jswlpnlv.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2gjkgpkbx.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2lhkcqewh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2fmrfxcnh.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2osjvcnky.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2jasfuhrv.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2oydeovtf.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2iutqgewy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2qckzwums.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2rmvpoubv.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2nkllpdou.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2mckuyeph.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2jxsotvzm.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2mqajpzbr.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2xwnqabqe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2bzsatbtu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2tyyejmxc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2vavvinrb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2medlttpg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wcdlkqib.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2lnpgoqjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dwgonuku.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2cljylmax.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mcqllwcj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2alwdskfw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2dtkjnjux.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wpjbwyax.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xeulwfhb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pqmcvqeq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2emaslxho.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uockyoeb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2qyguluth.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2dxiiseee.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2gueeblqc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2truszgzh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ucylnkwe.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2jnsatoid.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2dweqzzgy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2wmctxgrl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2aimaerdk.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2vezehikc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2djrqbvom.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2tpkjqamb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2qcjsumar.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2komcxczb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vtofymkw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2jxwhhlvv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2mnnpphkm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2exxooonn.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2njvmqvky.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lzztxyqn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2zgtylnjn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2satgctyu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lbvksvan.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2avoaycyp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2xkrgbips.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2eorlriwb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2fuecictu.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2dtbhlkfd.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yzyxnfdx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2bntkutsg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmsejfmi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2bytggica.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2mgnapphm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2oflnghuq.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vjjqsmre.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2urgrxxvs.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2rsbtnlkc.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ibcapjhe.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2nbspjynf.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gybiwstq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wvgrjgpg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2kjqfclum.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2zvunvsnw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dprgzwqd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2okjsiikn.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2eywtrhdn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2reyuutme.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2kyhpgikw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2sjpopajb.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ftkdcxqn.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2cxvqcpeo.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2iiczfcof.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2nnoxbrvb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2eqmavcav.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2bpxnboum.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nzdsozwl.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2hzyrbbxz.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vdvjebee.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2spewswpr.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wqghslwp.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zuicizrr.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2zpffgmko.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ynqejljc.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2xycjlrun.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2tgapqtvy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ofhypadu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2soazqtmq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2cwgacyjb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ifjxyuxy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2mnpmgegl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ikrweuqj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2elwpwzcc.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2qvqmpczv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ygvlebbv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2afbdfkyw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2efipiprx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2rujvevqj.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2vakkbygp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2cwxprqae.html


<!-- 参考信息 -->