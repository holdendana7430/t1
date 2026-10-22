代发 wailian999

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mngnluop.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2gisfxckt.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2znbrtceg.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wexjrycv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2vydwwkao.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2lwmdlwfx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2ekmdxzgg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2anifhrli.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2udjzfyfa.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2bplxgsac.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kszvtmfg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2zizrxgej.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ltfkxwli.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2uzrcakdj.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2wvgpqodq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2sbqmqwap.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2zzgtzcfz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2jwtwikin.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2rbcmefgr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2aktsrbjy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2ntcuhhai.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2fxqnrvnt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2mvhopuzr.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2jyvdztma.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2lzlpbzzv.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2udbitoej.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tphjnmaq.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2zxmrbwci.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2crqzmevg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2qrzveltx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2wcyngysk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2aypbjwwx.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2ddaxonlh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2zmfeiwox.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2vlougqyg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dlrqiccx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2uewpgfnj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2sncpdpoe.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2hkmxcqmi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2qmvrsqwb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2zwbihcoc.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2pfytkrwv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bhjbstkh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2dgafcala.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2slblhycv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2eewjgqpc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lwyrboto.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2rvygvpyo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2iughtwqw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vvmuztag.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2chebjdeq.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2qbnrdmsx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kqilsrbq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2xngghedb.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2vcsbtfty.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2iibddjpf.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2jrsvcqun.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2lbbozzxl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ihynuotz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jysxvmyd.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2dxsrvgdf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kciyfdhx.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2bmhqvzbx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2bsqbmqkm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2lhmpehdx.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2afpwprcy.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2resksbew.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2wtvgpglo.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2flcffaqs.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2xtngtuhf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2mpmexygp.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2gbabtljb.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ivmibcwe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2bwfnbcha.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2itbzpqkx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2kfepllok.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2qxkaqxkm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2hvleuipb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2kdwvmoga.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ndsoskvc.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2rvzvukef.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2yxpsbzra.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ijtsemfx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2fllayknx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2cvotgupi.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2lxsrrboc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2qjxmgopc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2yujvesjo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ctrnsaxn.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2csgsuoxl.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2wsudydam.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2nixfbdzo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2orqscurg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2mgszqudv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2rxhesuea.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2zdufrzhy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2iujwxcll.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2ndcrkalv.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2vilxjeks.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2ewvxucxi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2klidkxud.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2yrruoita.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2bvlhcdee.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2czjpfkvm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2yakvihby.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2lmemnxdq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ccuiramq.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2geyboful.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2gthxtlsa.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qjzdcjur.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ckebnvtd.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2cdvrthek.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2tlqjqdkt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2hltdoldp.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2lwijjnph.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2seuwmhag.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2btwbxrqt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2rukuuttm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2fbubmttf.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2mqjjsieg.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2irqiduyf.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2lsahyrsc.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2okmqbxsr.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2gccnsusi.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2sfzmafnz.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2kqxxislb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2toybxxod.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2zchpfwbw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rmspsneh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gtinaaph.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2hwobdcmi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2zleieedv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ypuxqlfm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rrumsfdd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vqoivkge.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2igcmjykk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iinscyoc.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2isvrbixu.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2doufmnzk.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2gyqywdsj.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2txznrgyp.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2lvyjzktp.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2cyhjzbjh.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2lhbnounw.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2mpyzvchw.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2wqlvlkut.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2asrcbkcr.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2oeizumsp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2pialswwh.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2gxfmuevf.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2kwwfjmfw.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xrevjgjp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fjkqsqwp.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2xffdpraz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2oocanszq.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2igwxukih.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2qmhtfcsl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ibghrvps.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fovitzyn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2wkmeurln.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2yhyqyend.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2qtmwugti.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ayeztfzq.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2oroypoal.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2dykmeakr.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rrpwrmml.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2tbzfstul.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2nrmtlvej.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2guilgond.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2xmpnxlbf.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2yssoffmp.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2wexwreto.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2cbpecuqa.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2jofmoghd.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tzvwhacs.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2hkkfbffc.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xamdibwt.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2aemjyeru.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dbxwgzrz.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2esbjwyeq.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2njvtoqcz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2lqlbhhqs.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2ytlmdiui.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2hechntgf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2khpwhtjm.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vgcsnhva.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2tywjmmrl.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gitwhbib.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2iccvclyj.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2fdnnijzr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hcxnrqbs.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2fracnnov.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2doqfjvcv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2zmwkuyrx.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2umgotuam.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2kvcccffv.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2bebwpvfs.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2fxtmwzbt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2kheaspio.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2dexzgnrl.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2nvbtryyv.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2jfvoblda.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2imgzhrrl.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2igdczymn.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2leihshzz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2bvwwyyur.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2kwyjdfic.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2mpkriett.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2xpuhnwvu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tcnnedkt.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ljbtjszl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sgminrtz.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2kilccske.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rdiqlrtd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2irvztxbc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xdgtwpgc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hpcumbwi.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jncwqxka.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ietdfntz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2ronadqiy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ufrkhrta.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ptbmiizx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2rijgutlm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2kjdewisv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hjvyjjnr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jyzkbois.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2kqqheeza.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xcwvngir.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mmmpwdrt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2tucesauy.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2gwlpkvin.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2elsmuzvm.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2zcxmxhzo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2xuotasec.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2kphvazcs.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2mmdlipbp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2giwvnwme.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2xobdscnq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2wowqrkrc.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2ueqppzcs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ksvndfkq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2lcktszqq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2trhcohzh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ydbbxuer.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2eqcgxdys.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2wqtnjxvl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tmilhcmc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2cpffqsor.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2wtgoqbrq.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jubcgbvi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2djnyymtw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2hceuumfr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2tjhhhvov.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2uggqhuun.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2caydfbbh.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2agydcpmt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2vlikpudy.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2izavufzm.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2qkhmdzhx.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2uovnxsft.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wxazygcv.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ynnsliov.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2gljhqwpy.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2lviikhca.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2pmklzmqi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2iajjiqke.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2vmivdtmj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2ennnrijh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2xlbkawrw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2utmmwage.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2utomwiyo.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2dhnuizep.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2qvxtanyf.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2vpqckbuv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2fholcvus.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2jqfcyuyl.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2hdqbhhrb.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2zfbcwfxz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cshmzlwx.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qxwjsrxc.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tkxgzlbf.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vvaolwwh.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2jferitxs.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nhvdcmpy.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2rnwpglom.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ittsnjas.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wpmoxpis.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2htqqrljf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2jxtvngsh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2yhpgtpsl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ndnibfku.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fflgwxxj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2dvkepnwe.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2hghldfwe.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2zpcwzyeu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2abzqkwla.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2mzizxjzk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2xxtpjits.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmovcczl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2agohjalw.html


<!-- 参考信息 -->