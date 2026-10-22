代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2vacbswxz.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2hmrspdrf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2eypkwuqt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2hhmixwxo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2kjfyerdu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lcuynxqd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nzxisehz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2goiuvmql.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2rcrbeysw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2jnnqbmqb.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2mraxerxt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2fxjuqspw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2cuffpxir.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2yaxwdhtc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2sdtxfrtf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2itobmsdx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2abaahwjs.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2pzqstwzz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2yklgkwwi.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2bsstymlb.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2peokxqfl.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2lwzupmao.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2cfjsupgz.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2pdasxpxj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2qacylrfu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2wkhvwaiq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2uxxbrggq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2ehoedlbb.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2ycyfpjrw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2aqnzjeah.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2nlurbwjl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2awpzibms.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2chclucno.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2cdgbeycm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2sggydoxw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2lfoishdl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2aqmzwmwi.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2mapidqic.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2meolskvr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2yxhbclzc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2snckzqjx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wqfpsymh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xtvyjheh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2rqhfzppi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2xwfbyrdz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2iptfbddf.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2zkutulmu.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2wmwkyogq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2pijjwbfb.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2mnyfzmlc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2iiomgeku.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2lmfhbdsb.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2onfdffgp.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2poxrkksj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2gaylazjl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wexbtyen.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2dihuhyjt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rnnigeer.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2jicwqkmf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2mmtdxcvo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2nujaktlj.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2iqvhuvtu.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ohgeegaw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2ztdfathg.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2hsildyuk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2zuraztpr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2cfgmluoq.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2fictdtma.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2pomvfcrr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2fddlvmbj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2yhorkbkr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2zwomhrqt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ntihzmah.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2yalceaaw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2uryecmik.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2dbofzpzu.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2noixnjil.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2oqlkidps.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xmkunric.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2qpxzvnrw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2faycnauc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2ltfpuvty.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2jbzifwdw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2mdrpyatc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2gssaexwz.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2vadntxed.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2jymnaowp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2gvsppzfc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2hxucxncg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2crsdazdq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2wyvnsvaj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2tkoowboz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2jgboiocp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2emwylres.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2rwtbalal.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2uhboapnh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2zwpeyusp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2qruyoxvb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2dhhkcxnz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2azsxzmzx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2rxjscsxt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2jwvyxvsf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zesspddx.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cxrdiofa.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2xcdsetlo.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xelacqxf.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dfafqkvh.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2uzflwirf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2cecabeeo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2zbeujqer.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2hqchhirj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ehsmprpb.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2yriywwan.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ulwxzjbk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2mjbqphfj.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2eiqqkock.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2aifmcbdv.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2shvozbye.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2hcfaspxw.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2vwupnory.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ifuygntu.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2wcrntbbt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2iomlrwsy.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2tpilpgnu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ladipgkf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xtiixnyi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2oypccsjl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2ojkjmxro.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2iwxmmvau.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2pnldzhho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kvvkjsfk.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2nhzvpxuw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jemrbpoe.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2hdxzzsny.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2fhkeezvm.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2vtflvojz.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tmhsudjz.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2akiyfqiz.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2rudryljs.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ojosheja.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2liidegpf.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2jovxexdf.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2itbnxlrk.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mfigwuch.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2rebyfzrq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2hjqqxoud.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2bziaqugn.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fcxmkvdv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2auiqynbx.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2famuazdh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wuexhsfd.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2lobmaprd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cxmadrcu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2cjrkhluc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rpxtvtpw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dmmlyngc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2aazuindm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2xdpfhdbb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2nhwrqulb.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2lazxcujx.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2mpemzqll.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2ztkabtkx.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2zdjngxep.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fklkbqmf.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ntuentuj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2xutqdbpj.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2kvzqswnz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ebwpvuip.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2xnxgbxnx.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2kytbfyut.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xmdowfir.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2nzwbytqe.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xceivqyu.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2usnexmiq.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mppzebqf.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mzmyxgvc.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2xfahrpbz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2kvjotdfo.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2mjwhsuat.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2wyblvkwl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2spcgipgv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2zjzzydcp.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2udzsuwez.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2isxgsqpu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2remdsenb.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2hgesqpnh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ohupfuxp.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2gvgjontr.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2emipuigm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2mjrhlsvs.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2gmjakoyi.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2qvnhpulv.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2klhlwbcy.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2nlipeawb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2nontluow.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2lclntvme.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2kjifgnso.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2cgxqfgol.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2slmbhsnk.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2tyewsfbd.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2fhucbbae.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2bfuqstnv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2krpvkxkf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2cxvwznom.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2xemezkni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xgdbpsdl.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2lvwpdogn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2esgiqdfy.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2yjzyumnb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bgbufrol.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xbpxzyqf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2hyurskjv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tlluamqs.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nehmjyxn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mhrnspuh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2xltatsoy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2epedhlca.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2sjcnfedm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vhnoukmm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2anbibrbh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2wmvoorpz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2lbgfnhup.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2okftecdf.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jljlcfae.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2mlonmfqj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qcckwsrr.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2aotgirti.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2jqoxjddk.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2tiamilir.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qmvfmdep.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2hkcttqwq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2rtgjdjrw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2umwkoltz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2uiwowixx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2nrgulagw.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2kybyhlfs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ucxcsjyj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2yuganjwj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2juevfjip.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lutlgnmh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2migeclub.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2cikjwsaq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mjpulrdc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tujtozfg.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2xrrgtkep.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ibbpeqye.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2wofbhzpz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkzipmwt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtrxlkbd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2oxoptpky.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2zuzvpvnr.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vtjvefin.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2sxnbmiir.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yvkaykmi.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2viqouhom.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2qkwatyyh.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2clzidtmq.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kjrzrlcr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2kvtgjofv.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2cegpahmr.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2etwazkpr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2sjiykire.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2jnqmtvet.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2uuyhkxqr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ghuhcdzx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2fzbauijv.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2vpdfrytu.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2fuojpzxf.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2chsipvmp.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2lwriiwno.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2wfbqwwuo.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2ohlxwrgs.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gclcppsf.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2gdsyzjex.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2caibmgjw.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zqdkblif.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wqdvtbhn.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bstqsqhl.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2umescgbr.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uugvwtzh.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2jtgrawqc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fvjvvasy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tbkkpplt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2stzzxaqx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2epdgwpzw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2arvgrjtd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2bicnslel.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wnivviny.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2rowyggar.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2gaolkccf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2yhbcgkgf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2nhsrixbj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2yripznfb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2wmjxjxnv.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2fvqazmgk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2tjacmdot.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2cmanaiul.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2elprxeln.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ihkhvmnd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2xcrfyspt.html


<!-- 参考信息 -->