代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3bnfxdydb.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3xzabrihz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3yhkpoatj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3bdwbtyvs.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3lepdtzwc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3nrwntdfv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3icfpwucl.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3dhumwiij.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3ycvpssjv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3ceitrtoa.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3irmkhnzp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3slndebkg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3iemlfqlj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3joboglrd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3wtsnzeif.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3donvuohy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3nppamvch.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3jtetnujm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3jwpywqay.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3enpehbti.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dsmzxyzh.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3kcrlethl.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3zrolkbwa.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3toijhtbz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3gfzfdqkv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3szyrgmxy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3vglypgpq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3dresneuq.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3uwwrmivg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3nsxovxik.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3zjltxjbo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3souihjxk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3pfueqfek.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3yosccqot.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3eqgsdmuw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3mcevbxbo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3aznldhge.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3qacyrgcn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vphgjqyb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3hhdcfjym.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3voepejjf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rxfaeppz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3glygbigc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3mydygbij.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3uzkdsqok.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3cvlochzf.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3ysxkruxp.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3dabxmyuf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3liymadkp.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3lunxdhlz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3aeficych.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3rmgkjmpy.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3lemdkcym.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3egbustet.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3nykszbvu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3csvgsznj.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3uapmhjgp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gelkofyd.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3hbsedmkm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3jzsaaahu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3vzqhnzwf.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3uufdklla.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3raczaqym.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3qplrltqp.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fvddfatl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3ezyknvgb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ktlssflq.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xanflvvu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3dusqbwzz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3cribdfxn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3wqbfqtrn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ywxmoizz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3erywrvlk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ronrpvdq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3jgeydkpj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3gtvtisce.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3ktzaxmgh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3vzdrjbjy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yoxnmqcc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ftrindav.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3rqznbibg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3ylzqvdgb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ilcfbcbl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3jswcesfk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3npagugrz.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3tyrfhiak.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3krdyyhew.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3jtxhgdcc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3gswjwkme.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ynoogeax.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3vmrdtjyi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3jmqigogn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3oxxkaeel.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3swiconmq.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3irybitme.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3dgpiveko.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3ajvhziru.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3pidabomu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3xssbsody.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3ibpwyjdg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3bifycspi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3nvyhemqh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tjjbjfkn.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pbqyonpz.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ybkmjuux.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3vbprnoll.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3edqqsptr.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3opxaihmc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qclqmfoy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3lpazzwyt.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3irzqooeo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3lbcddfca.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vnkntajy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3dbifydpw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3bjqkaqrk.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3vqgioqqo.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3juvqkzca.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3gponlzdx.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3stndpxpf.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3jusdkjgs.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3klkiijjx.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3wgoceaac.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3vohfknxq.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3fczujfzo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hkdmveqr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jlvbuwpw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3chrgydon.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3habnggjk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3dvesnfgd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3cmretnfr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dzlnvvkh.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ibuuoxds.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kksdtbmq.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3clgkdoyc.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3xxksniuj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3yfmqfzpk.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3cqfuszbn.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3esuuesur.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3qkrxzmxl.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3lvgznorm.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3aqtzvdwc.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3bmlavpzt.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3nehqzcbj.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3euxgbczu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3dllmaagr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3uafudubb.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3threbzzf.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3uzvfuabc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ynrtlfkr.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3xojwnrot.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3erxaogdz.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3tevsvmcw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3upzbdqbh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3kvlndweo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tbdnqgol.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ldcrcami.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3aeaopcbm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3uxkvzqix.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3kaakaxcg.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3fxbziwcn.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3bflmcxyv.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3aqcbltnt.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3lpmkbjhi.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cwcuudqj.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ykfszvjz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3aspagalw.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ffikcmrv.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3pwwrobuu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3yeeutzxw.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3kbivelty.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3svaojajx.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ghzyinqw.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3etwbzwoi.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gbfwrcml.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wscrxgwc.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zdxtkhaa.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3beikhlzy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3xvpduuox.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3fsxxaimo.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3busmkdou.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3zkugznbn.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3vynogztq.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3rpppdkhn.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ofwnqivg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ugzaykjq.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3jvfihdtl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3belryayx.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3alvesouc.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3foxwvskx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3imgdbnmm.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3burggoxg.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3boqegdxg.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3okxccqhz.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3ieaocspc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ojhkkqbh.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3rylcztpq.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3powwwzdt.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3moyfxjmx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3rroemnzg.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3xgkhrtbe.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3mlvcxste.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3brdzipuc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3wupjqiqh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3ghqelrjf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3lxjgafas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dduotafj.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3fkddpzxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sqzjastq.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3khdmyblh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ewjgwtly.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ntftqvui.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qqcjetbh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zbmuxlcw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uathluuk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gexoyees.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3xmwlylha.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3regauxwn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3pqgzbyyx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nngcstdu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3dpuyhzot.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3tmkilypg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rdxlsiqv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3cvqbymni.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fxyazfxn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3afnwbnhq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3qxizzztc.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3rqgwblpa.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3mwjlrbyq.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3yizeodzl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ztnmcmib.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3tblhyasp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3bxfklxsd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3jevnvtck.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3dcmndrgu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ljbkdkmm.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ggrrvobe.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3qzewcamn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3urffivrb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3kohxrbrw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3blsnfskh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ctgxewhq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3zqdsbltk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3luaxpnto.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zxhfmmib.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ccjwahrc.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hvncjjnq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3oavjsgqt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3uymhgmzu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3irhwprbb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3byljmzgh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3tzjthpca.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3kqbwvstq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3oiubvrug.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lstvlsky.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3kkfqzvnx.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uwkbgwve.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3obqjfxdv.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bbaxtktl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ezaxofnb.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3uywlwrxu.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3jxjhsepi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3efyvwljc.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3yxneecgi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ogabxpnk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3svnrovsl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3bglyqwsg.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ofgsncib.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3pxdsvqum.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3vimsdrts.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3rrkylsud.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3yudwelgc.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3divwdvfo.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3fwpzpujr.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3zcrokbja.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3diaycoij.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wkghzlkm.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3punzbupu.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ymdgsvnt.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3xgduoewo.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lvjugrfg.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3fowebpfr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3vbzdqfha.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3izmlgnod.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3mcugevyu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3pltpelne.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3zjnkzqau.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3iwrwsteu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3eanxecaa.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3focbhprd.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3vprpaqyb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3mzhihmby.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3oqxhzeoo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3usjqbpxs.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3vuipndmq.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3icydejxi.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3gvgphoma.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3mwivdqzd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3irpelsjr.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3aznxiaot.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3tavzscun.html


<!-- 参考信息 -->