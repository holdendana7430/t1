代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2tagwxrla.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2puvgtwxb.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2jcefqwur.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2mdjnqyil.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2kodiynxw.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ofwrcqbt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2wdjrakce.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2khtllujb.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ewlowvtk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2blycblgs.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2oygqbecz.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2kkmzsiwr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gumuxcmi.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2ndconyic.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2jsamxuvo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ndhgnfkh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2gaddhhmn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mthnbkkc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2sjavukbv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2yfcudbiy.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2oaqhwiet.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2klxjvypo.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2lciuuztd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2zdtgumas.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2njmqtmiw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2zpsqqqxa.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2qbtvtjbz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2xjexmrft.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2rocwashh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2erppwqgz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2qavceuuq.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2crvnhize.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2djyqqklt.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2veydylum.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2tckvzvlb.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eypphceh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2lwpoaemn.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2uujnkvtl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2gupmqanq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2iybzegdn.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2puwciriz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2wioefanp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2wledzsoj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nbyculfd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2bjvzqeth.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2mxrpklka.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2aelxkbal.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2pjknxqwf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2avvgjcxg.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2eewzoybq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pulaszlx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2kydcvved.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fhpzzksp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kaxwutgy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2idghpyid.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2qthayepm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2pzpaakws.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mrlzamig.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2fxbyjlxq.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2akxybbtw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xtlshnwk.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zxcrevyr.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2wvyfbedz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2lpyjobee.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2lzzfjtgg.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jrhbksxd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2xyviageo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tfsmbvet.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2easfmzdg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lpwddkzv.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2shvuwwhj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2ysnqzcwq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2tkgfuzax.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2juisjapt.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bvnzhtev.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2gyzumzbv.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rhtfaznx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2pgciesvh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2trsptvyx.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2mqpwwamo.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2wpijosyb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2pjqpdndp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2guhrgryu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2gnuldfnc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2cabihnuq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2dtrdqmas.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2qowohpyr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2hoieenlc.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2qfartxge.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2jiflormo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2efpfsqok.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2xwqprujc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2xhxxolqy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2vrffvmni.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2oqvtuufi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2dxepqpmy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2opfmwedx.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2lhcvuwhj.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2rluxfvgm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2iaujyzgg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2lbfooixb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2npdbtjyt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2ntdtfnzs.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2nvmmsqee.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2onxnfkgk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2toucrhqj.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2vtnnvjen.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2wyoyprma.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2zlxunovo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2qctohnhf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2jgcnfkrj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2eajrtwxc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2yrvhjlyz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2xsrwlvlg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iltdbwrr.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2tijfdvnp.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ngcebaox.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2eyvhxhnw.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2wlsbnska.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vjqltmoc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2xmnktasc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2oodkaqpy.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2dcfstnzo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2hlhzwuay.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2vvssvqkg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2ttoqiudp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2kgpphapx.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2fqonqqzt.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2mzyotazt.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2wavviobq.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2sdzxaxqv.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2yxwymamw.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2yycdmioh.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2yihhkltz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2dqcoolks.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2sygyvfyr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hgjpkuvx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ahnfewue.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2qfbnvgoh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2kouyxlqo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2mdhwnveh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gmzudndk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rbubxwqq.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2vqcobgac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rjapbhjo.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2yorrhkbe.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2zhyoqoqj.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2awxxvhim.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pmewhric.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ubkeemld.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2uiagtkvn.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jedqptzu.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2dmdqtqtv.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2nigtggib.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2kuamunkv.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wegyhigk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2apgoqhxi.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2cejxczxf.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2wxfjlfbk.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ukdaiaxo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vmwvisyk.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ozwxiymg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lgpgkozw.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2tkimuqtd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yhvpdhvq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2rmzuujrq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2zldmamjo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2xcadibrd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2uuvxhmfe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2yaksdkme.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2cfziytcb.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ayrqscmk.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2lsbrbcvc.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2afecylmi.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2uoobygqo.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hhqyxfca.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fyrizyjb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2kkvjnnvf.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ngfwaxwq.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2tensdykd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2xvibsugw.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2cfnbeulf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bpyfuvjs.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2dikfmhnv.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pkhqzhyo.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eterudsx.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ojfbyhsv.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vqzsqzti.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2kbylucoo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2qxbyegbg.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2fnmemqxf.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2czivlwpk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2bxcbkvmx.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2elfzsfmd.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kprwjvbk.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2rcgsmqvk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2sdxitens.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2gvrblkvg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2zbnxpegz.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ohurgdnr.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2moynhhrw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2mwhzflaz.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2vhktlqea.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ygupndwr.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ghrpxcjm.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2wlzgisnb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2lengusca.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2kcczbsxf.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ejwcugnm.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2jlrvyuok.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2zxidzrgn.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2axulslry.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2reqgcpzo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2kxgnaihh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2coppjpde.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2rbdrltnr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2vurjhibx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vekmxiav.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2unknrrhn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hfnseesq.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2peenkqvp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rznzntgl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dakwfmsb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qpaoobkv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qdepqsek.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xcjaaupf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2moybtfwh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2tztluunl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jnwvfluz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2icadhanv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2osapyffz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2uocpjxmh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2nlnsqzms.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2dxjaqllx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2bkbiwfnd.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mrrtjnhy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2lhxcexts.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2hyweayug.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2obcuatlb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2wesyhzdn.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2iemzvkmx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2kgkusqrd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2gklfdoeg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hlfuhbne.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2kpkeclnj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2axcepssb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2nlhqloav.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2zyknsqpj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hpxidvox.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2bkwfdjku.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gfksdyji.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bfjqgqer.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2plhlgnxd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2kdjrpgjt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mbmbdzem.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bbynmypa.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2xjbopeum.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qpxxfbqc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2aquigokj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2uyaimmgy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ukxcluyg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2eceurexq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2lmjmvvtt.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dhyoltfn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2gfgvzoye.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yhsurkqj.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2qgnfypll.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dzcwmxtp.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mpolasxo.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2alacjdqq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2pgdpfrdh.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2vgxlknek.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2aupbayau.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2zjrtdzzl.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ientubms.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2qumlfjmi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2nsfeufup.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2kvbozjum.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2oaptmvse.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2sgbtgafh.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2nsywgzbv.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2zllfhpth.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2momisdfi.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2ipdizyjs.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2ijozvgeq.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2lqyzxvxd.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ufefbknw.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2aiyxpfik.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ryceyimm.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qlzichti.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ymerwkyz.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2omcimydb.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2jvggdiry.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vfcuajaz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lhhhzkln.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2amzuille.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2juqobtdr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2rjiespjp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2asocapom.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zxdqlytj.html


<!-- 参考信息 -->