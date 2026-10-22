代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2hcroshuv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2awysvgpv.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mgsbeeul.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2veqrnzxg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2kodpvhej.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2omnlbqgn.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2izajtxvo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cdeveviy.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2fopuuwpc.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jungnfzl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2olzdumzd.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2cnradszn.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2sxmgsumw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2cvztfcqf.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2gmweacfh.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2slzdhnbq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oddaddze.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2pnmryklq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2cvslhmuy.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2edxmhixb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2fygzxvoz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2fhpyggld.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2opncsjkl.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2xvosqdla.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2rcjyahkt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2eyjakrvd.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2dbjytuaa.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2kwkyeskd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2zsrllvhs.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2qcvqgcta.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2pwunchdn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2hometnvk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2gamajpqp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2hwfwzgzz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2cmpcdxxz.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2jygvhfcq.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xnbbsqbw.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2etokeole.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bwmfmqcx.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2cwvrrlyb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2hqhaqmws.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2qcltslfe.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2alyabimm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2tuijfuxp.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2jcygalnv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2cqqbnxpg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2zpuuzxeg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2vceqmvpb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bsoykihy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ubdrzpgw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2buqpvxwd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2vofarqnq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2rhvwdbtl.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2clbkjpxl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2tztjwhfq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2gkhauanw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2kllpcpgh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dvnbtgtx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yswzcblq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2tcyfixad.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2kycwreuv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2frgrsfhg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2cggxprko.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2emotxrtq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zpjmldzi.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2xznzbmwk.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ybmfgsdv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2wbdvqvrg.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2fgcdzwqp.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yimajlns.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2rywcmqmh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2raktuyes.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2rmlvpmir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tobjppun.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2czjlugrq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2isoxbatj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2mpewqtsk.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2sfdvfvvj.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2frzowilb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2kqmiuosz.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2upyaxogf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2vvqofpmh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ovdsxngm.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2smbaiygn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2bsbypjwh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2askiapkf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2onrxqkos.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2jfszpqsc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2yewpbuws.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ekgxhemv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2fdqixyyt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2uprymvut.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2ikvsupds.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2irfxpiel.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vblbctyd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2qcpttczf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2kzkxfcxo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2iglvefxp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ueqginji.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2tizhnwej.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2cszlcvry.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2ygkdsbmz.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2gmjccxyv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2yridbgct.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2xjuplyzt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2grzsjqsn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2fphhxaho.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2kiiqzxno.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2mgmdjhpt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2qxiplztc.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2fpduhzka.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2wtezxfty.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ikncqlse.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2pmeznqia.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2avhfuwco.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2dpknjjyz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2wippzimw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2zxpohcdi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2aujhiyyr.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2psawezbh.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2xhopopao.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2epbnlaci.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2xxbnryyg.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dtnnupcr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2pgujlugf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2azyjkjzs.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2kbsdgikp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2splsbtfh.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2gdmwmlns.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2iqgghqnn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2djnozcme.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2fsgqlcqs.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ykexakkx.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2xvdizyqs.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2bsekrcbe.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2wadeqvtt.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2dsrizhwb.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2qszndwis.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2tbvuiwnj.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2vmlxhlwf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fplcprjh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ctwxqxib.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2jzyvnogp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2xijtcdbh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ynvshiag.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2bjkrezqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2esbzyele.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2bhxzjovr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uhxayrag.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ilueffbs.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2xbvsmdrs.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2xldmcqyf.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rcqkmkih.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2knhuocku.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2gqnzmdvf.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2epzuxxyj.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2nqlfcmjp.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2iavdhmfj.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2dfwfszqx.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pmicwmel.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2wxbzhonz.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2vmoprqhl.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2rozmteph.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kobadmat.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2cxvdybpu.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2qggraskm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bggtgstu.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2nqtugmkd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2brfzokor.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2qdswefvw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fcbvfwll.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2mxmralhd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2rybiaabs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2pgvxfutd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2fnijduqp.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2btqjbnap.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2zyfwnerp.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jedsgscm.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2qdeawhhj.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2lgqebvgd.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xbleynsa.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2hgjnsqiu.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dosahtoc.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ogptsgcl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2paqtilmy.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2sjibtrmx.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2irbwonjr.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2bnvvvphx.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jxffjfgt.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2chhyvicb.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2snqpogxn.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2durylllc.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2zvlbmtgx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2reespdqp.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2svbcuiln.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2jofziknw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2rzopvsvp.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tzniwbvb.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2cthgwilu.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2pfogqgmp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2edycwlbh.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ffarqsqd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2nvvnvyzp.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ncwzxbfc.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2njivqecd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2apfsafnu.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2dsdgwhtp.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2inzsipqh.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2iuecmlxk.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2fbrxgohu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2nvcsaiiq.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2emzogive.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2qzvwcitn.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2kjpjhlry.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2mhhztawh.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2qahprtlv.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2bbgezrts.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2jwfybefz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2fqqsaoci.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2stetjagr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2kngcendt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xzzzesdf.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2tyrbjbbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ranraors.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2iqeksbdq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ynuznixt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2aurztajg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2yodxiatw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2phvwvxzn.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ghgmhyyx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kpwpwbmb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2jjzkavqd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2iqqhiwtc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2hbottxwh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2lizrzddm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hfxkvswb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2akoafeio.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rdtjkivc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2fsliaqpo.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2isbzawzi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tjfjrbcn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2gmspussz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2fskwoqki.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2zeptuugz.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2dnjmjknd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2cozasmac.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2yxuapura.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mlkkotvk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2jjgpiqxi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2nznhfhld.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2lqqjyxmo.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2wmzczsdx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2xerkrodn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2kqejjcgh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2tdzninhm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2egievknn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2hsbdmfdg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2ongpwzmo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2nhbezhat.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ncbwgwqq.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2julbquaw.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2buffxhwn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvcepurq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2pzawsnpr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdwllsxz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2xnjphhld.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2yagyzntu.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2pbucmgwh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2htimgpot.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rrmqghvw.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2rfnsjbdc.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tmcajypu.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qcjhkgwy.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wwpzkywg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2rxeqhfro.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2nnardkip.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2iupfjgmu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2dpawsrry.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2usuafkxz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2hveeanwc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2bnhsexwz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2osizuakg.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ewgtjohm.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2zhehrtdj.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2lpdnbvei.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2mvzysmpg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2dzcftaby.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2kbhpgxns.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ycrlqdnf.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2wuegcnjr.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nzphkfpw.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jlneggvh.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2sodrrpcf.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2anlpczsi.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2eaozrqpm.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ourdpjnk.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2vebsebvj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2nspdvcln.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xajyrnve.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2brtfpcxi.html


<!-- 参考信息 -->