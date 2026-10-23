代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3evqtcofu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3hkugfudm.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tsfdktjq.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3vdigvbgm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3vykkvgud.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3ngdlqleg.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3wwqrjlrx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vmowurkj.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3rtezebzx.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cbghznri.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3avorahax.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gpavwdea.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ktpsuqco.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3azbglmnu.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3blnsfyym.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3rcarzygv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3uruyppxf.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3pypwbded.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3ggwnlfgg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wzklsjfp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xrdzxvpa.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mydiyblz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3mjqawspw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3dlmlfzjq.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eniwmdzu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3ipjxsfoy.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3ctswvlzz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3nbwpfpdp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3ofgcmrof.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3epxbecwc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3gvfepkjm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3gkybbxrp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3iqaiyvak.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3cgbknalm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3jaengins.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3xgpfuegx.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3onqvfzof.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3adrjxkem.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qfhrgssu.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qbfetdbd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ojqowuvs.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3xpehwakn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3lnftkobv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3pvmlcyhe.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3bnkveiwc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3bipbgusl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3uwoktsme.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3tpdqwjbe.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3acrasqiv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3fezjsnfk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3fmydjpsk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3rnpiswrt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3smncwopg.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3jcuedclr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3awegcwjl.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3czdlolyz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fukdtiha.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gxqqneiq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3uajcgamy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3afznvtfu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3ogxrbfsc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3iiifoszf.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3luuljqwp.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3mwwvmrrp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3szzzuxjh.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ifzzpjab.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3gerqzjyp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3bolcxpen.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3cixmwrth.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3onbczpfx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3iuieridt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vbgwserw.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3xxrpjgng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kaenobif.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3riwyoxdu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3zwpbcnie.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3cutpmcrz.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3cuwapatz.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3cjbrdssw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3ywahkqxl.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3ceslubtz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3zhzelgfr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3nsnldcpb.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3wdcpfsvo.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3fxtixlrd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3pbssvgdo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3zmzixcic.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3hdjlhzzs.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3dsgplncv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3voomvguc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3fcnotsfh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3amzaszzp.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3fqmgmdlu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3suifwxrz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3oyhyyqrk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3vmmkuelv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3aqximphf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3hlkjpcci.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3zkdahulm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3pjkdleyy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3zrtlasvm.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3kbvoghsk.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3uywkmrqz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3kmdvmyit.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3frqvoewx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3hrgpkfxs.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3cwitynll.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3hnglswps.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3dunnbpht.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3ydseckun.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3jfgvmgas.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3vypsltsn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3godhofad.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3xmhadqjb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3dxgvdivz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3uyjtzobb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3yxpzjjix.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3foujetgn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wbpmdfcy.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3smhnpnjg.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mxzsiyfo.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3imaiiqjj.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hnieuumk.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3lyqvnxch.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3qnqefxio.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3fcotdbej.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3qbqpsskk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3voepvoez.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vsdntfri.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3jtxgedqt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3rjsvldfn.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3xefhpmbu.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3twtdgeyy.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3vnikmriq.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3hdxgriml.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3vbpanqyg.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ddnrkmmq.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3zmfnrhsh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3pmvvsbgq.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3tcsxvhec.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ynxfdgdr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zdvdkzph.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3gzkdfvxd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3tfuvbcsj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3illxcchn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hkxaywdh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ysteiamv.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3htwqaxqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jitcwitw.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3tqktnxhy.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3fyhuauem.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3vcioswcw.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xtbgljsd.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3wtsenunp.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3klcpsofo.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3sjzhockc.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3uzqymzth.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3avcpvkma.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3kkgqbwmn.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rudnmwon.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ngzkiagf.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3dhdfmejf.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3vsfttzgc.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ttojplec.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vahvzzkk.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ppkloplr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dgktxxog.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3lhcseyip.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wdoehtnc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3pifxfycu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3phkqikwl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3jdevqmzk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3usybfbgg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3tzlwemff.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3ruwiamkk.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3xvuogpsx.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3cyjpqszr.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3crbzxrzo.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3frulluhx.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zhmjdeye.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hiwcjxry.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3kakiwvhu.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ykpmgcyf.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3zxuisutm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3miegxphd.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3jsvwtebf.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gmojanwt.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ppwqhfhy.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fcqulbao.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3oihjzypd.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3esjqtjov.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3egbcuwjq.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3lsothohs.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3wpzgtlpx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3iegzkueq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3dmrzaiee.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3satdajxp.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3kauthmou.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3bgeodvhx.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3zidbrqrw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3gitiuoub.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3jopnkghd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ubltgeww.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3xsewiqxb.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3rlqzugtj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3vaohpiqt.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ziorhwzv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ofoubjkx.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3mjrieluu.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3ipvxndud.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3aazegbua.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3hnztlnan.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3shlyrtgr.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3wmtrbfhe.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3kwnidijv.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ltgnzzzy.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3uurcuckw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3hezagkwp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3ierredio.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3bfnmddhb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3lvkzgaas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tugmszzd.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3gynskohn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dljidhbp.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3knyaucnm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sxbycvlz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3uwnwpyuz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zziihrir.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3gjvvuzal.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hdjcdwts.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yfrhmuly.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3wkjdqstb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gbsyobfm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3xxozxwfs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3prmbptfg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3iwuvpqpd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3taqthams.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3tvhqzchs.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3rmzsfvnt.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3wwgszyue.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3hyztstsj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jawoizlp.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3teqlrmwl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3szukrlin.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3erkogzkv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3tfdpeuxq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3syfhqqst.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3sggyxatc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3bazmzaag.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3xeetxolt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3wbuxquom.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3otxkgejz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kzmkamzd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3cdqytwcg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bfxemasr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3txvwbmmu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3gynetaqp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3kfsqckwf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3xuphztgq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uqrwxotn.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3fjkuumyd.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3qxsxfimc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bweljdpy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3bqjsaiyn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3fnnldacx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3habygwqi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3waefcsjy.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bheikhvj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3kpfnlqjs.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wufqndhk.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3tejbetvy.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rhaqtbnp.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bvxjyjda.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ednhbqxp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3gmrhhmoc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3bvzikqap.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3hdebzisl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3enohoxvh.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3pwnkhnsb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3woqymgyi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3zuzvtgpb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3hpoiyntp.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3iikdtuul.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3fkhxwcbe.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3raxclvru.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3obtbbkmk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3rvlftmhc.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3tmbtchda.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nzqhyyxu.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3zztkwppn.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mgqqwloj.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wdymvkeg.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rklykarc.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gbnarqka.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3rysmmwtn.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pitusadb.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3dfhziguz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xxmfresw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3lbphrenn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xhteuuzm.html


<!-- 参考信息 -->