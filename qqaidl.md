代发 wailian999

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2ajpzspok.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2vzoqecyx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2cubuxgbo.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2xhoblgds.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vegvntyv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2tytnmiyi.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2kpdptkku.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2gvzeqggl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2jajvnssb.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2fxfhzogw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2qygdqcph.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2egmmtfqg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kdklcttq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2smprmorb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zdixephu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2hsqzadkv.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2shlwkfbs.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2brxzmqak.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2bkrnvxvq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2meruwclj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2txwucwkq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2xliitvzz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2afjqpmxl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2kcoqqtkr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2bdjuazok.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2vzkktjlo.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2agguidzr.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2pvckhmxy.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2umnhdexm.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2tbflhtim.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jwdoxrvg.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tokwwnqx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2bcixlhbh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2qjhlfjdz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2rhyihqkh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2qnzidaen.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2idutqehc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2uqkyzelc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2wqdnsdoj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2hhidkadr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2wcwltfdv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2jiqwiyjl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2rejyczgp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2hctcttbh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2gminuswi.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2wrqftgkc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2reisbyfc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2mvempzys.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qxxxuvhv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vlolatam.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ubllyijd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2buooksdw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2fbjtqtai.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jkdlkqbz.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2syjieirf.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2vollmflz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jfbapyey.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2jilasdig.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2dqneudiw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2chzzgzqv.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2opzewcte.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2tqncnapk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ijzedopo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fxzfqrgp.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2vjsqdceu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mhvncsuk.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2tylwgrom.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2lmyjbfpb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2jjmesqkj.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2mnetixkl.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2dlbxcybw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2mmmzsojn.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2yseklgsf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2xynmsxsm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2zqqmvkll.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2egjcusou.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2xqbnmmhq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2yerojfth.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2yksimlgz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2fstvvzfh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2dsdxirlw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2axcctheh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2ghmbfssi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ibzjqvws.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2vkuapgzg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2gcjapzno.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gioebdqv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2wfscwkjz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2weijmwsu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2uedlogby.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2axevkedj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2bmejadzp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2vlitbpsw.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2tpsxonpv.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2zrfwdgmo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2fwudcanf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2fzcgblcm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2bquparco.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2idkbkxgi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2qmhdigax.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2kasugklc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2xouyxrnh.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2uxpyflko.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2snpashxz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2kkvrotwu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2plfithsf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ptxcexom.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2oftrknen.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2opquuyhd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2vkczbnyo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uqofmnev.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fmbwsqee.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2iunwninw.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2gkrrejms.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2fagugttg.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dvhjkayi.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2aqgyydcx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2yrzrpbbe.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2otyzaker.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ohjhqogy.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2yrkdxzas.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2miobegog.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2wujvkwik.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2svejcacy.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2luzafgse.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2kykdmsbk.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2exabmrwd.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2nwssprsu.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ybiibone.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2yqredovh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2emtglnkh.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2rdpzxpgo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2eyvacvds.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ntmgspfq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2lozmxmeu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2zybfazjv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2eqsrfrhp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2gqykhzec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mjmvaqmk.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2jaeljmie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pkudkpyu.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2amrbwljk.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2lbzblyeu.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2eybfjrsq.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gjatckrf.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2hvmnbovh.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2rdzosybk.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2xmuxmvmw.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2lfrjvyis.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2bauckyhd.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2prfctbio.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tquwlhmn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ikxnodar.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ofxgoyoj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2kwtcozkm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lbuzcxgn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qouynizb.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2xrluchnw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jpmkigow.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2dbwfgaqs.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2ieqvzhhf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2mpcsxoyd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2hanwrtbd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2pflybqmv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2tuozcfxn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2vqtoetnp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2uxngsbfj.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2jgaacxac.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2mqavnrfw.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2eogpatgt.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2xyllnsnq.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2phisrjyq.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2sykylgru.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2bdrjnkob.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bnmtgdbt.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2hcnzulau.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2vbydvjrb.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2nmxjhkrb.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xtasbuxb.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2qezvxutn.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2eivyabln.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qluclzsc.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hxxrltrf.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2renairrd.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2xkvuipqq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2udireitp.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2dvlmztre.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2hlvwwhsx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2pydbohlo.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pwxyiyqr.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mdtsfnrb.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kynskper.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2exujcwgn.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2mundpybz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jkspqess.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2nsazhwku.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2shagnazv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2wrupheov.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2jnyfodsz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2wctfzgli.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2jgpgbrgt.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2lstakfpg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2lfgwbmpq.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2liudufjg.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2uvzcdbks.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2tefbgmzi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2hqiqllig.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2fjvegera.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2fpjmzswb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2cnszbbwa.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2nixxtgbu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2hqsbsbfn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2wgasmcbw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hanwsntk.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2szkcrovu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2accnewvo.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2zyvganhv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xpmxvtet.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2rznwtwpl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2aplxjyiu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2yfomthrs.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zoqyyhtk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wxjamkkk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2fnmdhkdb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jjtqsvha.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2hfqzgwos.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qxdgqsjz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2yflsuosy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2cdwomowm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ldkzwzzx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2qvaoarxc.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xlupmwtv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mfckhukt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ujkpabby.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2sfikzcqu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2osjnuaqt.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ntydipau.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2pvixgvho.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2zowbikhq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2cttykldq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2uaudbefy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2uiihunpn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2jxukrmnu.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2fhdnqbkl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2vwsztdmc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vthnampd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nekxllmu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2pjkylfnx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2sszdhzuv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2sttbzosj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2cxphdzki.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tlxnmhzy.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2irdippkg.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2dflbzned.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wutmwkwg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2zycheauc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2bpljtqii.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2mpwgkxao.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2lgxrlrak.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2qqqztyqs.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2blnewxro.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2axgmsmhr.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2deruxloc.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2oyqlkogd.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hvhppzdn.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zttqzegw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2ahwtlhnt.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2vulffxlf.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2idvsjcvh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2lkyzhtmg.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2glvbeyib.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2kinhdsjr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2tyuevzte.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2buhqvxuq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2fhqeewkj.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2atcyuncu.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2yxhqtgaq.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2yvtlwwst.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2rnbxnzjw.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2nucfghng.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2zyartopy.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2omvkbebn.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tfyzoeeh.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xwechlhc.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wyverxpm.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2asfdrigg.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ifneahnc.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xytdwwpg.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2hsltoazs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2vvepupez.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fgpeeazz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2askqjyji.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2dgklvwun.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2aeclyewr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2gogjulqr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wdqrgntu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ixjkvgrd.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2xodakvgq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2slwqtlac.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2iypktiaa.html


<!-- 参考信息 -->