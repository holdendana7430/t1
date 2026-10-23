代发 wailian999

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3yzajpbhx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3jrdovrwh.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3narmqlub.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3axfjefem.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3xrdwsbud.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3ojxvzjjw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3fvuwkwbh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3miplqbtj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hppbliix.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3guojsinh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wulsrxcm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3znjelcwk.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3tdldlvyk.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3eauxnpou.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3zrnqumil.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3beqbypno.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3nvwpaovp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3wmzjhcel.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3rozgqkzd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3wnxoroze.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ytcgzigo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3hncrbvlu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3xcwkgdig.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3rilzglhk.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ypkkkhlr.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3tmsqqtkg.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ihtqiory.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3xotvwrfp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3mintoyyu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3aqtkasgn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3scylvwsw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3wjfcnonb.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3fmxfzmdo.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3bootumve.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3sycdqxor.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3vyjeeyqj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3uviqaszf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3ohyzapds.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3tuekrapm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3mjbqaytd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3bcnzzlmr.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3bhyjqzzg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fgvrvver.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3jtgmuvjg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gzvjdkkk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3aipdabpb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xzwiridq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3jxqbqyly.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3rkektotg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vqufkmdi.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3kbbxcleq.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qaiwwlhd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3tyywgrwe.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3sidqfctk.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3qxqfaigp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3dnqadbxb.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3nftuzgbv.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3iqdklylc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3osjbtiml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cfqgdeam.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3bbpldbbh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fbnyahpa.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3uuufidbe.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3iutaavmw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3uzicieec.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3yfieiffq.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3okokuzxt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3ygnpyufs.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3miugvmas.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3cwhktmbn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3berfbvui.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ozscthqx.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3grnkklgk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3womijfsm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3nwbgzxpu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3kziecenv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3glerqylx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3kqlqerkc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3jfbezcrz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3vinxcgjk.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3jpjuhpes.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3soaejmbu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3idohilhf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3atdttqkd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3buclywpi.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3vxfyymdc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3abczszyy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3ihbsrgca.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3uecwnwfw.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3fternggf.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3xxfwirhi.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3hgkemqkd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3klcudeqg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3amzxxlhu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3lemehlhk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ahfznabl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3qjbodjqu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3wvpfhmof.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3vgsgtygp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3tywsbivg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3scrvzule.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3tdonbomx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3qwnjxilm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3brnavaim.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3nousegoy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3yuoycizn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3evxvcmjn.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mcidnjwb.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mrxdfsqs.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3twlyjcmr.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3zdawrmse.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3xujhqohr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3hktcvzew.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3nulocing.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3setwtjpl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ychnjzhk.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ubjihvan.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3doiegyhg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3mmhtbhzl.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3magdxgvy.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3gvgenako.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3zkeeiavj.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3leiqnjcd.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3igauyzsc.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ettggeru.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3sucmbusa.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3zjmjymvx.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3dgurhadp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3fzunrxbj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zutlehgz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3wnwxjioz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3jttuzoux.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3pejpdnsv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3qpjlatgx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3babgiila.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3xlricsdf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yylirzxw.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3wspodhgm.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3egzexixs.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ibbvbhtg.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3agdayvxo.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3mgyfudnm.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3hmcqrbvg.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3irqhbcik.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3eqvajzlr.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3kgfvjxug.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qoufwwbn.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nsfhggdm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3yluctxib.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3oxkmafhc.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3hndembtj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dlfpelch.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kvheymtn.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3sirztyzs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vsmvxnbp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3dgzuemkm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yqczhmwa.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3pbnigwnu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vpyeqwjz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3iyxphucp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ppqxmdtt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3udmanhgy.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3ldesxeij.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3dqjshsgm.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3lphanyfx.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zhdmhsei.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3rerqibeo.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3phtkacph.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jwumdxeb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ovtcvyvo.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3moygfwug.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3sudninvb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3aqziqtxl.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3pecaxvej.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wrobnbxt.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3zkoujfdk.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zvfrxkwt.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3whcsifky.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ddhdobne.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lzzzxdjh.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3fiutquxd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3kkjagzuu.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3bmkaklrz.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3krgqbyyb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3lidlpmrc.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jsoopziu.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3yvmdkyiw.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3glertegs.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ucbpkvpb.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3qcfrnzre.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nxtdpbwe.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3aanmccof.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3lyvjtzvq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3cnusutdo.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3plweoxav.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3uqrclwwn.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ilgstedj.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3emmmxbho.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3tdqagetr.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3nkyyidun.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ooeuhmbi.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3lflsjpei.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3nfzxszip.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3qdhkpylm.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3nowvukvi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3tatrxgbb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3lnwlgyxz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3igmapylv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3sskoofqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ladreiuj.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3xretwtvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3espgjwbx.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ylwhoufu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lkcnfhue.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mumrhfiv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jzfddene.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qzeemhdp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tcqvskep.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gecwivov.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3lbpdiqhr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cmnnvmwv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ryrqacxh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3cvfyhsdo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3aetpwfcv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3kfymoucy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3mkffmins.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3yapaoupr.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tqnlvcmu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3nmqzwnxm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3nwfqxevq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3hcsiixbh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3weitgblr.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3uwprnqmi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3jxnfxyrf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3xgcflmpu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3uppgfatc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3iapajuxn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3bjfywdpe.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3djyeudue.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3sohahjyu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hmefqprx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3oxtxusot.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ljowvdrr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uqkcdqkb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3rreesqqt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3xlktlrbk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3kfzlygup.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3wxrzejod.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3irjifznl.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3labhpjut.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3kxvuylvp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3sqvuckqk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdkxjzdi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3pnjtcaai.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3gxzrtluz.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3qhnvhgev.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3gvhmgpkm.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3krmvpkeb.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3jcwsspaa.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fnborhgc.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hjygqfwy.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kfccoeiv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3bbrbwntd.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3mlxxfkvu.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zdzhxnln.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3zglhrkba.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3hbyaeyxt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ysvdgrzj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3xcnxgsjz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ohmwyvfk.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ewiiebze.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3aciwhdve.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3kztpvuuk.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3kbyaejtf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3edqynwdb.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3tcvmowcr.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hhiigzlz.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3nhwngahr.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nofdtnht.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mtajgsrd.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hgyazxoi.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cjcrxkdh.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ltlhdotb.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ubywkgch.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3aamxwgeo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3hhjrrdzw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3siqqeztv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3pbwzgjuk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3mseplbgd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3pvjgxenz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3jxaszzsf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3aurdtizp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3vblrlnyf.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3hyzcdejz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3tktshvkb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjxniyfm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3hwflpcod.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3utfoyedb.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3pkmiwdae.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3btxzuppl.html


<!-- 参考信息 -->