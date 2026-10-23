代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3vbvkyljq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3iwndtemt.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ykvugmpe.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jvcjlhba.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3mdbzjieu.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qxmtjgrb.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3rksxyiyr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3hvbfuugb.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3uaqcruhw.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3vscrqapk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3zkemfxqz.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pfplpitc.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3jfcptzoz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ypobifue.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ckzvycfq.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3lowwlnjy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3huqhlcix.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3hoxenrmw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3gcaktryp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3gwvgkcck.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3wrvhejfa.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ktkqxjvz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3trnurkba.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3dzqrukmw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oclksnle.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3urocloph.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3qrxqyqxy.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3udamqgbp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3wtnqvuza.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3mfxtlokn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3snwvrzmt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3vbuxfgyu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3wvceyclf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3oylxybjp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3zzloepmx.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3horjblry.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3kqoxvpqy.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3wrtcdvup.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3dxtglbtk.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rwzltipd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3exujirbh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3iztivncs.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3kzsqdquh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3ctipbivn.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3zwektbkl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3tuesczui.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3twsjtdkz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3mjcdidbx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3jgfxgdms.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ztkanljy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3qwflqicz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3jpzpeiil.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3sklxldcx.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3fvkyxhvi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3edwxrnsw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3sdqrorfk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dtfttbsi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dkncqenq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dwzieekz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3qskygmzx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3qkkhsvcr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qgxgdpbg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3kvlxthyg.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3bbqagrws.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qxkrvpdr.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3enayepmh.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3qbytjrcr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3esckkbvh.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3zqtmeytt.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3jmgecjbj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3hanjcadt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdytutxw.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3kklbsieh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ocndhjwz.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3xhqogfrx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3dtplocfa.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3iskargdt.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jgswzstl.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3oexphagx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3fcvhciol.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3excoynnh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3crzqkwxb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3gydhqdbv.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3odxaooqg.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3vhkccmrj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3gfyazpju.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3elupyhdc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3yjkgqfam.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ojrystjj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3tanaxpcs.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3zatmxokk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3bmvowziq.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3dikkoahu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3bcnsvkpt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3nlfrqrle.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3imzchugg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3uhomnkip.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3maykidjt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3lwlcqasy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3ztszijau.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3rxpxlszj.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3jndlznxb.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3znuabkip.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ixdwjjoj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3zrdtbkhl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3iombsvql.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3jlnvkozq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3mzyvoxzu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3qjcperuw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3rctpleoy.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3ldcznxto.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3ldwsyklh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3rezqpusi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3zpmoijno.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3gjetvjcd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3zkhapsai.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3lcakmadv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3rpmodgtv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3amofnrtk.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vjywgxbn.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ttxxrhjn.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3wppjfrou.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xoqqxhfl.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3gtlqdwvb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3luaetqle.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ddojvhao.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3wvcriacs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3vpsnzemo.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3pdfpzgva.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3nmmjierz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3pnsnrcxl.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3xhamqulx.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3detnsqvg.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3czfpuukl.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3bsnjlskt.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3jyimnwrc.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3yfzplbze.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3jlpdqmfe.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ozcmqrbh.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3olhtlxbi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3scariybo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hnbeznin.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3ehstwnrn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3hcnkojqg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3omqoodis.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3obuevnkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cnxrfqkw.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3hebcrfio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hloiwhjv.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ppwcveub.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3rizssxye.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3qrhzydmd.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fyumtrbx.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3vksawkhl.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3oywgobxg.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3wzrythyk.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ugykuklh.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3gponbbcl.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3skoidjvm.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lphhrznc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3jajeagng.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3gjcchfya.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xdybefot.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zzltsmdq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cwlyxbro.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3rvocqluj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ksivozwd.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3ekbewymt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uizzktoi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3erhgmrqd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3daepnubx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3seoemagu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3jejudyhj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3dkxlioex.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3szxulnqw.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3fxnbduzc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3bwdjspud.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3srbujswe.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3lxklumaq.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hkvqrxcv.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jqbkvltp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3offuzxwu.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3widnowde.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3rxrhqqhl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3qrfznmgi.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3dedafqzd.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3exzbwcku.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3aoeplvcn.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vbzogtgd.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qfluwlus.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uxljnbyi.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3boyrcuya.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3fchbpwys.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3xoopuzwk.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ppljohaf.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ssorpnqo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ypbmhhdx.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kksobhae.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3oazxjysb.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zfubfshz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3imalyusy.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ijtuheak.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yyihdzyh.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3mbcvyjkv.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3pvxpmwvo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3sjuupeid.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3rwoxyyzy.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ehmsgwaa.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3jrncvfkt.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3zpdyqmaz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3wfozwuff.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3rspimsjb.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3qecheiju.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3zcflxyrr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3whnrxeyb.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3jxcqldfx.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3nmvcajgw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3nedlzlmn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3lbmntbmk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3zrtmzoin.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3mdcktgnz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oswsozkt.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3wnkxsoft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mkyajemb.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3laowtbpe.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ostqjaoc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3svrllkgh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3nclbhygv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3sjlrmghp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wgzahskm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xtvaefkx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3smitwalc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hcjgcfgs.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3qigsjqup.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3yolvpqay.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ibqmabin.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3lwceksoc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ivkltcun.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3tnxnciwa.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3uvftzatn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gwmvvpnc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3webhakap.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3wxxbwnko.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3nwrwskuu.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3ivtekmhy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3oarooayc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3vdwmuqvh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bhtbjucc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3ujodwcwc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3nreyfqlw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3jmwcufvm.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3qlibkvdz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cmaktswv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3bqctvufo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3lzoazxur.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cqfagfjb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3tbsfkskp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3rvpgloac.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3bsxwpooc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aphbdqtj.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3odusnmcz.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qvkjkirt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3gzzjexjq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3bjbognsx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljovoulw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3rhpocsoy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3aayduejw.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ycqdplce.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3ztycmvzi.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3srcwopac.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3rszqrune.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3iedaodrk.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kekcrlig.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3atjhuwug.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3uejlslpj.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3goipswxy.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3nnhpxxbx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3dsanytgk.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3qjqvkazp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3njbgdsru.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3oszbksod.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3xxrfggkb.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3bbsxzfxx.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3qgdavzqa.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3gpmafcbj.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3lzhwntdj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3bxkcxnyp.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3edchcpll.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3jvatrzpl.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3gcsvthov.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mfxzwllb.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rpqjcleb.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ttpuahbs.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tydlldfb.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jfuknzoi.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tdjuzrig.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3zpzpequf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3lxnodwff.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jrmbvjtc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jmgqoecl.html


<!-- 参考信息 -->