代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zjoznrpi.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3pcmjehqv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3xmfmqybj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3yzdskdbn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3roxllelp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3orttsuql.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ijtqcxin.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3adfhsahd.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3uxtovdqc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3anrvickz.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3purmihvs.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3lioawuox.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3dxsbjqut.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3vvkmvvyl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3kqcqibqz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3hameisen.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3xqushgwd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3xknwbago.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3lsvxxxas.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3hwjpirwf.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xfkqgkeg.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3xctveoqz.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rvumfieb.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bqxqjggg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3jlufxvpz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3zctabksh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3xoqepjol.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3skmyqzmd.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3kjhipjsn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3prrolvjp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3zmsieacb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ttajcebj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vvxgvmeq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3zbgvyxgx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3iimafuza.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ekffefok.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3tohtqpmx.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3bqwahazb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3tpumubgr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3tagdlocr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xpmukryx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zbnldqsq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wvvfivey.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ujmpkhgh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3anlcfnnt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ddsnhxjr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3xbuvylsi.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wzxtctei.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3eszisrlh.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ropcfakt.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3uastsdef.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3tiydgrsb.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3nybtrbti.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tylhpcln.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3wkgiamfn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vtxdzfch.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3dkbfqaph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bmwwybgg.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3dlrtkrjo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3gvuystkt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3lpqzbxzj.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3joxckfjl.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3adnjcnsa.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3csfgehjf.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3efctjoii.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3nvimxgkq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3ycyybvxt.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3pkhbrfhj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3sopznlrh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3wlqwkefy.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3extdthny.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3kxxwcndr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3ooebviir.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3qfjxelyq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3ijsncjfh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3wkbyvozv.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3qaldicdt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3lmnaqfaa.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qrbznkbm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ozefmmbo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3yvkzvirk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3twjprjon.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ghjgrukd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3mrwldajz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3cehfntep.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3aaderdxa.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3ppdduwkq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3kohviksa.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3tudadxxp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3xaifkvqk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3eeyyaulg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3lqntswgr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3kgwszabm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3wegyklau.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3owqpuhkm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3cqoifmxt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3gonvvnuy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3udvqrqsr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3oztfxumw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3aunhhujw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3bgyapyws.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3ofwpyinu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kjvtyaea.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ecfkolbe.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ygiawhqn.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pywyplox.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lkzvqtgm.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qwsvviys.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3gvxhhhch.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ntjjghtf.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3akmaqlez.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3yggossdw.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3waxdpdmt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3jivyvxqq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3hksgkdag.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3eitmaesq.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3vtncdkln.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3uhudqred.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3mzzthqix.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3zvzzunly.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3zubnsrdz.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3ziuzyzuw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3fdznsyxn.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ogtqwjek.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3yjcougth.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3acyvgmxs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3xqvpwreu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3sgypghho.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3mhssqqen.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3zqhjixfz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vcztgnyk.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3rdswdspb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fhgzrwfv.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3kxyroqan.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3adxbvjwl.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3oalnsgpu.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hntyypvv.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bmxuffoo.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ttayvgtr.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3cwtmvoea.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3trzweykb.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3qmhcbytd.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ykoemnau.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vatxiwtk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ggtrnkmm.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3aogjbttw.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3htdsmxkk.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3yahyvlks.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wxnnfmgp.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3nxiyeptz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3glekaxlj.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3cdcjfdti.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3aonfxnyy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3vxxjxxvz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3aaytqmkj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3vpivvxck.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3hsogfnqa.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3rtguedxt.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3bsjrrxul.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3mcmeetpa.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3yucfvynq.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lojfiscu.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3onkaogou.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3catgjint.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3xydynxvf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3vcftcrjc.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3ethitwhl.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3gzvrjeue.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3qhruuqdw.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3czcvvdiy.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sajdukhu.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3kmcjhbro.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tkmnblsi.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uamrgbzm.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yccqqtmi.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nivlwmuq.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3kdeaulso.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3wwhyznfo.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3mouqsxaj.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3eowyends.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3rlczjxri.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vbblpwzu.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3kuzngrdt.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jebovitu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3gealeewl.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3rssiogav.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3xfxejmru.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3fyxbxqea.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3vjtbbzzw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3cyovwjho.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3dtcsjfzo.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3urtudvhc.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xhabutmp.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3nyvsuslm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3addaxyvx.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3oekihtwr.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3clhyysyl.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3myahzfww.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3vvclzqhj.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3plbiaoho.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3prqjvbam.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ysxunavy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3cgeishhi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3filaxete.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3etglzlat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ozpookjb.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3fcaspojg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zolkehdy.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3lmtmxvhf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3csphnese.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wabbflqd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rklftaas.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kpbyeumd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xybwycix.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3eucmhhaf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3npkaiupu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kvzxtech.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3gzimkhbf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gxabetwf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3fbghceur.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3eacvwuih.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3jybejumi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3rzkzyfac.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3erqyjohw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3esqrztin.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3chcfrabw.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3zzliwumf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ndphcyrh.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3gbyeatjh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3yoipzoek.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3upjqwqoq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3phusoakm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3xtzvdqti.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3fvaccxqi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3yyybmxww.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3vendcmzq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3wuleitka.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3gpghgxyf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3iyrmjhzw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3obiarzjb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3lxzamern.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3gywjiuhb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mwixxfnj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ytqednlf.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3isjviwna.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mkkrdhmi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwcsbato.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3wvgqrstj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3hwfibjcq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3qerbcaca.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3lzsrbhvy.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3hemwtygz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3afzlbppq.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3qmpvieny.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3botwlgnv.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nanfrhlq.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ktuxvqlv.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ezziljuw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3xncvacnb.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3hvzjxfhe.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3sghnefwy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3cxgvorbj.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ladkmrom.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3rptrklqh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3eosyhabl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ilokszqm.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3vrcixcvo.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3hvilzpcw.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3yiiikzmy.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3vcikjlxp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3ykrphysw.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3kdagbzly.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3omucwfkj.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3rycedtrg.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3klrosklq.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fivlqzcr.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wzxxgafk.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3atikzguv.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3lzcytftf.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3prhdrrpn.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3qviocbri.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3avpdnlqa.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fzlzoers.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hvbrbieq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3xcelqhoe.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3bafpkoxw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3iflbacgv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xxetmymh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3xxlahpjv.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3ikdqlaxe.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3ickbtpdn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpljvlij.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3bazphfvs.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3bretjthj.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3klxpotxm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3cdgbupqf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3eqrhrunk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipocmhem.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bmkutawd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3zjbnufji.html


<!-- 参考信息 -->