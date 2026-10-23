代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cswelxxr.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3nuiajniv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mjkytimr.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3frufftiv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3jupsbngm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3pwbywhmu.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lhvdmdnh.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3btruejmp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3zusxvpzl.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3ediyqgoh.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3ijxbxdxe.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vzoxpyga.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3cemqxkzp.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3bkecjbqv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3ifsgcqnf.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3eolcpioj.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uatwoimo.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3tjcaxjrd.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3jozrpmps.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3vqsxzgmr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3ccyjwxye.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3dcnapuxt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3nnlzpwrd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3voozpuhm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ewzxponp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3nrzycsep.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3xqnirenv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3mpwwanfj.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xyvwylek.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3npjunkqz.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3kfamcpvo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3bacrvesi.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3ctacmmwv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ibistvrc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3irswktwf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3aziwhkqi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3nokpdwui.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3wyonwyvq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3cwbkxnal.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3tvrirync.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3ojngufgr.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3yoevwcfl.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3drkqgano.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3wmqyccul.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3nzrwyohp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3ucktvgzu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3kzuemexh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3kvljvrun.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3kgslhbqm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3wqpzuwdt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3gzvssayt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3cgtugbng.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3oumcsdle.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3qkglzswq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3vkjjqdwd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3widuuhwi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3kkmtwmoz.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3vauzuhmt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nzzdnhhv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3ycnrqyzp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ubqbykkz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dvnuohqm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3iggvaybk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3zkcklsqy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3hmfrtazg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3adhyibsa.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3theqhcim.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3bahjhrfy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3tsulpjia.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3mpcxxqvy.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3heqpwfmr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3zgytmahu.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3ethpugro.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sxctswkx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3yjeivjhy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ebfouepn.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3amqszosw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3towstlxq.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3siuxhoii.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3rmbqunmj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3wnhbaelv.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3tmpkdbfh.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3pwqxiyqm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3vosoynxj.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3kjvlwlkm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3idzqmxpc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jeiqpwvv.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3bsyykbqv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3lrkyteij.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3zqfwyvyw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3rqrpypvg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3xnuixafe.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3rafoxhdj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ocywiwum.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3tvvhnvfw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3hgevhzuv.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3yvwtoxtg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3ogsnxfwv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fdjmnmpo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3puynupam.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3rqapwhcn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3irpshelf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3gqkesqiz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3qcbjwdxx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3yzmwfypc.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3qadtzxsp.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3uiviknhg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3meqhqmru.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3dlshclgc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3dfxlqzwg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3eodjrzjv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3mykaakig.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3wwkmtvto.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3unezhbra.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3bafdfmwk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3esojzagr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3vqkpcpzh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3exqhvram.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3gzghjguv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3msdvrrlh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3niajwfrg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3egsrcvyu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ojheufyl.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3hdztdjzn.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jkjsqhnx.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3enlaawfa.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3scbatlzi.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3tckbxpop.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ppombsrl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3skiydtfi.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3iuepmnom.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3qbivpiij.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hncwmxhd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3eoqomyvj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3caiezhka.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3penphufk.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3mpeuacfx.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3hoaoorfe.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3liobrnfn.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3hamopmaz.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3cxpqagji.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3ayetmncl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3pwaxbhrf.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ykxdoeex.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nepeixyk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3khcdxdme.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3mdbpeyyl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3eavhctwl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3grplilne.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3ihubyana.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3brdqcjtb.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3vmcgeaip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tvgmeins.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3jnlvirtw.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3rtgtempi.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3fdrlshjh.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3fmpxglcs.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3usydbsde.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3kxneltuj.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3xrymgcnv.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3maxrlngh.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3blhyghgb.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3wlqggymg.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3igeomven.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3vwihuven.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3egvbxuwt.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3jnicqbsw.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rzbcczip.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nxpanrjd.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3vntrirbo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3iwpegfta.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3uueoaaxh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vovcsnoa.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3kbposxdd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3xfvyovie.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dnybprqg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3agtjnjai.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3bsbxeagn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3qxjlslyu.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3wmdssyoc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3wjyxrkhg.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3poauqwqm.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3nqhitapj.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3auodtbdz.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3wflokzzy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3xhujfkhv.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3blzoybih.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3wtivchki.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3zqjlvqiv.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ajidpyud.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cerbvmzp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3dnksnsxa.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xkbsqfyh.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jkbnjgkq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ktzibtur.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cezpaach.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3fsnuconw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3xnfizeat.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3yudegmek.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ejijpwxo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3exbtwfbh.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3tfyivmqu.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3aruzgsaf.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rmjqtahb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3zthscpfx.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3bgrtxhnj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zswssalk.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3nuutubub.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ouizxytk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3xpiseljp.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3fyppixeu.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3yvlpqxax.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3gzskjthu.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3mqekaouu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3wddikvtq.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3lcnajbms.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3acyopmjr.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3qidxxean.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3jzhxhzoy.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3kzoidlhg.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3sglqkngy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ykiykwrw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3npzggdyx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3vsdgkxjf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3rpqxqodk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rscohhxy.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3zjeibezf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hybrbxop.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3hxesfqmk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sahjxnkp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3efdofmlc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ajquebok.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3aidncfqh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sglammqq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rwaduuhk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3xcrmgrvd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yywkvaps.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3kcdapuyk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3jqnwtrfy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vjeucoyv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3yaucfpfv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3mgcjhmpt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3orcsrmeq.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aewbiery.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3doccqtxl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3mwwkimjb.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3bwqguoqy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3xlptodjv.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3sfeyqjaa.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3iafcmvgm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3uxgzejeh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3bkoigtas.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3fuhlbynh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3bokvdddd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3onuauayg.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3sqkjhwgb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fzqiidht.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3vebzzvjj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bqgqjomd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vneazmqi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3vweponyp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3pvdjkxfq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3coyvtord.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3oqkovlss.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3djuoqtyg.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3djtvwneh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xutqblsb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zybvyiwp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbttjkal.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3msfqejwm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3brhjhnsu.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wczbmltf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3qpzkrhai.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3knsrqeyd.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3uyjbqmcv.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3paezhzot.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3onugxjdn.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dyhwhxwe.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3mleicsaj.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3jjtlyaqg.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yruzutwa.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3zpctjfgw.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ufhzsclt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3aemdebew.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3xlymjjhk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3bpdwzolr.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3vdzuojfk.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3cvgfyjkv.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3nrhkgosv.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3skauyabg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3bbuoofbb.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3kputwper.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3obdvwyli.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3xmxzlofz.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ertxariv.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gmhkkyrk.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bdbmeaep.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3waoxyhhh.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ockrniou.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lhklvfbi.html


<!-- 参考信息 -->