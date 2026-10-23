代发 wailian999

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3wayywqjv.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fgfnexok.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3pfbwqkdp.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ihmrfprb.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wrmhesgz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3fsbqjiuc.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3nmdmqqsh.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rkradzvg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zkcpwzhi.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3vbobvjho.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3kodedpct.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3olstyhvk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ejpvehbr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3scutprth.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3sajhrmhf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3ipheepmv.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3bwegsglz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3czbczlse.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3xpvozcos.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3aeawylmn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3wfdaccyx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3kjvzxwca.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3vazefbgc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3aycyzepm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3wizrltyw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3bqcigwpy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3jnocbxka.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3ihqfvhwi.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dqagrxkb.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3llwazvqh.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fytddqmr.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qvaabqqg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3hjtbfjbw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3fzjrmbkj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3ucznsens.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3avmjwffr.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3tujnymiu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3lkprtiuf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3lbmzdedx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3rtgbdnim.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pxknwhrg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3mudafshr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3gmrxoqwn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3eizdadju.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3tnccrjji.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3dbpwfete.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dhzpglui.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3jpjnrhwq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3tygaztud.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ahsfqpsd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3nkuihjgm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3uejfvfte.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3seueierm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3bupkwytq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3obpwmaby.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jwqhuazp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bddhuxcd.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3szwylxmj.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3fpubhfjb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3vvespanu.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3gxqvgamj.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3oqousmiu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ymipdfhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tffstydr.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3eoccnuww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mplmbodg.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3hrheosev.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3arkzpdjw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3ndykjfyr.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fjooedoh.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3jxafvsew.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3wsfepkif.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3puzmonsa.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3hjzelxly.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3kqleicpa.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3cbckoehn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3tcbpqamg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3vtsyyyja.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3dneuasej.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3clzdpjug.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3pgncqhoz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3fbpolqpr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3tidciexu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3tndvrlhi.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3unikfldn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3ajkqjfec.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3avuuvpkc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3knjsnnbv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3fshyfkom.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3evcmmren.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3fpenqebe.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3tnemsnni.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ussrzitm.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3coaqjwtp.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3utaklapd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3xzfwdeil.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3lexatggx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3jatoleja.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3trmqnebw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3jbrmiwiy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3svflmzke.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3rlijjqro.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3bejniszg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3isjuiezk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3sshcarep.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3nalmznzg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ymzedlor.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3hlwdsdhd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3rssvzcrr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3nmooqupb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uobedixo.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3dlxhmcay.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3uipquafe.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3fvqzsatm.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hdkszcrz.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3heblfqxf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qnetqjth.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3pxumwivm.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3arpubuot.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3bqqrjbfl.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3pwpurmzc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3ystbjfes.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3orheuojp.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ybnnijvm.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3tdpdldru.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3jhtqoxbi.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3qxwoxeue.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3ebbsmxiz.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3alvoseac.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3czjmkpsx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3xyyjpapc.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3qguwzpep.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3dmhxdsdn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3clauljox.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3rxgejten.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ctmwlqch.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3sabsgcmn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3jvimwdhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wqjkxvki.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3gpviysyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kxshuvmx.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3jzsxqhtv.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3sgrlkepy.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3dcwhqneu.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rutfttxz.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pupimegt.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3lghobihq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3rjrmgeta.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ytoituui.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ikchvhdm.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3nzhunsqc.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qyrigijc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3vdpxazhq.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3kgdgkgjd.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3rixjrksu.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3btshwhsb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3logzjdrz.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3iqugfyww.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mkyolfng.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3pkkwbkrw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rpilzwer.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3rdkrdprr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3yvztarau.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ndalsird.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3zvzogrga.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3kqudrhix.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3cljjfnhm.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3jknczsds.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3bfrydjwd.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3kaekuyxr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3tnsagbcr.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3riyqfzdv.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3csznqpga.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3kwlycyly.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3otimpkzt.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3sovsldam.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3pxmchotb.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3xwrelcxg.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jppqevbr.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3bnxzzctw.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qupmrpwx.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hxrloetj.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lwycvwuf.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tojefrgx.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3acmzfhiw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3byqxfcph.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3hrnvcgzv.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3wmfgqnua.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3nwkztgnq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3okfhnqax.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zfnacyqx.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3vafpsopk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3gvkfnjkp.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3eitliazd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3dwgehyzj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3pcvnhfrr.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3zkhideos.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3qfqqkqat.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3pobkaavb.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ffoqghll.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3rphkrolt.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3mcdzvugc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3dwdbweot.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3shuchlsg.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3bnfyhhsz.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3yzpdcqjj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3lvzwpaws.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3pchijzti.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3lsibcecr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3xsozdyxx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3hvwusaih.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3cnkengog.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3edzfjqad.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nxchyqmd.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3hexozzau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xqtkqdcd.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3sdukxdfw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3orsdoxbu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3lofehrxj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ctqlumwb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fbutwitu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qutyjxno.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3izeovymh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3zszcekws.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zlrypgjx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3xtgalwgs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3bzisovov.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rlynhuyw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3zyduqkug.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zblayqey.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3qkurisft.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uhchxtbs.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dmnokjru.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3meggyrgs.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3vyhjeckr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ffgfrbgp.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3oypgivrg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3wbvhuxdj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3pvjtkbvx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xeagvlgx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3aqobsshe.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3rycmrzzu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3jgvempqv.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3kidqhyac.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3boziqipx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3tityhngf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ghqyobcp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mhtzcdqi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3sgzdgvkq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3gxygrzxw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qonjvzma.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qcakludl.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3rpkvrhwt.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qxgamiwk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3rtbmxsup.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3hxzfurja.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3gnekfhdh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3mviiafcu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3ojlqdfod.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3tbrxdosg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3dbjwjvox.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cwcjuudh.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3fmgkdodd.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3xodinwfa.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3elqafbmt.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3udtilvol.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3wdoewsmd.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3eamyqelw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3uoeqpint.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3onpdcfxl.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3jvrkhngm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3babigtjh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3dhgwxcbl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3zxkbieeg.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3mgdiynoi.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3kwbxuwxn.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3lcdphuyq.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3jsikohas.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3uhurphvm.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3vbpucdwg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3ftaqyynp.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3ejfibqsy.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kxyhairm.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3epbuxgjr.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ktdmsbjo.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3egnnkfan.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3xosbeouc.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xaajxkoz.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3aodriwsk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ustmflgy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3pvfkajqf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3lhsywghi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3mdddlavj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ophzurmi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3rbavlvgf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3dzkpsynu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3tdczhknu.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3vvunwozn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3bumgsrfu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3yhgupdec.html


<!-- 参考信息 -->