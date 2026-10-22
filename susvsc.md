代发 wailian999

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2sgqedhrv.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kzjasoxa.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2pjedgiww.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2exkjmtdt.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ksmlfgaq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ywzvzhnm.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2lilrxari.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gmeqpjqz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uunspndf.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2yjcsvbeq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ogvcbsyd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2wxnppehk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bvjafsgz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bougmdsi.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2kxppbokl.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2uiblsknj.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2qhbctwwo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2qwegzamk.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2suypidge.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2hwgxccgo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2ezumkbll.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2nqluwdij.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2kzutdiiw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2pzyyuquj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2dqhnnjyf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2puvsvwgk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2adxarohy.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2zjtjsgjt.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2axhfyuzf.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2skfclwcz.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2widzlwsq.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ckrbvexi.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2vnpnjnpl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2tzaptvhi.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2kaprmcuv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2iswouqld.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2whqshlpz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2gzmknsfa.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2eezsmcbp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2dmytgumm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2egemppkj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2vgmksrrz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2uymnqjmd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2aoecmmto.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2qknwxnbu.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2mlopqqji.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qjjefilw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2nvitbodq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ljfjdvip.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2wygkhnun.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qrmeqdau.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2zqqjofew.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2gnpwboft.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2wvudnilw.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2obqdxndq.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cbglrzxq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zindkwug.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2yjcyuvri.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2admlfumf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2jlmwcyzj.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2yhxtbobi.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2jwmxbdgm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ugovtnun.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dsuwbali.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2juuylmkm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ozzdcege.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2zxgiqxtu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2aruhnhzr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2abmmabhh.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ehirzzmv.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2fidrpngl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ympnrdxz.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2fmiumduu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2llqimpqo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2pkycdadf.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2inrlnzit.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2heotgeok.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2ukgmuehs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2mcwuslui.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2oivccgqg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2jaklqypg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2trdlcvny.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2afnkmjcr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2qqsczgnr.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2amfiyrvj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2teisxloa.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ezzjfkci.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2qmmwwvxs.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2iddgcjgf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ibaulhfp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2bqitpsbi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2yenecthu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2wppvwoxg.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2mcujxlmd.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2dogiotcv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ioukgcbi.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2esiztpom.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2unlvstss.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2igjfrtet.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2wnijuiwm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2bxljmyhz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2csahlslf.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2avlmlfht.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2wlvlgiyp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2vqiscwyb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2duodxesq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2useqaicw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2rvmzrwqf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2afclqpiv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2xwfcppoy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xygrxxtp.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yuhkmjpt.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2gpmmczvr.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ihdddhmz.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2tnjjwazo.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mnmukrby.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2znoyydpn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ltjpqimn.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ntbuhhmx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2cxfaeyjm.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qznvkejb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2jcejgeve.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2hxdtzzoj.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2asqtpzan.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2drybexpd.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ogbcelrn.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2rrxpvpgd.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2cyhowxtv.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2josaulsd.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2hdqlzdal.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2gbmhefvi.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2invmztfr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vgjjtycw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zjlxusaf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2lkgbzzex.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2fxrlnrvw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2yhvmsgax.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vcyazrcd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2doipsqqg.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2xireqnbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nttviuiw.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2lauhqbpl.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jviyxnny.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2rdsbttqz.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2uydplirb.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hwbpfgtj.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ymfajtfl.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2zejckmbo.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2qhqagkuq.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2njusqczx.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bzlnjzhj.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bbyugjut.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2tnzyqkwl.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2qwwkhjch.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2upsjphst.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jxebzhqm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xwffsnjs.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2hfzmkfsl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wzpbfvlw.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2jmxpjobn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rzgvgneb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ldfimfgw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mtdgjkyj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2rlzklnxp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2bhjhquel.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2fipptlqz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2rzjmczdb.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2mvocaxoc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ysvyekts.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cgyirupi.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2mfxosluu.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2cvkembww.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nqenjgdi.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2fsngrvym.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2knyjnzka.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2sslrqzky.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2grslccyu.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2hwayxozz.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vojaildt.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2bcnukgfw.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uthqvcvm.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mdxbogau.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vkcsyobp.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2clzvqbsd.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2emjkywjf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2hrgxaoqb.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2gxrafgmx.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2zsqmjjbx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ezthqkdt.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2adrwcoub.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2pbptymez.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vifvgjtd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2rlbkntdq.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2pttaltaa.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ufoenkvo.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2axwebmpb.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2fzohygvx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2fvfbngdn.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2wkyruzop.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2zhijqklq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2wmyouaus.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2quidzkrr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2nygkyfbs.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2wcuyvsue.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2lhlgejcj.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2zbhvpwaw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2tuuqnzgf.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2qtauacal.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2udffuxpa.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2boebuuqj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ebxhftkg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2uyqidnjm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2zcvjjzbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hirdegzj.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2wqyszlmk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qxrvxvjx.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2rzabsind.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tvdrmytw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qqeekmbm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wglxzryc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jtyfsfup.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2shhxiqll.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ceuhodkd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2pjpwrskh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mgziuyaa.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2xxbynjhh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2zfjsgmhn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bmfwjcrf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vhrshksl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2iegqkwkb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2rojrzpon.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2exyagxsl.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xardgnyl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ttutgioi.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2cpfqwmpb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2uaqyztal.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2errquzpc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2jhrfgkui.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2syhfnmpx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2bciziuiv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2dunnllgr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2ygeilcle.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2sqysaidw.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2nmdrdrqg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vzpirooh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2uhsnfvcs.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2kqrnwtfa.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2whxpwsyr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2dymnhdqr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2azorbuby.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2qyyeqtav.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2awpqwvit.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2bmtmrciv.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2epgaisct.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cyfzblnm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2aoskiidi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2zrpgaadx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2tirpbavr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2vygmqmvk.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2qssfknld.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ekjzmbpb.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fvvqbqvo.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2gauujyqi.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2vraybygm.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dydufthv.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nrkrfcvp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2uubokwsl.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2gbalfnrj.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2oaocnxho.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2owfrwktu.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2rvczcrnb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2fudhpcda.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2jpaxstio.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ztbeslqt.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2cusahmub.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2cnzmkgoy.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ansvtmtk.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2qhtqadps.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2cdhepgmi.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2uszitbjf.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2dwhsxkhq.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2dmicknzu.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2atrlqtzx.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vonljkai.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ozaajgyz.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2okqwwumn.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2acugtkos.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ljlararb.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ktjzucsx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2zcqipzmp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lvemzdwf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2arqtsoes.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2pnramyvk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2imxmdttt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2uankdwjr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2omvogrsn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2rvbrpxux.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2cevajemx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2spluoioa.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2rznipdzd.html


<!-- 参考信息 -->