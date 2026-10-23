代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3buzqtqtg.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ewgppacj.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3rzjglszk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lnwlkuks.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3ihbxfrkc.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3knpqjqrz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3szioxaom.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mgesoiig.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ongxverq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3cuodkesi.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3dzjubmbh.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3eztzbwmu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3cryxompf.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3kyhfmhef.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3qmelutbi.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3qngemdsm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3wsttcclq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3uyayusis.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3xjxhukgn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3lltzcugc.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3acsxyfrl.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3wgvxwcjc.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3gtcoprft.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3qebeoggp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3jnlrjvau.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3goaswnnc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3kvvujnvu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3kbkpeyfz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3omyuzpow.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3rqrmxsgl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3eyusjrkj.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3xcjqkbxc.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yhurjcxe.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3prjozlqh.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3sxfewnti.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ogrpflld.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3cupejnhz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3beubrdol.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3konpuijo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3ffyxfxnr.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3maynxbnf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3dripuxtm.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3ophtldwn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3aqfwptnl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3iformenj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3gyhnaqen.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3kgokanbx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3xpzcrmko.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3tqnzbntp.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3hvrosfoj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zlxfffbh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3qwzmlpid.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mcfismgj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3cgntiprk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cnemjjbs.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3axoymqng.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ncyysdmp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3myjtklcu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3pmnqmsxz.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mktdumrf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3etdtgbvx.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3yeischum.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3pjtielnr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3ndokaofg.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3bkyllexx.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tnunpfki.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3sqlqvyxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ekafjdcd.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3xezrjsaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fgespayk.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3xeqapvip.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3youvmxab.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3lkffeneg.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3imqycroh.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3fzvzmxdb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3kzpzyfes.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rzrqhcwi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3uoztrhlc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3nxbwcbgc.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hqyxudde.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3xgcuygns.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3ppcywbwn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ihpqojjd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3pfvwniho.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3jbuviutt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3btkvmnup.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3mzwdhjfs.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3bduhjwlm.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3etybjeyq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3ujejtnfj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3toactgzo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3zxxffcwy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3grvoviia.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3vccpmztg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ifrggqpr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3jrxlcpni.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3dbnelqlw.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3qyqjcjqo.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3gyvilqdb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3vufyicjl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ybmbukmr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3vkbhchcl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3nmflubpp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3yhliautq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3fcsntjrr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3hfwgfrec.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3spbvdiba.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3fepuacxl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3studfhrd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3zpjazxut.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3krugcdnf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3upkmadnm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3sxlfnabv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3zzbqvmmn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xpkytlqu.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3dlfwjfdo.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3uawzmfjz.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3lsjxrmgs.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3iwhetlrs.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3gqvnslzk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3gyfqsbtg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3rhenoirk.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3hxyxeegi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3vleaqbsx.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ttnjvlet.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3gigdsprp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3dzxjovbf.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3qvkkqpzb.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3oscdroqn.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3bxividhb.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3lssqewni.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3wyphepsl.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3yetftleb.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3otdwmvmr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ygdevlaf.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3rhevmsuj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ktsnvrad.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jbqzpaju.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3leswhlcd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3asqatjvr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3znnzjude.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3anhalfoj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uvpopzxb.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3gyknvwjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3huvyczza.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3kqxmtfug.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3jolghnpg.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3joivvhar.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3hzslbotp.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jenfrwzb.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3bgwzdkqq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bkfqrlxq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3uzauhjao.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ssddnamz.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qgvqbzgl.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xmhanvbu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ykimuslo.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3dgijjsgu.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3wfamdyuf.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3forwspzp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3beprrkwx.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3hoibcyae.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3yslabnwv.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3sqwemlxp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3pkhphngx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3aepqoiny.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3oypmgkln.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3hffrbbuq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3gjpssujx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3gqgqnxcw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3wajltuga.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3sqoalceo.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3uqjqrwwd.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hkdvxhpz.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3jncnrjen.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3cjzezccm.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wrexolbt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3eyzledyj.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3indljmzq.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3esembiwh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3kpiwnjgl.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3oilsdnjo.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tzktoewz.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ynzziuvu.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hzufdhpk.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hxqykkzw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tpnxyyuz.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3opppwabd.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3mezoddck.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3aqewkiwj.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3dogtaydr.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3kghddnqk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3suvmjaaq.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3czjxiwxw.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3hoocczoc.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3oyxtmjqg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3sdepfgcf.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ryigegii.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3kjqzyabm.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3stbohlhb.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3enrbdyca.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3xrtawczq.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3bdlpnyto.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3guamsrkv.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3iuwtcxfl.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3uezsufhk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3fgtlsbhi.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3njinnilt.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3dllmiwqv.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3rioyrufc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3gakfotlo.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3cxswuicg.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3wrsxdbsp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3azptjcmt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3wlkxxlyf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3qegcqjvx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3vpmepmqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dvfssken.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3qnckjase.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3edlyxkkb.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3bzpmrcho.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tljrwmop.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3nccbzthw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3hgaaqtmx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tkldshvr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hrrwscua.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mvtrtcgv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3grbfyhfo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3esyfkfnx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3awywmslp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gokzjtif.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3qkiwxmok.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wstuqwiq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3lebuqbmq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3dvixykuv.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3klnblhbm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3qojbgdvk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3cbjgyhxq.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3rrivjuzd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3phjxvnva.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3dugpiisy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3rbameksm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3jvmxfteh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lbeauoih.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3hhjgpkcj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3xnohbulk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3eywwowya.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3eczzvilv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3xwsijstv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3dmzujspk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3aifnbizs.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vdfffbiw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ztgfynxg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3kwpdhgss.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3namunkyu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zgigtoos.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3cbhfrwig.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wsnmkwer.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ogqlprqi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxjuycnt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3muqfulha.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3ltwzmofc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3fnolkxqe.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qrpoeqiy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3krctjtxq.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3vshjartf.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3sdatuxck.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ltxkujwx.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pvrticxe.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3khrejtot.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3daaayfgm.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3aifpgnuz.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3efiqkgle.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ulwbgdfe.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3qdaeweta.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3uckspifo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3jwpadlag.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3wyganxwn.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3xuqwdlvx.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3qkfrfbwb.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3epojisnw.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3bmuhmxbx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3sewpkyxw.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3pvdenagc.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3hcwhsrau.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3alrhcolt.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3leczreyp.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nyzlfmuj.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3atpxeujb.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pvehwrci.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3fimgshjp.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3efigllya.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ckglsons.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mbkpxvgf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3litpjqlq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3smjhqtye.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3qjhxanib.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3fjyrfhom.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3qtmcfqnr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hbhusdll.html


<!-- 参考信息 -->