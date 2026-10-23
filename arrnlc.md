代发 wailian999

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3hlrthtwb.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3jcujfgbl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3uqoqrhiw.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3glxkzxdz.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3vkyvujbw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3srpqjwyr.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3znfgvvaf.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eesnkzgf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3gtqzulqq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3xxhvooih.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3blfgypde.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3melvljib.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3ijyeofkv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3udcxwnjb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3xiynxeet.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3rkquwfwd.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3atdnattj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3pepurhos.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3zhcrbaea.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3dyvzgmzl.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3vdlptdop.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3nroizlkj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3jiltyjcx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3jgdqgyqs.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3apjouitq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3hnplisme.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3gfultryq.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3gorijhaj.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jiyvochv.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3oxyovgdm.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qsbbcikz.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3oybshnee.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3paupubfh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3sbzhspad.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3zmqszauu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3lgyjzmgc.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3tjkzcucz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3vxesviwd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3phcfknkc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3bvkolgvg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3lpiuauys.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3qohyejjg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3azpmdggy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3dlikondz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3xvviiosm.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3ravbbwqk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ifpznrsi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3wivttajj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pndghzaz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rqnoeegh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xxvnxgbv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3veqdhmnb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3koyxvnmw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3wjyuiyez.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3rdnijwzu.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3gljfzhrl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bhyoqyka.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3afwsagfb.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ymdsirli.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3nxnjpnkl.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3nllpnxpq.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yecariih.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ccfsvtur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kalrukiu.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3shswwidg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cyakzgbz.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3agwsjpgt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3pwrsuecz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3hmmmdsea.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3pjkqvfqu.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3iewnscss.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3mtxwyatp.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3pgikarqe.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3uyjjcaff.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3ahfnczmq.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3idmwgmvz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3hsntzujc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3njzxjjze.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3olobaeng.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3xdogsvor.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3qyvvaldk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3riazejiv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3qnqnfccy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3strzfnnx.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3mcbubgqh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3nbdktwgj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pjkrhqdf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3qtfitmtb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3gbbhbyup.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3todnwklw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3grddbsez.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3iglzpzpm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3kbwvewap.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3laxihxny.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3tfqdpnpi.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3xkhzihkq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3uvjykknd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3bspefzkc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3rlzfsnqk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3qsfbhzae.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3pjdlopkr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3fjebueyp.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3biysbhdd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3sukogpnq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3fijcvoks.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3gawtcxdd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ivlugslx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3fsffqnmf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3aicrwska.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3hhmspzkz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rzyhjiye.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jhfnzril.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3pqsgehmy.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3chtibnbb.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mrmismcl.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3btdlpcqo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3voipwjqa.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3valjdysq.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3bakcaoul.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3mfhezaaq.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3qpyihqng.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3gdzxrnvo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ymvwhzqo.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3lxhvstis.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3rsozrqyz.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3uiciskle.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3nqoicltj.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3gijiickf.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3dhlmfbyr.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3lejttucj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3khjicxti.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3obhwydxf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zhvkiczq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vwalydop.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3zwgvcxit.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3axdawldm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3oiwbrghb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3acpbifew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kbjhwmln.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3edpueuxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xldvcjwg.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3seqmalus.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vllaldxg.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ugisxjwk.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vlrraadx.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3aivwzujt.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ualbaock.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3qblmqpxg.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3dputjdry.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3fgksoexf.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3nclptnaz.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cqfdplhz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3amlrfolx.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3vqwazpkm.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3gjoakznj.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3syjecxfa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rellvfcg.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3dhywfeve.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vuuqpgbt.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3pggifcvw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hyxzlwus.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3rllkdwkt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3cilezcxb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xkyuywlw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3xyvgblzg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3khknlbfp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3twqvzwsq.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3tjgnzosh.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3eqourogk.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hpglefer.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3wkvpbrar.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3dgrwozjn.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ucmyydji.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3sxqtbhns.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gmuzywqc.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3zawnfszl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3vmkegtje.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3tsamplbp.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yeootzuj.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3fizypwon.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nnrgqhvj.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kkhmriht.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fhfbkuws.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qcmpmctj.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3zxscvbai.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3zwdfnviu.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3saicenky.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3xefwveuy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3npltfmoc.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3znfsgxwa.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jfbzjjkn.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3wafxzleb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3sitegxnv.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3voestiwj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ztzlwbnv.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3vwwoobgn.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3xqchucfv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3zcoybiyn.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3cmruurmk.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3tgqrpjps.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3iqqizlan.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3hujkpvao.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3totntyuq.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3zeqkgvfg.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3auaalbyo.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3qhrrllzk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3brzwmliq.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3yfsjazha.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3cvuumceu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3jyzmuyga.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3gfklbwru.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3sqtzhcrx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3wtgemmud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aomwdbjm.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3wmpbbowf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hxqchbtw.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3dofbekae.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hjovhnwe.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ekrbjfjt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3drxyqhga.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3yaklnhbc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wiyddvpu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3svgqdqnw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3dyyodcxy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hrmypmhp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3gwvcdvpg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rauqmfmc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bmgrfzfk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ucrhhyby.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3oxuvtrgr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3wsrvcrdy.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3rhxhqcyb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qikwogiy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3ahzgrthu.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3qpjgvbge.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3uaywysll.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3uxzlxwzi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ppyvkipj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3xcosjvde.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3kmtsnzzz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ibnuepyk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ealmgffv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3avnsqljx.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3qfplcxbl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lemranpd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3dthwxgyf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qevbdszh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kpytzrch.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3xbvyypuh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3sqbyssmt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bjiowhtn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3awfvksdn.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3sbifdacp.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ueyxgbkj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3iperxiex.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3hvobsdkt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3lgedvosh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3ersxcbcw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3webdfssr.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3iawghphp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3ozevuxzw.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vnhcgbal.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3cznvdyhh.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3irgmyzht.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3orhmhgaw.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vujelxll.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3svpmpkxk.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3hdsopmrn.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ozbavnsd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3tjjqibob.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3dauhduxn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3oomwpuwn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3uttmofdq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3nkqgjzxn.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3konieoim.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3ettpnguq.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3qczkvkek.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ykypiqnn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3zcvxvggw.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3cvosugol.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3gsqqxxok.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3sybrmvsh.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kqtjmfzo.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pxqdkxra.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3abdkjfnl.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nzkynneh.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3wpotsusi.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mffqzuni.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3vptgramc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3swxorozx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3sbyfiblb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3clclnjzm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3kbstbaqi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ecvnhccr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3qjobirpz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ishijkje.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3zjrqjcdj.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3skpmkvox.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3auximpjj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3klebktzb.html


<!-- 参考信息 -->