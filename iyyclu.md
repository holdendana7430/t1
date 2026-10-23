代发 wailian999

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3akdityyb.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kuoplsns.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3ovmgdijt.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nriyduea.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ltvsqvgf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ezkuxmdj.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3egpcbrqn.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3qgmuxeaj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3bxbuotfe.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3kznzxsbp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3phswvaec.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3szrabxvd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kldmsxbo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kufnhaxt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3focbxhyq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3qlirfywa.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3sajfcpoz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3ougwodxy.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3ijsvmahm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3szbjwshw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3djcucoya.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3hfcxipsn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3socvgbpa.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3hsepryac.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3tpqatzpl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ujhrzozp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3wprujaap.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3rhaseufu.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3ugesorkx.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3oxbmeukg.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ewuwjvbx.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3hhdukhvg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3hdjaeutp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3jjwbxqdp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3armkzcgi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3vaouuksu.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3rqwttypk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ucywwmap.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3hykrmhqu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tjxlwaqx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3jeepzyry.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3qeymiixj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3tphrdsly.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3fslljude.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ijujlnph.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3fbxjfdwh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3stpyalno.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3yxhkjaoo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cijzfrcb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pmbbcpjj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bbntyroi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3tjjffpbi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3jskxpkbq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ixmjcsha.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3cqdrlott.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vcikzobk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3dfexmfxt.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3iqhrfaha.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3fyohyxdi.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3rvctsgjo.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3zjhwjewo.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3pyieglwz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3jknpklff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lwaqahyb.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3vllewpkv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bxmfhldi.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3nekseppg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3pmzrdavm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3kcobilxz.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jgmthjqn.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3yughmowm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3fooyylho.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3axjzanij.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3ptvulmur.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jiqiyrfu.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3gsruvcri.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3gjinhree.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3xdqfuxqj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3puaebqtj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3pesbczgp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3mfeiqqew.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3hocwrlwp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3ddfyuytg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3ffdqsrch.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3kagjpcli.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3ukibysfv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xbwjeyck.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ibspylvh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3dhobeheh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3stqseatl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3gkjaskgk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3ymfsxjyx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3kvvokpkh.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3euddwtki.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3ayjcdvxh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3bqsmrspp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3tivkxypy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3vypohaeg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3pfdyqeut.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3gotcesdm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3brflivsc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3auhcdrgo.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3tysiftch.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3jxqbryjs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3idtakmsg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3uixtexkk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ulzhesax.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3noodiqco.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3ehbcdaic.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3otvvifyo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ynsmsecl.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3irpbegsn.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lzqyxdgk.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vogutmhv.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3iyebxyqh.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3oocyzopm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3mlwpqion.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3uxoykewl.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3swbfwjod.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3cukdpgha.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3kwrvzyhz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3benmwmjy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3pncyjrys.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3hrwrwwnd.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3vddmqqyl.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3brtmsjph.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3gbleuefg.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3ffoikelw.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3hlegugdh.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3gnugefut.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3klvtadib.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3ndsvacsr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3yxkdllpz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3owayfson.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3alecsmgw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3crkrcgkq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3xqxtscel.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zltnfesj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3urglwdlo.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3mrgvrteo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xagtgotn.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3vuuvozon.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3fyhsrdsp.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3mxjwvzvf.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kvqkjnkx.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fjuxgmur.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3nozeupfh.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gyvdahyj.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3cdnjosus.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3qfrmolae.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qtgmujec.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ewyhbhzj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3nhtdordt.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3zxqzrdeq.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3bwszpypb.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dungidrs.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fbkbdwvu.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ubsqtjez.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ftsjtggc.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3dvuoicte.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3cnontqww.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3fmvjqhkt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3dawiunlk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bwekhols.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ugfyhheo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3zkfwgylx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3ahinummb.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3zufgivdi.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3vwoidbjr.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3juubosda.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3nnqjrqdu.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fqohufrd.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ebsvplpk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3zodkkwch.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mlrohqlt.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3itufvpsc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3kekeiixp.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3wfpwaims.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xwtqrpqw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3pmcfzzno.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lamoscke.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3plnntsmv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xccyvews.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lxrqpopf.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3thcjmpzc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3qeltlezw.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3dnxeqrry.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ktnpgozh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3hgweytya.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3mkumwszw.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3muzecbrk.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qpnqxblc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3zbjqufrg.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3rjqopons.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zweqddwv.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3mzoxcstq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3zsckirst.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3cznpepxh.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3faeglfjm.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ayvldgpd.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ldczcgmx.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3rztlnqxt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3iytagejx.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3nvfimqda.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3founlyuy.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3clojgcht.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ijxvcrnm.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3yvezkoya.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3hhrmrkyn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3bkmfgejv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3neiytqcq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3qqcghdnj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ldckaprf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dtrfzoiv.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3okruywsq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3muynxxap.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3apneplko.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kpkmrlgs.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3msaxalqx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nfchftep.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3exgienyy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jmeukdap.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yiqnqbze.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3tdrfkfyt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qeflrldm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3wprvzqox.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rdtxbptw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pwultiqo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3vgvvagzh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3lcjwahdl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3xejerges.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3hqcfhvlr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3tbyjwicp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3pcrrjgwj.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3bwiudwwo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3kqocfumy.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3bjceaquv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3kofccqva.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3yrgsjnml.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3epqhvhwl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3broxaptn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3emwhwluy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3cdvzzmqq.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ipdqsihp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wvksaqpq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3tdmrekal.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qbsfvvfd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3iwqzbtwi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3hncxfmtn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3pshkyamy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3scdljxuz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ghxfydah.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ccrkpcli.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3lwbgcigc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3aoxrsfqf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ixtxvkip.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3xkpfkchw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3xtjbopyr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3vnjsxtvw.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pgjrkdwe.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3xjockfmb.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3khcgnbkk.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xzdqvony.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fhrmtisz.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3oshstien.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mjnlbxfn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3xaqytehm.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3pxamyvol.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3oxrbptpq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3vphrvrlb.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3uogkjrue.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3xcuusvvn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ohfcclhz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ubpzkmhs.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3dlyyxzwl.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3ohjvzpbm.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3kanjbwfw.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3dupurccs.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3hxunwqjq.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3zxcniino.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3cddkcaok.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3uwgjebsj.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hwjnefqj.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ryvlgmjh.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uftqoatq.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gemkddbt.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3gdverpqm.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3doorutdj.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3hjpkeajk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cbrauokx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3avjcmajk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fkwsgewv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3nlddjfkb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3rascmwoq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3xbfehrrx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3tswesgmi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3wkxcypvv.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ffsysasn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3yolhgxjh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3amhhjzlc.html


<!-- 参考信息 -->