代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3mskgyfaa.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3qtrztcwj.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3gbvfrurf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kiazhikl.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3fmscuvnk.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tcwnnoyk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3dyiarsto.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3hcewynai.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3irlixcce.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3khjjsxna.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3jcbznsja.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ugknrbtb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3kcakrzch.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3bdtjkaes.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3mjnzkhzl.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3lqxnmcsx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kjratleg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3vpkrtvjo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bjedackl.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3stpifxje.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3zgygrwkm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3mxwdtxre.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3bwslbovg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3gqkztfub.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3djtdtbrr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3fafhcvzb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3fmsuaiij.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3mqdzrrpq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3emjvjlqt.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3mxggdcrm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3wgrnuyed.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3kqveolez.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hrzcpubl.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3fyaidnka.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3snntfwbq.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3iljaknhy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3bcillteo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3erxglqzc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3tnhtmpoz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3kvdsklcp.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3gbcjqxcf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3rothmeup.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3gqzguvul.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3siimtncv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3kiezjrlg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3blhodedb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3zzskepcs.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3reyfjcpd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3rlgviwhh.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3sonaotnc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3sdxdtqjd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3iwsnfryi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3tgbstpfm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rddexslj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ahnkfauz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3uwtrhvrs.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3gvrgpjxk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vylvjwvm.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3jvqwhnxp.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sntefqxk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zeokovty.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3sgofwhbi.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3cxfbjpbb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3ctssdayw.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3iafhbjmu.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xyoglzsl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3chzysjdd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xfzubyic.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3ydaegrek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3edqrseex.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3vyujozhz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3yfwghycf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3szvpasnt.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3rhqcxgjm.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3tmuqmpbr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3ygdpiiiz.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3bdzohecq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3vjyszxxk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3yseyspur.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3gttvvnyh.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3nbvxgves.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3qozdxvfn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3owuuiyps.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ozatgcdl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3sxpvttpt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3mtrfupco.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3fjxnmuip.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3sxiqoumy.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3wnrjfyyz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3rexelfeh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3zopxmaoa.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3oxvhaony.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3kcslctem.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3mjmmsigs.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3fyiceevj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3rdncapyx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3tftlvvdp.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3arsdzopi.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3ydfgqjwd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ntvbrrnl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3tkrdvebs.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3czhyqxei.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3iqnfxgrs.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3icjakuuy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3vhyfrvam.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3rrqszpdy.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3gqotowlf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3xaslrola.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3qdrovmnb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3xdukorvp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3wtptybvm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3fazrwhpr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3fvnedjml.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3tstkqmoz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ccdaddwt.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ppvujosw.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3rxjxxjnq.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3dzrsrlty.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3fcxzpqws.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3otdawljn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3juehffoz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ocjufpjk.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3jevkskwq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3cjkkufnz.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3nsqmonqm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3qucncwql.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3kxeahpme.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3bpynzslj.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ypexiwan.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3cwmhvbta.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3mwkkhuuv.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3qcitfbwy.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3rzcffaok.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3wjcgrxnm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3edurzvcq.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3owsqdjqu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nrdfhgcv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fqmzyxbo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3frucwqre.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3cayfuhil.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3keyncynh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3cuxwafxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hmrxzsmu.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3hlbmanyl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oiiwouqn.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3oppucokq.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3rlobdyhw.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3qvrcppim.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ntwfucrj.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3kxibupeb.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3nlovkbuu.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3lroqkmmn.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3wyzpimft.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3dugheyxi.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3dowoyata.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3awnjevrl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3pbajnkla.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3prqfnovr.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ylidthmb.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xxpxlqpz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xgiuehsx.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3lmlipdxa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zhfkozdl.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3llzjdsvu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jqfyleul.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ulcecfrw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nrwaaqob.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gocpqfpk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3xwtgenay.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3altpwqug.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3arzhehzs.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3qonctttx.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3exkevpgj.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xhnoyjac.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3hnacnzzg.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jrljpexd.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hrbdcfdp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3luazdnhs.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ikdpyxps.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3csznardy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3rmyjrqyf.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3kpnvxdvf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kcwxgsfn.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3iqifuifu.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hpcgkvzi.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yhclerhu.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ypsvczdv.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ikdvbmie.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3glbkunwg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3tvnfsfdm.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3kxharxrg.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3mozcjvao.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3nyowvhzu.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3eurlikde.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3dljgrdmt.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ikgonanq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3uuskxpvg.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3tzitaotf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3fwlkokpe.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3vcxzcdie.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ztqxdbom.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3vrnqgipd.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ehsnbuew.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3kyakkjkc.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3fiswogop.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3ojroqgkz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3anqzfvij.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3mdhtamzx.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3gkpgaimj.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3rgqleztq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3kkaamutt.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3aztbqnew.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3nbvglses.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3vrmyndrb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3zrgdkxrm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3yiilostz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3lvoezqut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ydqcupan.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3dgydhwou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bvibwmxc.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3aovdsrvt.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qgzoetju.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jdxvxaqw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rhuootig.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dmjdliuq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3aisjlftz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jzrdpdxv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3mgaentho.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ufzkjkwa.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3nanxnbac.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ssyomcnq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3zexwezxv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rchzgjgz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3kdhskqfz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3bnliwhgn.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3mrrmjazg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3dxtvmkyo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3bbyxarph.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3otlkyfsn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ixflezph.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3gcgqkohw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3kkqmumfh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ljxjlkma.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vxotewwi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3wnxapazf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3wzbsqrpd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3bcyriokw.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3fxgurtqx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ylhmrdcp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3hnungwjb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mcsdjvgm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fcvjjvgw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3fhclbqvu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3grwgkhrh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3rscjuckd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3hldlamkt.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3iemhfxqk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3yrfvozsz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ugmfwccw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqpqqojc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvlhkwiu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3kfxrtckn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3npkmocns.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3aiyfedjn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ooeciayr.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3tsekusif.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3infrsmfz.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3sqiogpko.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3laqqlxzt.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jqlsmlgr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3qgvmqckq.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3mkvnmqhi.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ghjkzxyq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3kvbzkyep.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ncplzdgq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3nqgmxata.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ljrhovit.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3mufiihyo.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3vsvzefux.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3rosexbmp.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3beqlokhc.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3mmcvvomz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3bduavfmt.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3zbubugaz.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3laqscshm.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3zzbkpxht.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gsugerjl.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3exssycay.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3azjpfgdj.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jeepqfqx.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3oemjconh.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tamqcbzp.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3xnbwndwn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3iatmscsp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3aippummb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3dhveuxqs.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ydmqwyiw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3wxfzfbkh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3cfmyfpdu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rbjpixbs.html


<!-- 参考信息 -->