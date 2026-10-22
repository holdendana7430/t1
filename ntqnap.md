代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2vyxtaoib.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2angvfgye.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2uqebkehn.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xsrafbdg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2fjyynrym.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2taxqmpxt.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2lblubxwm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oguryrwd.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2agepuxkw.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sqzigrnv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2waazhyal.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2elcsruip.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hdejzgkq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2drljkraa.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2kximqhlg.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lpgwldda.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uxbcvaan.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2xrmmyugx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2xhnmyprj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2cpluhzyd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2upecszfv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jignsuop.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ommvpqqf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2dijncboz.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2nilfblax.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2hqruftgy.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2xpqnsier.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2uuraywmj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2wubxuejo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2xxrbnhvc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2goesaylz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2cepyalcv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2txrhiyol.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2jghuylvq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2qaevdrpt.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2yuargjum.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cpeilyvj.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2pbesalym.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zngvhrpk.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lanldzyr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2vczihoix.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2dwyivstw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2skotlfoh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2ecoolpvi.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2pwtzxbeh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2zfccmusr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2pteobnoj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ealuerfh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jgwnvgni.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2uxgmbmou.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2cmakhqir.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2gtnrkhrm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2qmqanwds.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2lwkawyiy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ndqxlsjx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2kidxqmmo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ilncwsma.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hxxpnbpj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fxkmgqwj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2gkbexqno.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2kzuzezrg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2sybtmnlj.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2qfsczemr.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pnnntgli.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2oedobwxj.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2zipzhhuq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2kbfjenyf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2vopapmfy.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2qghhxtpg.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2avnvalah.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2mvufslnv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tpfzrxig.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2cueclyce.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zeurjkug.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2wfxkdewb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2wuuqukad.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2tzaywdfh.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2noprztvs.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ifahxtas.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2tatmfkrt.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2stobikjm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2cfkieald.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2lzslxvce.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2qndbcrzw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2pcgsmofi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2ruelhhgk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2hvjigqpd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2devlxvxl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2nzliywqj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2dimseauo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2tfkgfqjl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2wzeqsudo.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2ugatnmeb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2smobxagd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bfvykhre.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2vsoowutn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2exlmpzxw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2tixxwkvq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ubbxakdo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2fztywupg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2dqgbraxf.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2lwzxtali.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2dlfoyvbc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2wfjvxbwe.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ncyaaahw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2lnlbwzca.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2czxdlbdh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2bckaabcq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2ujlionxj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2osmxgxbs.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2hkuwydis.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2knjfxrpi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2kumrtwyn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2cyzauuca.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2fumeuyii.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2ahjjvvxf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2ujkkyrzc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2rduusfaa.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vsjjcprk.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2wbiommww.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2veebtggj.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dcfwjstx.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2nupbyynn.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vwhjlsig.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2apshkneh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ioojvnkf.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ddjhqlnn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ejednofx.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2eyfgnhap.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2yghunplt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2iedodwob.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2socaijav.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2sikjuvjn.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2vocbhseq.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ilvchhyd.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2eviiazhf.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2jyneenar.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2wlskkmjw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2iwxbyvmk.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2vdphiadc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jwrscrwl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2telnkvmz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2xcnzutio.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2tjakqlyf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2eittvwrm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2cxndwesb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ycodvhht.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2bwrmtwip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ggcewmpt.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2umrwnjnk.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2upbszliq.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2fggqbhkx.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2sxmjshfo.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2bgbvkivr.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2lmganodn.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2jkcruppx.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2rwgzwxvi.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2gcdvigkz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2mbwldrmp.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kdkdwzft.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2qbfypuzr.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2obddxzud.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2yrowsorf.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2areswonw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ixtmiyrp.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2qcjbwkaq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ebrplfma.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2auuymdzx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lbvbxdfk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2balixyio.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dykyipcv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2gbxhjqas.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2crwbydxv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2yliksiia.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2wymofbkv.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2xjxlabtw.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2wvmzatky.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vnyavgdr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2vowdhoer.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2iydwjmvw.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xidwgpgk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2bfjefxho.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2btvhhsrl.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2vyeysmtn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2gsyjhiqs.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2srgiwwcm.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bvilexui.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2huogqlzw.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2luajtpcc.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dplsjvfa.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pnaeueho.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tpbuuymb.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2vncldexa.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2vqeinbkb.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2bijnhuir.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2eyncbclh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2crztdfzh.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2joueoqrw.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xfhuzumr.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2mirrbvxj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ikyxgvxt.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2iksnmoks.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2oppopnkg.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2sjiaqmtj.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2pznebsfu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2hoomcgjz.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2yglnlkta.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2pqllyntf.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2iipxvlhf.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2eweirqwo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2ihprfiol.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2fexjvhqq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2dwpycoal.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ynizuleh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2qnahpkbx.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2djvirvaa.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2wgkijonb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2twqfgzth.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2rmcdrhox.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2ueeitjtz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2dhfgixfv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vxsikqzz.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2cdmwiasy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pwxiozgk.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2rdyccted.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2krrvppaf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vogtmmcf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wmidkwuu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2aqyfbtsn.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vcwgkguv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dcywdnez.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ligwffzh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jngmpjri.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2xexckquz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2tmuocgjd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jbsvlwgi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2eoorcjya.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2tvkoohib.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2judppoxe.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2syounhkv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2gqqqzltm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2yihytqwb.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2xyvqblws.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2dnpqudqv.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2xqystvff.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2dpszscaf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2vdcwivym.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2slvkcztd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2dchvdaer.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2axgjloim.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2myhrrpsk.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2olmsnqev.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2rvyfnmko.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2dkjmasma.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2tjvxbdqn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jhqhheoz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2oruckenr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2jgenxrti.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2qprwqtrq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2knbsjjcm.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2ocmeunim.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2iccnvjvp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2gsmbskqo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2gyemnakn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ntyzwror.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2gmhteeeb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2sqrxxmjj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2nzyuqovu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2jwufmgcn.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2rkkmdink.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2tvxzurny.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2yxpnepdz.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tpnqjcrx.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kkkgxlti.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2kwnwwwbi.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2qgvopkar.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jvpsgusa.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ioyiajpy.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2udtsjuih.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2tdssvqqv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2mavspmyd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2kqsmqhhk.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2nptswdux.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2pkffudyp.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2nezdpqmy.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2myaordfa.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2npsltikc.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2ithduryk.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2uwovspuf.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2ikvpfhyw.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cbjcmvsb.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2opaedqaq.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2slnaizun.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2sktommzn.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qqqitwwy.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ktwbrype.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2sljzmzfx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2cpbhnfax.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jxaiwpcs.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ddlacfnl.html


<!-- 参考信息 -->