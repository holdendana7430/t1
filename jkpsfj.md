代发 wailian999

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3blyomcxg.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jekptnjq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3jtfnevxg.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wcpekmgy.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3zudqriir.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3yihffmwz.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3snzkssqd.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3eksevaox.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sqcvugjm.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3liwgoejm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3xitemaem.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3sxoiueyz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oxltrqef.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zwsimyif.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3gyysbjsd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3slowxaky.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xnetklga.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3ilyhtkxh.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3eglorzmb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3wvcjrxzh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3vpfkxvzj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3guozfroz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3nifhuewu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3txekpqli.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3lpsckufg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ktxjejct.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3oswbxeir.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3phrqihmf.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3gadmnyyf.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3ieqioxeo.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3bjztngox.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3jfylbndt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3zvmbeqjs.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3bubdlwoz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3bslwtetq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3mtqugmgd.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3sveydgqq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3bbdnkllw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3hgkbvcun.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3bmuekbzg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cewewtrn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3jtyznhhr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3wtlrqrio.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3gcwsixoj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3jbtamfal.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3yzskxqhs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3wofwgiwh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3lmbjpylg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tohygacv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3koxmexru.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3numsmxvq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3jpmdgfno.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ugnkgrgj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dfxbrhso.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3mjsfbkdw.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wzmqsvpb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fhchbixj.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3jnftoqnp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3rquhapme.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3njgvnkoy.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3wmfuqjrt.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tgifwqfc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3gecezusr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ldxnzxyb.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3yyhsblop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oxpokhzk.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3uvwmtskc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3qefbezdf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3pumtxgua.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3lqdrpboo.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3dzdobniu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3bgzyagxf.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3iytkiofz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3kawzwmxo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3klbzbite.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3skeorwpp.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3gljbgkgi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3akjhoqeq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ppmzxdhh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3qomajyfn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3zvkmkcgd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3zzpnxlid.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3ugqykfzt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3vlplmiul.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3izwcbtbe.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3tkletsqh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hauglrhi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3axqwgvui.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3pbzpsfzw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3vdcfuxik.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3rzszcgcq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3stakjlag.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3zacwyisb.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3gpthblto.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3wcgpsemh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3mmgegtty.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3dbuxbhjn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3svmchlzm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3uqkvwfns.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3iqyclyul.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3dszuqohp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3zefihnug.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3ordhcyus.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3iexczsou.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3pgxhduef.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3sznkwzmg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3shlwabym.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3tqkxcaxu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3hyzaorzq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3miukmdzy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xvthpmoe.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xujspsiq.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jsbvjogn.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3wwbvrgau.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3wwjxhxej.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3vxaomtpi.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3tjylzzwm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ryqmkntx.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3svsbdnwb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3zjhzauik.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vnfobidu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3xmdsnqvr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3clswuofw.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3kopojuax.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3oqnbuvet.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3lmayaesx.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3crpbeiif.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3kvzibmvb.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3hnvpmacs.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3qlwxbxtl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3qrmgvwhm.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3dbnhuieb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3yguifbra.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3wnxiyhwi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3gbrmcfoq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3iisrethy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3mlxxhasr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3slemxanz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rjdmolrc.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3svhqsxxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jvvccnhw.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3zwqbqurq.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3txqhorzj.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3yqlmownv.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ckntsukb.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kuyzmhku.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3xydjyogg.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ranhydea.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3zedqpzel.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3kdzirspo.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ahjnkpda.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gwtnhbnh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3nduixwme.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vbevrdew.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3kqxjnhbf.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3uhefqyde.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mjvdwkxv.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3xcxqfpdu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3azykjamr.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3gpwvavag.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jdzaxsgw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3jrocytzr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3nmmbpoio.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3stlsznra.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3xlioryof.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3jmufmwgh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3imzmdxox.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3gzqusakz.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3inrahvvk.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3lfopiyyq.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3spwunvzg.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3sqfdqpbr.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ioenxrba.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3tchxojbb.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mkxnakqz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3owbvmbgl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3fvzivwqe.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3mnxparkj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hyyhfaiw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3jtkckuhm.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fmhawmfh.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wzqoyuai.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3atksmksj.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hhawvcrh.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3psbxxrmb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3npiiuuvv.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3iymtprev.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3dwpqoazw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3yehqxlur.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xumfkmgo.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xaybxeeh.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3kiadyxnf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3slfnxpba.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3uxefwtiw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3haczocec.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3rqokiopn.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3zfticwjk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3gzccrojf.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3kpmtmtuj.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3bzayutmm.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3nxanxfyf.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3pxeoqyga.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ufctkuoq.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3cffkabyj.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3xonksgfc.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3zrqzsnfr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3wdkiayrr.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3sqlgtlni.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3oejnasmb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3vgmznrdi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3fakdrihk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3xvsoxyvg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3xbygkjtb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zrrjgqne.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3zltmqqqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sdjucivc.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3bsuhuwkq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zovvqlsm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3efqvggwh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3agqfivqu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qfnvqxuz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mgefgspa.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pfprqayr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3lyjewtgj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pygapqby.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3sfqloqtc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3umtjprpc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3cmjlbwkh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3sgtxdobw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3gvnpuliv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3rkjiszcj.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3iuvforbu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wgzkushv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3wmwobqbh.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3iqzydntc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3bzerodky.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3cokmnwfd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3brjauzkn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3kcrmylzy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3sqalryfm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3jtvkaqth.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ecfnstzp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ccgxftsq.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3otkykxhg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3alvtujhi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3cwsbvjei.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xqkkgxrh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3drdsxiov.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ywdydghs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3dywmpdqw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kacwhgfh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ghcddsix.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3tzaxgaok.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zfkfxief.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3qfpnuzdf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rgvqzump.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ujotowce.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3gamvuwup.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3zmguspow.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3qpaydmlo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3evqhgeza.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nuaamjqc.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3mmjrsbqn.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3sdcmcfrs.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cleoaaxj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3uuwueqly.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3mqpjgykn.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3uqknlfgs.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3esnnwjys.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3jvmcaxwt.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3shrpgbpr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3jfiwtxdc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3rdvwbilx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3vgowjytw.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3dveawzpy.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3eckecvnh.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3mtpamuqr.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3bdafmcyq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3ppgcjpxg.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3qlmlbyoc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nhafhqed.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3dudehxki.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3behwdcww.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wjowmvbj.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fsbzgcpu.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ocezclmr.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3hgkghvis.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vbkfktxr.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3gtfrvykh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3elqpaecr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cwjauzmq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nommgcwe.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3zpptydqv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ftbpjmau.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ymnherkm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vcozxyri.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3tqdziubm.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3fsqzqqwm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3aauevsbv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3mjvyxrlf.html


<!-- 参考信息 -->