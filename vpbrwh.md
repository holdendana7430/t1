代发 wailian999

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2uenizhrq.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yiwoxsji.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2acjrofoy.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2jafxpkfr.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oppthuea.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2izlbbjgh.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2ditrdfch.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xftbbtjx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xfvojbix.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2idqgjmwv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2aiseyadx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2mxztkvez.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oqphkqtx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ppjvrwas.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tjmttxnp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2zbkqlfqk.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zjbwyyxs.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2alnnijnk.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2qdzansba.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2fqwlwnyk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2mabgzhno.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2vsgahfpy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2yrlenwou.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ockiffbl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2zdqcnonb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2qgwbwagv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2eihhrqpq.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2gsyucdgh.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2wctthvli.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2upvcrgra.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2okmiyimh.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2olxvmgrx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2czyrilxp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2tmkpkcmg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2qurdrfwb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2rctzutbr.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2lwnqqlpz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2hhsrzwtj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2zroixuqe.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2knlmqmkk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2oghutawa.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2iitxehax.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2idufmwam.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2dzliigrx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2pjbomwbk.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2rklfdahr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jvxfamxj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2lyjseuth.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mrkcjoqt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qltsgvbr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2nffoiraw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2bjrisqbn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2vjtlhebm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xgfyjtut.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2qtvpgqqz.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2qwpgeely.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2xzmjaawf.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2fdotxryc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ywcwdwri.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2hjywrufq.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2wevdvlkd.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2inmlqemo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2eduokqmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cqjuwguz.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2kvcthbem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pqfqtbvh.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2vxwhdifb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2gkmzwrwi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2bljjpera.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2hmnelela.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2gfsreyws.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2tpfjqhbg.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tgfgxwpg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2edhcssse.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2hchtonby.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tvasheqz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2wtxduoji.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2jaftutpi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2qtaznjsh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2jsbbnfcv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2gwehpjph.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2kzjrpwdq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2stiggotf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2xghqxhjn.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2cffofurh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2frntjcbc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2suyhldjr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2velunjdk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ccawzbhf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2mkxcleqt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2mwcnziyl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2ypmikphu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ioyowxoz.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2mbmkkklo.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2ehdmkohe.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2smhntgjg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2bxdnryfg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2sdhmllru.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2pkokmify.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2gkcsyilp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2hrsvqdql.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2enidvwrq.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2rlutfbzw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2osrimqeu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2jynqytat.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2bxlhovbh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2vnkqvdzu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2zinbocqg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2mevskogb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ilwjaobf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uptmmmpj.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2ukndjgfw.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2jqiidxfa.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ccmkuirh.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2psveibgm.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2skxfwlat.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2fbcqwgjs.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2erhvxsyu.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2anwikdsz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2sujzhpym.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2glddzuof.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2ohopaopg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2lhawepxe.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2msjbzsnu.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2utvyhybc.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2wqbnaanj.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2zpkkcfyn.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2vzqcpowd.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ckjopojv.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2tqbicdfl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2rcdtxcjl.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2bpmogwoa.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ixyeonhd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2jkspyggw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2nbhtirqx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2fxdwhwfh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2yyjluxab.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2nnkmbkzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2biazksqz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2eantckoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pigxrwez.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2xxtazucp.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2hfawahma.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2mkujimuj.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2htqjapfw.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dvomhjpd.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2uuesdxlp.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2dqkkdqra.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ushtkmil.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ypgyriaj.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2usriacnu.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2icacapxb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ukfipxdv.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ynzaehjz.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ihndsxml.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ncdbljym.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wkyldedu.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ahjzsllg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ebwgfzke.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2wujcxppt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2nlmmohrx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2qeszgnfj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gfewcykk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vqeagrgv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2rtwxgzfa.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2gaisrfkq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2rhdlrmrk.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2vdavukws.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2xqzkhpgv.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jibamfvo.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2rgydkujw.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wjvgvwnc.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2vadiuans.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2uuwkzyrr.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2kiqjwlmd.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2tzvmjjuz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2hmknwlzm.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2jrmrgxit.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ekwoztpb.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2logcjbdc.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ptetyscw.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ymwpzxcp.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gtzoglnd.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2twmfazkv.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2kwboxfid.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2jqhcfiph.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2ecrjmpwz.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ykpouajg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2bdgfgqik.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vyjvmkru.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kpciavth.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ptrzvfyj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2akwlvntc.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2bdmzzmhi.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rficurog.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2lujhmyon.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2wpxlosrf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ltijqvmp.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2vxsmbgil.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2yrcboulr.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2tfygvois.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2bpsgqboi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2twswndys.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2uahhdjho.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ybftmnsl.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2lfrpochc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2gqfsevyr.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2swybazbd.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2oecjeyfi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ryebtusu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2wsjmegkm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2qnhdvrto.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2npungvnh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yvibqjne.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2recassij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zubeltjt.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2iknxsrzx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2trynyvng.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ejulayeh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2icyldayx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2dfhvhjzj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kesdbpya.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2boctljsy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2syxqdwlb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sajrjsue.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2mdhpvhnr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2xtjnaxpq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2sbibbeue.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xofxkrcz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gilqafiv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2jljhdrqp.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mgxxsjye.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2yprjlimc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2egynldgy.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2jtthdeku.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2owdtcflk.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2tcksbkti.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2rfkxrknw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2kctmycte.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2yzlbvhbj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2kgaxdckw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2mvfrfpqn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2vonrrjpo.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2ubryugak.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ludyqehc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2qwcxtowd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eisddgks.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2auzszjns.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2pqqjlvgp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2mqcsndlg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2btuxzhil.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zpwyztug.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2dlznwtbb.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qmjathlp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2iqituprj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxvppzrc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2itgrsteo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2jyrxggcs.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2sefsmrcn.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2wnvhpgfv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2nqwhwjrj.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2jpjejnac.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ydekbidq.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2laqgtkrv.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2knskxdpj.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vxgzgsos.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2bhsyjzgx.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2wbpdxpvv.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2prkozhco.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qdttdpvm.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ooelbquo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2gjivmfwq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2jxvpqhdi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2vlfxtoki.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2lkicqjir.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ehviglhp.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2hlrfnrmd.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2nkgyympw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2oaeoxila.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2uwkwjwvw.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cuiqdvuy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2lmsfzjcf.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lthhytoo.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2inxhpltd.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hfszngjn.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tafpcwtn.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2nxwvuxdi.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2idnydsci.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ocrdqzow.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ohbdwkxq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zfuzjmca.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lozssexx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2avngodco.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2kxprgjgv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2xgzkiyjf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qkvpupfz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ovesgmae.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2kiwvzwwc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2hpcrngsm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2chjwljfn.html


<!-- 参考信息 -->