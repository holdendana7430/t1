代发 wailian999

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2pxatlvsk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2cggrbuim.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2qyljlcyg.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2mopvkbak.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2cqcgohfh.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2qvndkhbk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2tnpajxpv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2pfqwitzh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2yhkplhry.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2dansgfyi.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2omgpujqy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2uldjurnq.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2cuhoswmb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2bjldakjv.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2dydjgpgj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2dbolqoka.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2habxpqch.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2bvjnutqf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2kaewninp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2srbjsmew.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2suiwwxje.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2fqdfuhov.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2gavjryfr.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2pvkhheoi.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2dprnxyor.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2urazgpdc.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2axmcdymz.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2rvfmfnms.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2sueestpo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2rcemefuo.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2lrofxecz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2nroztmmx.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2ldqfhkrc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2qnnmlonp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2ipgwcclu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2rymtbtiu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mmewuzid.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2mkvvhais.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2wmrmtxnp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ghukquvq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2xehysumg.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2anmpnsex.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2eyauwwmy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2hgkqgbvu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2agkhtsow.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ubllvroc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lntjyvhj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2xxwvggza.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2vqorlwnb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2wqrhysib.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2befkfjoa.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bjlimcsl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2mmgjgrxk.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ftlrbewq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2yvdeizjd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2rqnykhjm.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2ycreejmw.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wocdklpk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2vytuighj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lveuebzd.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2wtswtchr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aayrpcif.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2hhewlnbu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2qgfjxapw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2hcqiicko.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2shzkvnal.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2rhbnwwep.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2qwvhfluj.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2nzvuymtj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2jvhsnngz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bwdvvono.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2zupgwdew.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2xbavfmmg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2glkohbex.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2iamyionl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2nniynrzb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2dykbsjym.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2rnboxsbe.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2qqcpuplk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2xuxlurbd.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2guweqjkt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2apwkljyo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2mzhurbco.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2vwpdidog.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2gnmsigbz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2ekhtcaog.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2mqclejsm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2pdwtsxtl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ocysaanb.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2gicpmmqq.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2wgpugwne.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2vcngxaxi.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2tlsmsjxl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2qdsaiybu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2jnzvknbj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2wslsnrhm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2gnfovdvs.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2wnzkfjtx.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2hpgqwhqp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2plrzknbq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2ywdppnub.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2usupzens.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2eblheyvi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2izkpbgdw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ssxccirc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ovfrxqdz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oichsilu.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rsdpfhto.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2diajdevu.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2psmwifua.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mehufizz.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ljcaypab.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2edrwklor.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2hcdnvqeo.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2tazvnjyu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2pyczrshr.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rdviphts.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2coahexlx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2jfybauia.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2wefzsifw.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2xwnhhpxt.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2stgajxdi.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2yzhtcxhl.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2qfuzozbv.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2lggtejpn.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2jcotkjye.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2vpdzbtrb.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2ucwrpksb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rfsozydo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2noiwexii.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2iiydygbq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2knhxeqvd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2myfwazxt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2aaioklch.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mgyxxokr.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2gqzwzusa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pzsgcibx.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2pxhumhdz.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2oppxmcno.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2bhmhgzjv.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2exblmcvp.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2yrmrjfdp.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2bbuuklyw.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2knzcixeb.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2rwtiihrq.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2erddeany.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2qsvbzkpv.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zhiijufa.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2uqjhzlky.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ibhvtmmv.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2odabcijf.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mbiixbtx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2biggmrpn.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ykeeyooa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2trqsuroz.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2cwfhlncy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2ybwussov.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2pzgtamgf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2bjklwgww.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ozjbxjpj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2zgtvakub.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2xrtqssgd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2kybwyguh.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2cciwuaph.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2imliiamm.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2aagwchdo.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2laommmwa.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2wkhqnswh.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2lrwsxsbf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2fnpeosqa.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rkoarzam.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2wmfpwcpl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2tucotwwm.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2tjbxkcas.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gfrqpmcu.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2xwxagata.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qsmjiqst.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2idxvofvg.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jgqfbekc.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ribdujfw.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2voydxmpg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2cfnzkloh.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2dagybyam.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2lyrpwjcr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2goovqngg.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2iailoyjp.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2magztnvu.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2guthfgql.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2wvnpjsfx.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2licenfjn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2yhyenbsd.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ppfhslll.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2riqlxvnx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2tuquoeji.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2kegklnrl.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2pdtqcvqf.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2zufdgjms.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ywbsrenl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2ahjilsri.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2lhbibdhx.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2fjdaesgb.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2oidpwxgl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ghykoxfi.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ptzdbrte.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2bwqmtchu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ruhjksqc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2owbhgmun.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2lzjpoipx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2ziuqzqqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qzboncec.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2kfxcuhda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tzbnqgoe.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2hqslgrpr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ltrbbvva.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2eswswvjn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2znoynddc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2tplgtegh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fvfnmawc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lnsmyahd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2hpkncibo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ylrscpmu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2usrtbivq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2jrzwjhhs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2iaysylpz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2eqjohrjc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hchacyix.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2rgwscxuz.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2qjoapneb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ralxnryu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2owxbfjpi.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2gqjefanf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2edmgpkrp.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2zpwgjnku.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ysmbbvvv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2nnfjvlaf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zixiytld.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2ymayabqv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2ejpguhel.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2laygfdll.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ezzngmqj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2vyukqdzb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2pbawtelf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2faodgomg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qcqgakpz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2rkvjazop.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2oxyfoaki.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eivtguxt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2aodqgnog.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2tchjmtym.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2fohelywr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ttjbehyx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2jpfqygaq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2eytqgrcj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2oqrapixb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2zuegtsru.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uexmjkrs.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2pxkecuiz.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2byhprfju.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2xjqtkvkr.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ecrhscjo.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ovtksadr.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dduzggcp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2xslvzcrq.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2votbvotm.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2zxktaeqz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2fjlkdvet.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2ghdxlncp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2bklzweou.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2pmbxyllp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2byxzulif.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2fzdjrfbr.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ccxdeqln.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2qnbzzrdc.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2yporgzgx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ugmhsxfh.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2vuayjsfc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tpsyyzpg.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2axwqifsp.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ymttrjvz.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jztihtzt.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xwldbmqn.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rvwiegvn.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ytizcfyr.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ygslmwpc.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ooybiimm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2xlawdyma.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xyfrgybh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xwnzozsb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2zhnexvgc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2oglzaets.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2ihapepdq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jlsklyib.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2njwrkand.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2pbjodrlu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2xabyffwk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2zwtwvqvr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xobehuas.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2wrbjmuak.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2kuvfkjba.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2xedqhwri.html


<!-- 参考信息 -->