代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3pmjnogmp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wltvfzmg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3gysmqwdu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3sqqkxtss.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3svdecyly.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3lbysjyzr.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3iplfntwi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3gbdgfxqp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3xymiihxz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3dlegvbab.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3xqrsqyql.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3skdfirbe.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3pkjvzpne.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3slwbpsto.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3snqjigij.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3aihjbvvy.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bmwxyfyq.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3kxvyqjcy.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ypdkuail.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jssjotog.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3hekkdgtk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3spwftitv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3alzheeev.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3koiffdyr.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3udmplczv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3qtzvcins.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3sywwlpsa.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3hzhqhvee.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fffdmlbh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3gynjofvg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3fkpshrez.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3lrbimapw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3mbvvenbf.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3mshilshs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3khsfutwp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3qdhmhcph.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3eenwxhji.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pjtjodqo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vqownfaj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3kquvldyj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3mypoeobd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vzchectu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3yskcsdve.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3wuerukhr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ehkxbfxt.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3htinqwbg.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3oscpejdm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3lxzxaaeo.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3vfwwhvtu.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3xlwbeddm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3tfmsaecy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tugssfsg.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3dhqpoiqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3itkdbbyd.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3gionakca.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3ectbaeyj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3cxohegxk.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qdxwrcnr.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3nzmpfawb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3msdtzbbi.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xinbgvjb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3xcrgatid.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3kfilmpwp.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3hzyalqqr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ztqiirlv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3ktvvrxyc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3oybmzkpj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3inxnuklv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3ezwfgfly.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3fqntsfvd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3qaznmjuw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3gwnwfofn.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3owcijkzc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3sumphjtm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3urekuorq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3knvmfale.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3hgjhjdgg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3ievivtwj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3igbcbdxo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3eatofuxo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3unbwjnaw.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3ssyicuop.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3fpcfubhb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3lxvzfgod.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3nxjezzdb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3zifhjkzj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3qmfetzmw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3jkheokoy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3mrsqityl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ltiieeds.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3dffonpcb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ivdrzsku.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3wcepuchd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3mqiuncav.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3rnxkwpme.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3ajjhtjss.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3igxxzcyw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3zycuayoj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xfewnuna.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ifcwradj.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jmmhhyjg.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3npwllosa.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vysexnfl.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3spnxxwel.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3swqyznzy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3wqgeyljd.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3gqewokhj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3jtagwqjs.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3taacdall.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3jyrxbwyx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wotcajba.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3qsizkdfu.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3gyyzihjl.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3aijcdxhl.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3osolsysy.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3cqzkbbhh.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3vsnnirhb.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ojflxgas.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3pnbibpia.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3bcixdedu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qwvdfgzb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qzcrdxlk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3szlkctlr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3vgdrlemc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3edwgqzgp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3qflhyonl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ialxtaia.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3sicajnel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3msumhnkt.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3vddmqqha.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3gwmppdgg.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3vbmtaumf.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lgciadeh.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kkklgefi.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3tvtzykqz.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3scpqgljh.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3hvbblzfw.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3xkeabfxu.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3nuiofoea.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ygbefqhl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ietpolju.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3bmklzzoa.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3myjggwie.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jgevnobe.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3yvxnuxia.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3sziekizw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bbbumhgr.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3hkjjcgrl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rtegzwyp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3txeqnyey.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3fzgwsgya.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3okcfpqcl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3gmaunybg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3fkbgkbsc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3nmnwadfy.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ansncaqg.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ykxlkymx.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lobteqlj.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3hinhtkvj.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3yojqfnkv.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mxnnesfp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3jfolqtam.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3csefeksa.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3gvkqvcmr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3pmbvlmao.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3grfjixiy.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3crpgzfpb.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3qxiebovz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lzxbavfv.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rbxpujjr.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fbszebiw.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aonoctcy.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ktdbgrxx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3mlynczhj.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3dcntmjmk.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3qibfyoeo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3fshpbnxl.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vpvifdgp.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xztxppnk.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ehxatkpe.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3nqpawmta.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3tgwelzmv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3baxrqbei.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3kexegdqg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3gfxfsdkm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3vtfbradg.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3tphgrfor.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3dxqghpij.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3mrrtftsz.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3dzcjcmes.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3jfnckjtl.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3hrbdevpf.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3dvgkikrl.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3zqrouarg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3tbpkijan.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3dtukrfca.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3hzegjcbe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ziqmaipp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3hynemose.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3kwraoxyq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3nqucmsbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ysovtpwu.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3mcbuslma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ttwclsjh.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3hlourrku.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hwykwclk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vzhnrfwl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kzeneilh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mzhkrmbk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3szpzlyyr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mlyvrfyo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3zrispsqt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nessybhg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ldhkomwv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3aoipjtnt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3cmqaelpq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3pwxociuu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3tasmtzgb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3yvgoseqt.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3gehvcdwb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3wrvybcui.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ioesnewy.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3meusbsed.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3zftmnljz.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3oixfybsg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3hrifbpkf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3dwsqbzod.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3jsblzvpv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3mjactjyl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3gkqhcplq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3lxavlpdt.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3cdhikxen.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3buwwqhmr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3qxfktheg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hzinoicg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qubjlnsw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3hajjyhdj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3opkigsdw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ddmgswar.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vdyoyngz.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3imetbmbt.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3cjehfutt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ocwtxxqs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqzyiveq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwtsxkwm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3udjejrqo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3xihkhlsn.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3shedubnc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3qetnboxs.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yzzvzspl.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3pofcdbmp.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3stpgjoth.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rcnaxpjz.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3danispef.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3zulgtwhe.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3pczuvmbw.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3gbhfrmnp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3vmextzxr.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3kzqrjqlq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3cdrrtmze.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3yiaehzvz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3noztgobg.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3envacpjd.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3jzsppjam.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3rxrxbywf.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3genqzioi.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3hsjxztky.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3hzmrjigf.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3xwpqtowz.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3kwjkltgn.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3iljtkhln.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gbxbkzwm.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ujcrsaji.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kqdtjaad.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3enqmyixu.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hsnwzfuw.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3kislnnbu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3xkfmkngj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kmddpjts.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3abdjtsix.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3irnrsvzw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3sbytgckw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3hewrfsaq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ghgdbach.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ljcaahnc.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3pnrvayvq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3sxmvoidn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3wqubifyj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zdqmqzwl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3prufggze.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3fzsxazwy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3zggatqed.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3jzydajfs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubhsrvie.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gftoufva.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3rinwrmwj.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3gfalnedw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3jsbmypss.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3dfstebbq.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qajemkca.html


<!-- 参考信息 -->