代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3bdgcpkir.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3zwlgswgv.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3qfvcgzsa.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3zgnqzqxl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3hiyynhvb.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3bkjpuxys.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3mtooixft.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oflrsfxr.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3nfarjnzo.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pwvyhdwo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3nhxcvkrx.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rqszzjnu.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3tlukjwvm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3fkgwaxwd.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3gtnxwoey.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3cnnfpxfq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xxvettec.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3nwykiekh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3htsbwaau.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3hnnotpxs.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3dscacuwp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3tbzzreaj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3nghniwjk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3shdczccs.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mzkhabbx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3wjapgrui.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3zkyedrkp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3onsqakdl.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3dfjtmxvj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3zhyywuvr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3hyqllniw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3rgvcvzmy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3rdmsyogt.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3xbvrbjta.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3xbkemoen.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3apdutvgv.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lingmsgy.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3iekclxfj.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jnvkbsxd.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bulntubk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3zppagzmh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3gjjzutjz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3yyzbvqlp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3hcmjmjvy.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3vncltwvb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3kxeaifbn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3givykhca.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3tzusyakn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3yozkgrtd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3nnwckpgv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3picchbbg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3sduoqatz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3urxwlabg.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3ipeimrmk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3bjbdlkpp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3eidjtdqo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dbxemmrw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ohduaooa.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jjvtjpzm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3vuxdicyu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3mlcgljup.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3piblksqv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3oczvrslv.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xmyemtxo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3kargywkj.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3kqogfdpy.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3nkyniloh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3ynddfgmy.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3yftwdklp.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3xdfwlljs.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3rqzazntk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3klmsaqqz.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3igqkogyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mbxfwjzm.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3ipvvmbji.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3pzquagxy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3xqzenjhl.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fvdeidfh.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3fqdlnqsm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3qyirmeoq.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3blwrvnbg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3arvtpjqu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3sioobrlh.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3xcqzfrhj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3urdondxs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3turbvxcg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3wcqgzdfq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3bwpqobtk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3cyxbzizv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3lvsnjnzs.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3uuaknsif.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ffagrstn.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3riseqqgh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3mvdregqx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qqdslcpd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ayeuqxzd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ykjcshhe.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3rqtvkhtd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3eavzljck.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3xlsbcmxs.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3wuwfnqqk.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3qcgoxmip.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3gefwydcw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3deryrnug.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3tdsjydvq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3qnrymthz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3nhjoimdd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3gdbwilnj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3hynnuukv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3yvsxzozb.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3fmohcnuf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3eofgxtte.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3aksfuwkn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3gplomqkb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3bmstbbuz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ehtkuobp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3ysbcqvpr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3lnfripjp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ypyermxt.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ocnyvpvw.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3nolzkzzl.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mfssvllv.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qghqwzyv.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3mzrpbede.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qvwiglzt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3bhgqduwk.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3ndzupgzd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3rtmxemhu.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3zsajjvau.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3govnvsrj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3fcivmizq.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3phbfelwc.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3gzrushpf.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3cyvkxaol.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ksyprdue.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3gdklcomv.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3xhkznbsy.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3rfvaadgn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3hyjaeelp.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3hsypuagl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zieevevy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mbnyxbsw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3wpcrxykb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3gwhgtucy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ojwtffwc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3atuwnhfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cqxtkgla.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3krhiarzp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fngtqalw.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ntrxrlpn.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3pysmeuco.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3immuppyh.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3qghboppo.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3gmhqcazp.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3fvnkqiun.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tvanicvd.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3cdsdjraf.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3njesqdys.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3bofkfnwx.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rkvjrxkg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ugaxbpsb.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3dfxtvrek.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3bktdwrtx.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mgdnamku.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3sntnggun.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ugdepkac.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3grpuirwe.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3heutbdeh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rrbuthri.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3mrujkkqc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3qffykkft.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3lhzseoav.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3gfxlykzn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3nfnqqffw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3vuyhqrji.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3jltxgpgx.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3bdfgnpyd.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yoaovyfz.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3pwkqsqfd.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uhizgutc.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ngintypk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ofitcokq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zybgrrst.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3ybrjhhxq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3tqpzkluc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3zmvyiomb.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kvzioxiu.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3pljdgiij.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oyrmvpei.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zalpsxtz.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3svvlvcaz.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zluvjedr.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ovkcbcbe.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3pgnmiwdg.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3mvjlinrm.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3xecgruui.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3evjmyvgr.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xtbnflqb.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3yqaqrsid.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kbcvkidr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3celfdczq.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3mlbvznhu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bchmirfi.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ehhmgtol.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3thivfdsu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3npgbmuov.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3demgzwsn.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3dbxewymx.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3tmpbnsjk.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3srxrrcuy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3vsrfnkho.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3fsvsfnbh.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3wmgxbode.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3lsrnghcb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3jftxkfzi.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3tkhtgjcx.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ahwaqwpr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3mmkcdmcp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3pobufelz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3rzomxfmi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3iyecubny.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oukzbyxs.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3akeqrzll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3caszlmre.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3thitfrcy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kjrxykdt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ugdkyeod.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jjtlxmsl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3lvkqscoc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sruxdiks.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yxmpctmf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3mvpkkbzo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uuchmjyv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ocqjwurt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3upxtamin.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3dabvnuak.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3pwgudfte.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3qbegzbjt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3wrzdvbid.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3azsofypm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3pizuynrz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3oqgadocl.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3gdsuirhn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3kbzrtseb.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3kivkaibo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ihgbtfao.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3sdyqbmnb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3awdttoxv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3toafnxbg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3rvcunvzj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3qsodllfl.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3aotdplso.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3pemtacdm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3bhxorkzx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3advxwrhu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ywoaazqw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3safboppu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3jiecukte.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3prqgxfbb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3hslrnlie.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3aijflfwd.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3utbxxvti.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmtbxcmc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmqaqemn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxppafut.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3qtdnfpff.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ntkkqqqx.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3rsrbgnaz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3uryyxumq.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3echuczde.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3gtbalyaj.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3nugyvwpe.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3akkrrnln.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wyeiiacf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ujroisga.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3kxsqyjgs.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3tzlsfvlc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3yzhwddbj.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3fskycdge.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3aultonnn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3lpagcbqo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3mpajwmgp.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3lwiqwnbi.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3iirmoljw.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3vfnieomn.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3tlrimxoe.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3wkhqjupv.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3wjmfalrt.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3kulwpsnv.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3elajnzwp.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cdsbgsle.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rzazsteg.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pzmqnizb.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xcimacph.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jkbcwckv.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dbfhited.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3pgbzjqhr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3uvzydpus.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hzvkkpjd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3gbajkfsl.html


<!-- 参考信息 -->