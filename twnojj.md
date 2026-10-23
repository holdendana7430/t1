代发 wailian999

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3poxyxndv.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tqvcephf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3naguycvi.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hkwbjsef.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3xrxkekyx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3uahabagn.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3cyyyzubh.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cxnhoivv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3aqfsgkbh.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3irtlnkbv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3utgdeqsa.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3zlqhtbfs.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3olbudmum.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3yknsclnp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lnfdklzk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3cvrvkfvj.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3habyhzfu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3dvhifycs.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3rxfqcnba.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ygxttcij.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3nbznyveb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3whidajox.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3bngsfadj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3vmfmaolq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3qiatgxqk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3hthyugct.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3tjsibvyf.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3hdliwskd.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3naziirqc.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3qjzvbfsy.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jqktpysm.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3xrwkalec.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3sdckujgy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3ytnqsdmb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3axytvzpo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3rciruves.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3dhvqwqbi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3zepdrlkq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3injfhefe.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ujiksdxf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3thuzlhsa.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3zdmnuppy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3crvmcdjg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3lkcecktp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3errltnae.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3fwptdwxp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dkxmeinh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3idgauyft.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3konddqcl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xsyzjgyy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3chpgacru.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3sxhssyqb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3absdxnsg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vdtdeqkp.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3khceolve.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3lmxrgnhh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3qgtejorq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3vgxjrgof.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3shlemzyf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3wikndiyv.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3yzxxcyop.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3hhdwedqw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3vmydlbeq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pxnshgpr.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3ynccfjno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fqjhmqlg.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3sfkvxwug.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3nopueeou.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3uarowghb.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3zqqoglzg.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ctphrltg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3mucbhuqh.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3tbjesbsm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3nqtmnboq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rtukjipa.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ehxcxnrm.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3huxbadxb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3lvdmhvbk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3vxfofjbe.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3qiokwecq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3ntadrnqd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3kvzclhes.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3pmlcoqos.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3vjflnhfp.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3awevalzk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3ygirafgi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sdaecgrw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3mehdkazm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3jybzmoju.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3lnabuanb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3rzivouhw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3dwwkxvaz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3dzqcsyig.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3ymloqnpp.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3lxjgrpwq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3tvxvyurd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3vqpnjstw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3xprnutow.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3fvnuvblt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3exmxxmot.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3frrzoptr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ihbdhfpb.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3sjfbxpkr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3bgbkbqyt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3qcdrjule.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3yzlpvczf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3cxedllwu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3qwwyndof.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3dfgdnzxp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3xeegiwlz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xwofseeq.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zcavpzol.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3skmpkxwh.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3nghzmjik.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3hcxqgqcz.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3fcttbcts.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3pzfasrpb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3gxovzzqc.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3bwrcqxgq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3wcbizvpf.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ddjjdrul.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ccvjkrfe.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3quwwrbse.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3yqwqnaca.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3rvwohdwp.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3bmgrmxka.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3huqjuukw.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3jpbxzuzo.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3xcjmxjmy.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3ykczuvfy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3cdzpzwwi.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3ryrhfjxm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ywdaevbs.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3udhxynbk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3tuafsbdh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ymojziez.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3fjwocrpa.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3jxaqppbr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rsvclgme.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3vkjocecl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yggrqmxu.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3jrhsqpeu.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3kistbvnh.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3hrciycyn.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3mlchwghs.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rfjvepsl.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3edjpspzk.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3uqjtyppn.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3luijcexo.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3jnspldpo.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3krcfzozv.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ymldellz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3yiarwyyl.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3muqvpytc.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3unykwszq.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vyfunrqv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zwhuqurw.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3zbfekuwp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lefixmxi.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3qfmznjbv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pvltstrq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3keaxhdlo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cijkscqr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3etjkioka.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3rbovxclb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3kfbhcudg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3cenlyyqd.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3nrfqldyk.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3mxzvvbam.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3vmndydsd.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ekbucmuz.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uorjqeyi.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3owwykkhs.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3qcpqadiw.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cfaypdlo.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3ixflxdpc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3cpgpwidi.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3axuwaxtw.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fihnvujv.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3yjljxgkl.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kricnysn.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pqmpqxvn.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wivyyshm.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gyaldhcm.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3oxuhdzol.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3zyccdesw.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3tqbqvwrp.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3qpufdxrx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3toebwupt.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xjdkazko.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gxlbslit.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3tiuihfdj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ltzwpqge.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3wjqblfhe.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3tycukuxu.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3zktvetge.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3fmevgqzn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3cxtlgrjn.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3uerrxtjr.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3tbcfpurl.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3mwzgbano.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3ierjbmyn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3wdbafojq.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3nbvprono.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ffuelgea.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3pzxjecfx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3qsmdmovu.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3odipdnre.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3injkaanc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3svtzolvn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3ftkqfreb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3lhfnteeo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3avhswnuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lietilrd.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3taqnmgwj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nxkeqvwc.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ictuuxxb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cehiphtq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bqioepzl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3srrybusn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fkjsappo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ncpmphjm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vnyqouvd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3wemecgrc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jpuffjjp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3joblghig.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qrgvfzeu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rfommvei.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ivsfkxcc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3igjtzhau.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ddmwfflm.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3cgfemdke.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3pyelykrh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3aaipldrb.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3ifvgcfez.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3lfbgxzwa.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3zvcsvgyk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3kcciyefo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3usazdtlq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ghqpcscs.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3bdgbtkcc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3srbiwbyp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3zppqcgxs.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3urjqqlln.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3svuigxex.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3xzcvwgnl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mcluohwa.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gagdrsww.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3nmvapcnm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3trcgvavt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fkukxiww.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qdamoujv.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3kveouuuy.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3oswjlvfv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mavgqenh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfwgwodj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvxfkmah.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3bnorqpve.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3janyrdag.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3szrcpypv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3xaslezeh.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3ochwuyrg.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3jxhfrwem.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ygolhszt.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3oryjqxtl.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3amduvbpq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3fypjvonp.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3yfullnyf.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hjlxcozb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3awwypplc.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ubzxejcm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3fsxzzhmt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3mkwuflyu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3eiuzorwu.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3mbpdjptm.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3yzsbyckq.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3ywxtvwkl.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3kjufxfaz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3vhzpfdel.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3dbibfhqq.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3rzwiemej.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3rgxhkgdd.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3easeimlh.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tolbrokp.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jmxsqidw.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kcncdrdv.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ztkwjivy.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jufnxmfv.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3exyjvmig.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3sunheleo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3gcgwfpso.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3aoslffid.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3hhjbpkrn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3eaevmbns.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3fnwxrfud.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3honrqhkr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3vsouilqr.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3kwoxfbbl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3tmaekfpn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3bbfhmpyl.html


<!-- 参考信息 -->