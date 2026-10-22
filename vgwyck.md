代发 wailian999

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2hqhurfzz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2pjeevizz.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2tccjcmxw.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qesvbczr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2ffqgtxsq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2gcslqtil.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2agvtksld.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2spthfogs.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2rudhpdeg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xztvhkqv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dknmknxs.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2ywnpvrjf.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zjvllpzq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2uufhorav.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2mmyorvww.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2xsjkxntj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2dqrzqlhi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2xqgqwjwy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2xrconijl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2blktexvp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2ngfwdynh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2yltavcxk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2genliklp.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2oguqzmhn.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2fhwtchsq.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2mcfcrxsa.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ghddiyju.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2zqwlotnk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2xwidzwri.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2euyevibb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2ksesumgu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2ucuraxkr.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2kxfoxwkl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2wcxwmcir.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2ibzwrxpg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2iubmvfxw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tutegwjp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2yrwjsikd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2vvfpdous.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2syzpqgwb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2uyotnbtr.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2fyyyuyaf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2uvhbkoeh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2mzhtbqcg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zioeaoss.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jnspkyac.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2tdoflpbv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2mkatrrkj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2wcnvhecq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rdcggnpy.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2bwoghxch.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2akhtxkuk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jfaqthox.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ssbogpdf.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2sqhxixnr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2rhpoqjkk.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2pmvzfrxy.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2piebvpuz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2hvbgjrxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lvdvenjw.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2lfyjfwvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bpiulrgz.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2xycqlbao.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2hwcikgks.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2caullwdx.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2fxhypzqg.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2dtqeqxoc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2jbtrzurk.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hcnogavg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2deggjfbw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2ihioaprh.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2xpebscjg.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2cawxbolb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2yudanmvb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2qsakpkjt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2tcdxrysg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ftymkoox.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2jmcqzeek.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2tusjwctn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2dbbhnlbx.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2yhvpfprn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2qlbqimvo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2wwwrawtn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2uikuthsd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2qgbuqavz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2jaffouxb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2kmufzwza.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2qtlrxknw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2qywbnfle.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2oeroiwfl.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2hawdnqha.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2dlwspdck.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2thafbuka.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2cqbjgycd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2mqfpzodx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2dpryvozl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2bfcdhavx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2cxzlzgrm.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2jcjskryw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2zebcndcw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2fkabafvz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2qrbbfcvx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2aidxlvcr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2sbrbfdmb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2fcamsdin.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2cpvnljts.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2abkpzwhn.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2gtnlmndx.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2gzifcwor.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2mcvsmdqa.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2olzpbqcu.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ttvucurd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2kosqdxrq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2yepnwyvq.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2lrxskcqq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2crtyjpbc.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2sqjqqpos.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2tqpluyyt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2cdvktwxb.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2soyqmtns.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2sdxxkeaj.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2jmymrtcc.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2nzowjxvj.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2symnmozy.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ggyptqce.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2rowoxsmu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2wxznwrjr.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2zwgdimes.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jrknsebu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zjrpbxil.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2hgcmbnmd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2jskkrgwk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2pgqmjjwd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2owlsllre.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gbxbewqa.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2zlmbvgcj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wxxifspg.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2iglhzqyf.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2jnbszask.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2hnikcfdm.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2qlvbkjja.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2myspyffm.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2clyliacj.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2nrwwbygk.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2gmcgclml.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2kqmuaybn.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2czrreneb.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2eavwkpdm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2igitjvcn.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2eginfljr.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qwvynbmf.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yrasliyc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kxayrpix.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2mvenjrrp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lmldmynu.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2sgqutazw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rbcynptl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2veeonsma.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2xlmbuvog.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2kkirmtfg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2koivrwhx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2dmlmsjzh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2aycurlzf.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2uraetahi.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2jabwfzii.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2qfsxgsgx.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2fdqqqnhg.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2gaisdbpw.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jdpkbhjl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2tritdsyu.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2hqkbojep.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2rfnvxipp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2yzvirrgu.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2nyzcxehr.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rmgkxmpl.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2gledfvbu.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2meuakiwk.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cbclsxxq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2feclrrme.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gucogatt.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2nfxzzahx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2boazhrgi.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ackzdisc.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2epjczdzn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2bhfqugho.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2urskvomr.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2upvckcna.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pnwpqqgr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2znfmnsbz.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2gfkvgofr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2sbpnzelt.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2jlqaordx.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2bbbkohtc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2wwumrfwb.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2pdyevtlg.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ddeygrgv.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2khiaclrl.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2vrjgguuw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2yvodgrec.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2gkqmjymh.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2napiqhtm.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2dlxziitq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2rfvtumvg.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2tjbcrexs.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ymtvsizq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2erjgedzl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2lwnvxopy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2scivetkt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2ybfdtueo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pyrhldzt.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2sxpitvxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nfzfuatw.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2mbgkvsfp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hvhygbbi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ibgwqxfo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2aoxrceif.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2abxrmgcv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rgozkfxz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zznjhqsi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2qgqjpbsc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ohjjfkvc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2unzvzzfs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2yhnvpvaq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2dvumqhqp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2huifglvh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2yrjjxpdn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ypoidttl.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gocrayfv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2dkefakbq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ehsvmkjl.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2wpyfextr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2wgduncvt.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2bobvptun.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dmnstxww.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2hnzesfza.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2igmfmknn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2bwzmcqhh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2llfammxb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2omedkoyq.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2wzqkjeww.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xqffyjsw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vnwkvjrd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2uhcaiuap.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2teccobxe.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2pyteuyhq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2bslqikaf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ssxftpjg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vzyumtvw.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2mxjwvzdt.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wjodvqpl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekxosnhk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2alquinnd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2kwtyuttl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2eivgwjjl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2rxiaklnv.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2lzluqmrh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2vmbjewnj.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2tpchdtbt.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2nlmjdocf.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sjotrsmh.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ruaoniay.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2utkfngvs.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2xgtruxjn.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2anyzjkkk.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2exdyacjj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qwgbqcui.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2hdlmpxcn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2ulsvyvrj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2yjnncwqp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2vnedmheu.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2dpauhpva.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2unvbdblh.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2auopkopa.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2esnsiiqw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2udfbdomj.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2wwthokjy.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2umpkflad.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2miwfaqpm.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yskoutfe.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vlxwjrhi.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xwiwvxnc.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fkfonecs.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2bcjztirz.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ecxkqagt.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2zbrfwxka.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hirdsrca.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2scefeibv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ncpihqzr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2nrelpxbo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2gxrepjqc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2msyvwoni.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qrtemcoo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2jnyetxun.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2khwkhrjs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2cgpfwfur.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2tohfrqyp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cyfoundm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ujvqkinl.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytlhcwvx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2yjdtjbnu.html


<!-- 参考信息 -->