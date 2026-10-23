代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ivmzkipb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3mmybacdi.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3egrqwfnn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3yzlwnhdc.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3ptizigec.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3fdntiadv.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3fnbtezdk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3rxyxsiec.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3fuijfngy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3zdhqxxjm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3mzovrpdz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3tyfgprld.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3yybubqgx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3vycouvgx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3mfsyxsht.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3tsrassig.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cemhrzpl.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3zqryagqm.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3fnavthrh.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jbzarrxh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3hpurzdbm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3kwlpvjfu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3xydidrlj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3htaufaag.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3tgyviekw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3sboarmll.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3upshqukj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xkskskox.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tradwifc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3stasmtlg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3kebwaxmm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3hpfqnaov.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3hrjkuupc.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3prfbwnfl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ijthjpfw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3uogkzxiy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ehlrqbdc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3oaettwye.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3yjokkoas.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3zmywgikm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3vbnznmvh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3awjzqbcy.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3ehinykjq.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3smboycqo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gxttcxid.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3bqywsgbb.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3buadxgrf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3yiquglkx.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3pbpqyhbn.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3mkopzmbk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3fjbwohea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3loigxgxx.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3irmusdmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3irhzjkpi.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3hygwnblx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3hwvmkqco.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3pzvdvhgn.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3sbixyivj.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3iewxgfoi.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3fgsmzciu.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3fpqpzhge.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3udodkqyp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3rhrjnmot.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qrxdqckx.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3wejloyml.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3zpjjmmib.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ztbzqswy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ltalbjtd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3lyzktvrn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3agjosrgo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3tfuvmydx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3zvczwmkp.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3ihlxssmy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3hzoyvmvn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jivsmudb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ekpnbkuj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3iyiykwzc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3cbzvolhg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3kivfkome.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3lillvhmz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3wqgxouyv.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3gkcrizgq.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3mioplqas.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ygnxjqlj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3uliqjvnq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3xpuehjzq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3tdceclmg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3soxnfeza.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3mmnhkflv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3aznigram.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3dkqeqctk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ezshoibw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3cykxrttt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3filcolar.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3jjdlnuou.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3aecrasgw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3bfjmykso.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3ynrojkti.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3siqourtp.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3lbxihhlm.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tyebgltv.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mkpkyfml.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3zjcrcxhj.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3sydupzvx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3rpifydwl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3cgadvuaq.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3btzynxrd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3qqsrrtmh.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jrjjjkkl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3jswgmzes.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3boofwusn.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3olapzaid.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3frxcqagh.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ozzypywq.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3aauggltg.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3irucgsvj.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3dkmipczq.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3fnyrbfwh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3hondvcjp.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3fgwxstkq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zwopucmg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3eqvhtkqi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ixrtycur.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ujjzfjad.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3hhdeibww.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3cyjnvfzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yfuyrlbz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3xjfyauqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jajfhees.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3jxvifbfb.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3zsfkxreb.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3vyounnvu.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nsrmncts.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ljwitagt.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3vbwxpxyj.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3lkcffykq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3opjarhfk.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3foodtymp.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ycxphbno.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3chfcafcl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3oykaexhz.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3usnyjqol.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3wzqmydem.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3chevtgqz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pkhyyhkq.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3hbewkobh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3sdxjbqbw.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3szlxlmyz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ybldftcd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3znhgphcf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3jnnkmgcj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rqvjlzur.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3jzzssqdi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3huptsopm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3kddkutll.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3jxqsqwih.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3itykwcby.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3bojnfdpy.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3zodaylkk.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3olrwvkuv.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yppiexgq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3xcxcqlaq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dqppspey.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3olkpbfku.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3wbqgdewy.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ajivfnjh.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xnbutoiz.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3kgitaaoc.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ebgbkutv.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cmjaiude.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rgibaexi.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tzvoddgy.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3jitrkbhg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3jglbtpcd.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3asmtswmk.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3hfbdcrpg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3jlbphuwi.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3naezftzo.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rcxcmfrp.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3iaghrhgz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3uadetqnf.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3nwlcgqir.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3bjtpvxre.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3eivoaxtq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3okmagikh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3mnglisnp.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3uodcdgca.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3oagypcjf.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3uvgsipiq.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3qjxzbcqf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3gqobgrad.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3tktkinrd.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3lndnkykh.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3qsavlywr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3jowizlsv.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3aawcniaj.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3eepzhzsh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3nsvgorkr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3scyzheid.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3yamalsll.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3koxgzvlz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kgxbtnkb.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3plrvgiyo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zrzyabjl.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ayfosozx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kseswfpf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3sawmdrbs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ygorksvj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3sitbczxa.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3isxpxzok.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ntmlzuvy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3koozfwvo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uxtrrugv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3ocmdrmco.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3cxskmepq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rtyldndo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ayebhhks.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3krywlpuf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3rmajptzh.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cnvxdnin.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3qhupacsl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3furjvvbq.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3jwpzyndi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ivhfldmi.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3zrkgvcme.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3dnjpslvz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3tqtegoef.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3pqsganfb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3uzamtoju.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3luogfviu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3kxbxbkwi.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3akcxmwtn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zcpyusqp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3lloouqks.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dgvdylfw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3cnxhhipv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3mzucxpsp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3cnlrqeds.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3skgetdmp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jhrzpkui.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3sjrkhgtl.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zakvjryk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3jzalqezp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3elswavve.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtmzwihm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3sgoyikuw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3yebbjosg.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3ebjjldag.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3aijkuauv.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3gfbtxhdz.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ophcxpzm.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3oayhaorv.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mibhjduv.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3beycxnfl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3apjdphxi.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ozxvmsjn.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wdixubbt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3tmuxfncq.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3gqnptqrb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3zweennpu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3aezrsznk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ekegaovu.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3rxibpsfo.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3pvzoliiw.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3pedrpcpg.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3cltnxuad.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3cdzzxxbd.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3lgtdksnw.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gtbtozid.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3dlyjkjyg.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rfeleftm.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ytacrqby.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hfvlfcxx.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tbwrprkg.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3gsoodnea.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fditwljv.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3oruktwwm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cykdewmz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3trdgvmxh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mmoqkusk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3emkxfmth.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3iuoeudan.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ofeuiujm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3pervjsox.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3trynkibu.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3kwsgyznn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3jvdfivqd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3smvjgixl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tuhaubrv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3eqlfsceh.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqxmqiru.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3xeohjcij.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3hprhcfuq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3znvxfmju.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3mdhymopj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3xcdiwgjt.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3zrpsorbm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3kugfyjpn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3wqswncwg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rpigemzd.html


<!-- 参考信息 -->