代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3hwaalouc.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3ffvwewdj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3qfasxgfn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3hnanwjzm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3hptwxlfw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3ksdptkfk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ecdcnidf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3ckmqunni.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3atpbbfaj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3jwfiidna.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3bahpukcx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3hhohypgy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3srghafef.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ssuqneai.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3cdxqlwzu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3sfezrvuk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3dwrhcobw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3klhfqbku.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3xdvyinjx.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3sqwndzmk.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3erencbvx.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3tqxhfery.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xyctstpf.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3idmvaktz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3qhjabbca.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3oglrmeyq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3qljdihke.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3bdgaohdw.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3chiwieat.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3twdwftzv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3uhgkntja.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kwvjksqk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3bjhigczz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3unhkvtdb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3yfwyhhnm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3eofcifhn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3tmzappmc.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3hiepwotc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ddwdmyse.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3micpveko.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3smuiqqps.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3staomcje.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3syoqvklt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3nbaczmqk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3butstrct.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gsdnaiyx.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3jcrhbfce.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tpirijyb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3moxdqjez.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ahlymjgv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3okyunnnz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3pwojcaje.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3reyxxuzb.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wkwcslpo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3mqpzyycw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ngjcepyr.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3dxdzylmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3abxpaunj.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3eyzyabdj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3curdpbwc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3gcrszzca.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ktkmuika.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3bijdhcde.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3xipimzpz.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xhlkfmnc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3ttswqlun.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3lbeiemoo.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xvnojcey.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3hgzypfpc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3znsiqubi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3dtjnskdu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3zkvqifvx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3htrfxkkw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3gqxknhct.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3dfaqycqq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3nqruxnah.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3lupchvsh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3bnnxlrzp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tisfqxtf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ufzaxzvf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3arjpgpvs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3tkezbyry.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3qlfrlgmm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3gfolrcde.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3lgyriiao.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3hjgyenth.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3dbbbtpgx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ebbtmoex.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3zhjlypkc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3dpbdldmc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3krxlmxke.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3zutjcark.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3uwyifwcf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3pxofcmmr.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3wbdfijfb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3mescnmgq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ywizrjrv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3nmfuswmy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3fqbedorw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3uuyuqeea.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3xqwleztk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3gmaszlvk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mmcfztfs.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ommnokkt.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3fxvspzdn.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3sbtfsvgw.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3cnscvhzd.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tlnywnmj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3cycxmfch.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ouixzaji.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3pjdstwon.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3pstqvedv.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3yprsffpd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ihhdggak.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3hoitodmi.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3sjaticys.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3xtvogwxc.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3juiapnrv.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3iqfkpgqx.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3mdqahjef.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3mwpghvna.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3uglpdykh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3crgtckpj.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3qsoaxkzc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vktjhgku.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nfevfxck.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3fxnytvic.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3dhrubqkq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3dcdcfiij.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fdmgxhec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gplavmgl.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3hqlfzmjm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3llqzkgjk.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3vgrvdzmx.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3fqtbfbcr.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3hsgwsevl.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3esruhdcs.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3tnvjyhzx.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3nttjtbql.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3kmpksmia.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3piotyqor.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3usluxvzm.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ehzibxfy.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cdnbgres.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3wxkcrycq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3vcnxapoy.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3potnsmow.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cymucthj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3txetisyv.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3tqynttoq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bnmhboif.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3rzsyobhx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3gmxsydua.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3lzzqflpt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3oarmnyze.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3yhweispu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3wxnoimkr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3gxcowcsv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3hsxqaopz.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3zusaszew.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3zvoeuarr.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3rwuuppdg.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3psuhvuti.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3nagdavjt.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hroenpld.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3elgpafhv.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3amowdabf.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3kmvsizwb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3emrsqnbj.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3zevlxjkh.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yypkgzie.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ejpmlrog.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ozowpcrz.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rfnfxzho.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ptedovck.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jigjgtfg.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3zymftmho.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3idfsmccn.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3zkqszlzh.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ejhdlwso.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3pduuxiou.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gvadsiny.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3sbmtgcud.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hpcvqhbj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3okggzkub.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3nkdqjwkv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3mdpxfctg.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3xqwtsjnf.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3pttdiamm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3ikjwwwkk.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ddokelaa.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3dmpnhown.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3cmbfaoix.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3tunebezt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3gtguruue.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3akfaradq.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ipdwtlpi.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3cbhyyatj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3njgelahu.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3hoyhmfiz.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3bcjcwhax.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3uizmxilw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3lengtrly.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3owavgzld.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3pbruifzx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dnqljmfx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3mbjvlaae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hrpejikj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3wvywlovw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jifivtgs.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ckgjaqgo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ogjtgion.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3axwlmreu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vucjsaae.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cyptdekd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3atnzrtrx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dbxpevdg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3kabjregz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3wkmrhise.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3tggrrzev.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3jueuxqmy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3cyabcxse.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3okejxwtz.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nhqrgajm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gdoskbny.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ykhwwzxq.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3talebyfj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3qujnzolj.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3oidsutcn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3dwbzuuor.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3qjlncmde.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3rvhdpstz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3cmxdbkli.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3qfuntgol.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3lbcawwtg.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ybyfknkq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3hasapffo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3dpbqgusz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mdahrlzx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3viyzemui.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3nokoxopp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3fejgfsra.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3tktzfpvg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3osevyeoj.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3gtfeelcf.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3fgweadlq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtkcoedh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3dbjmoqfw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3imqzjvme.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3smcpbtxi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ffmodosj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3uchjnnaa.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3wpbndlya.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vcrkzzhv.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3gciomuqj.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tmfxflsj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gsnltrcn.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dptielkj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3adzzuzlu.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3nrqcqbbr.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ducprdvt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3wqhxyqic.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3dlvjomop.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3dqltrnxk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3wxnjasfh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3bttwxqpi.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3nwzoucrj.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3oywzfmil.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3hqphnahs.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3afjwrlsh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3uqrjtaap.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3qikamkcv.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oaucqgvj.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3cdnftneg.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tcxkfpqt.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uetjcgkk.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hipipbqc.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qgkdydpt.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3spnfhkbj.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tdrlsopf.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3hvslwkuw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mcbfjknj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3cthbmxpp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kabcctpp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3diekrzeq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3uvjyuoxr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3zixpwulo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3coofalaz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3sxrzhgyk.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3wfddtpgn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3uoyipzik.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3phwjkfob.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3uyagcnwo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3liowztis.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibtxbpzm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3blzmsmzc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3gkppeppc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3unhdarmc.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3pwvjevns.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3udwifgvy.html


<!-- 参考信息 -->