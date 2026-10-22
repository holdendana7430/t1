代发 wailian999

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2dlphlwdb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2breawhzn.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2zmxmshjx.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2xddtzyyn.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zhanoxba.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2unrxbuni.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2qdhrwgjz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2rewwgshx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2nfdocskg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2nfgksjai.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2wlhpnczs.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2gsrvlwmr.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2ccyaofzf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2uljwomgh.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2kwxsashc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2eeezcjco.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2fpokocig.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2zfbpyqyc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2zokhgsfa.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2xpkssgkd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2jspnbvha.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2fcgovjkv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2gapbxnov.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2pabuajxn.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2flmsuyuk.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2ewcguomv.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fwirrwwe.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2hndxvgrb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2qhuahfli.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2fuwivopn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2rgjnymvm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2moutkrqs.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2pnqasaio.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2kqqvtgta.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2iogalrot.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2llydhzzh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2zjmseaed.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2yfihwdwv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2nrkmicco.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2tnxzxagj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2wfwogydz.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2agcosimj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gwhmyyeh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2bfsamrri.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rotkwbig.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2brjuzkwt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2wxnotqvt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ucymnoue.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2cwqahlsc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2welrxdlu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2vwvpnlrw.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2linjfvwt.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2lqenbpke.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ahspvdwq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2qcbuljjy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2twgycwiw.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2zwgsnrxq.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bttskkea.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2jihmqkpy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fmtyzygr.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2fnuqmpck.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tzfgfyuj.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2npscnyxt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2kgwyarwx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2hssprtaw.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2yodkepmn.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bsstgaov.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ytgbziwe.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2qnznmcil.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2uzyvgchw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2zzhttxrz.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2anexjhnf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2wvelhjvr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2sqremgyy.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2fnutqyeq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2omgkkoop.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2tivuiamz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2ontqedmk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2delrwyjs.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2nttxgawz.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2rzpwvqgf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2tisgxyyr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pqbwhfnc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2yaoqdaha.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2kzqqthwb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2zzdboirt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2mtaiedbh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2jjukyavl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2gckaleah.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2pnrvqetx.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2xdphgohf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2asepyhjc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2cbxbiewo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2iyyvxmin.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2qvxqbcsa.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2asxypjpd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2yhteqgrf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2xcbgjseb.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2itdherlb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2ptuqqpuj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2dgzirnux.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2nlewtxvi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2zmdsdfcl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2cieegyml.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2rqezhiie.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2prdhovnv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mbahhkyf.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bziqboih.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2seytnklh.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qxrizqjr.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2oboaijvt.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vyueumts.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ezcquqra.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2nwypcljd.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2lnqxtkkw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ejhvmkcc.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2aswafgik.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2xdwrczgw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2pbogazma.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2pmnlygfo.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2auhpvlag.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2evcherck.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2yhvzejwj.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2weidxgwp.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2jbqmnvzw.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2jlzgytuv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2vicavuyh.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2vsmrsqqd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fnfnmtsf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ekkspnmc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2kyjskfpq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2orfkqspv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2gydlbcpe.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2apuhbcct.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nthbdfto.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2herbtama.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bchwhzxt.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2wrfzfcyz.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2gtvhdycy.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ugwhfgdg.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2znmvxikl.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jufozign.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2exueuqeg.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2fxyblypp.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2zgmbwghp.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2sfwxinco.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2pythqbru.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bvywkety.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2kcnfequb.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2mgcfqort.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ggihbtip.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vezvuxxn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hhxtttoy.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2sffgfdao.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2olrcdynp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2pwclwlso.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vkoqxunr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ksaoyizm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2mqogtcxk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gwqiplwn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2czntoueu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2uwzmpqng.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ysjmqvsr.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2mvzaurbb.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ivtyvmvu.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wzbprhyd.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ucuvqsgg.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2iuvatuyg.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2sstnnfnn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2drxjeobd.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bjjvlhzn.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2exdebdkb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2zkocwbjr.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2fofjgulq.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yjktevzg.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2cbwwkmvk.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dzypycyw.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2quwhmwhl.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2sagcukdo.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2klzrwquy.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2rbrtpqfq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2lgybiymh.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2foksbaht.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ijbwrmut.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2kczthvga.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rlmusfbp.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2imhcrrvg.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qqlseoif.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2rzbkrwue.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ldtlnxvk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mjtecbaf.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2scgxdenn.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2hmlmxalo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2qsqemqwj.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ureibsgm.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2bslhuwdh.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2zcrrxhlp.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2woacxanp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2qzbqpggx.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2herstgfn.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ysardiyv.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2cgwayloy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ttmbiprv.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2qvsfvxni.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2zipdidbx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2bsjlgbtu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2xuxoolvm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2cjdjrwvc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2hxrgpnwo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hshapwds.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2vzoynhwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sogwwhqb.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ftkzwmur.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ktpndjxd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rgssasto.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2javhfadf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jjxtgrku.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fwypbysq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fedbzcce.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2vqzxykhz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2thxzauuh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2gvjuyatl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2wsjkaaus.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2xpqlsryb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fcegwnpp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2nifpubwf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2seqtijdu.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2cdofmhix.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2zpvgoglm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zutgrzzy.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2alifeuef.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2tcoscalk.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2jwxgeiwa.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ityekuii.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qncddfpm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xdeagzxx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2dxcknoyo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2pysboted.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2bxelzlhc.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2tbmuuscr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fqbiulrk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2uolioofj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2swnegahk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2jwthjsqd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2yalsibfm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2aflxmufv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2hiahhwxj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qtdiqpxg.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2jgtxttwd.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nykhtdrd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ubvndhle.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2eenwwkxl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2kyruvyco.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2lngbkaye.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2nrbyumro.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pmxhxoxe.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2njtduerh.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2geezhtme.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ubqxuauu.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kjlxhmzx.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pduaawgi.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ovpynsub.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2ghxubeqh.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2bylkhoek.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bwclbbth.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2kexlxpds.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2rwmpkonl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2hjyydrop.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2vouxruhq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2tnhwqxmx.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2yadfffuk.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2jbdvoqgg.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2phtpsxmr.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2alrnwygh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2nntazozu.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2zddcdlvw.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2txpbzxro.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2drfabwnw.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ocgkiheb.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ovzabvdo.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ftmgajtu.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qzvmikav.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ybcxbtyn.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kkpjrnbq.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2gundxplh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2pylsihvj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2evghwzmo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hfbyhfpr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2qehbawlu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2arsoclmw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2uctllxxv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2azbnpsgv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2vcrbrbxq.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2ctsdusix.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ygfymnej.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzfevzku.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ewsazskz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2hpmkcgqd.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2nbljulkl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2iybvfleb.html


<!-- 参考信息 -->