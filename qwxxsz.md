代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3ikrqeerr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3rkrwkqjh.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hqwtzlcg.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3jbyktpfy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3kzoejxer.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gdmvnxeh.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3xvyutwug.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3laxzzasa.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3belkzehk.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3suclikyz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3seimsykf.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ctintrza.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3kfbwcpgm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3uikagkph.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3vnrjtvgf.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xfktgybh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3neswlrvv.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3lamdkvpe.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3gyfvrese.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3thzrwllz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eypsvlyj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pxkyqkpn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3crqmlqli.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3smywadiw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3remkmbfg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3dwuaprxh.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3kdqhoaii.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3dfmxcenk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3bxfocvhx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3qdxypblc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3eewkodus.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qkgeptpr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3jywnexrl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3revgrric.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3sgeoaupy.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3csvzfiao.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3betemeio.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3egppzjqy.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nxjbvqdc.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ecrblftw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3tfdkolpt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3qmzszvai.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3ugcfnnhi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3ndhcjcom.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3ainwtgfd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3fpmkglur.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3qvystgim.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3qipqyevp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ibvwwldx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3uqpeofcv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3jvrrlcyo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3gnvzlfed.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3gvvpreym.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3tigcajrq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ucnkpqoo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3ujrckjok.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zczgecuw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3eyrspnyg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jjdlnwws.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3akfjzkih.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3vuvguqhf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3llgjmokp.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3zgzsoivy.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3qhjmscaj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rgfrzbcb.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3vezwtiub.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3gzorlqwo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3bkhtbsdt.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3ffcjlkuu.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yoswfica.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3nhlmxcum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mzsxwtxe.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3jlbqaknh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yuovxmou.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3twwhafbk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3pygkifkc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3itvciobd.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3hkvwszbo.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3wjxsymqx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3pkunsant.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3iwyyaxvu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3dcxwpxet.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gavmtuiv.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mrffjlcd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3wqmsdthi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3lzihxrhy.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ttwsdtap.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ybwoiqul.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3fvzaqspu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3vvdaacdc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3khozrtsw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3bsmjgtvs.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3gyhcsxqe.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3gwfcavyu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3yjupvgce.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3mefemlfv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3eprjwznc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3cdcqbyfc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3yhegnynr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3vnphkqyn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3pjowmrba.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3zjefaxkk.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3twrylpjx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3dhykwdde.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3gchalmzz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3hvvvxjoh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3fsalcqjo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3mfliaiwk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3iqptpwnc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3bbdulvju.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3sawpdcnf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3qixmyexm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3ghkqaojl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3zshmydch.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3tacyqfpp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3ovgdlfjq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3yerwbqlg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3qyyrnwmd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ebugjgyo.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3asjtfzhe.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3uvdxndop.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3jtqscycm.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3xxmwbzun.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3prompvkz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ypfavvdu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3nngyjust.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3pddzpdtq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3jpfphnsz.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3drxvjeki.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3zffaijvc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3xtehjsru.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ysvlmtsr.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3yzybneqq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3vstoazcc.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3amshsasy.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3luaduhjp.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3xqbnecgx.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3wcinpmqf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3lpsjulpr.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3gpxtzwqw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3yjhstshb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ffleqbfo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ymkjmczk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3bvtivafp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3kegukybd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3jtrojpfk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hyyngokg.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3qntzlfdn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vnqedmhk.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3xrfefmrj.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3mizunupm.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3pplbzzuw.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3egnrxpku.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3bppfephc.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3piaywbjg.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mpkmlzlq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3qoprjjyo.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3msroijga.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3byowohuz.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3aujxwydf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ypxwrkzb.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3jnstlqrn.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3oasseikm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3sqvmfbmg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3avaedjbj.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3kbakglkt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3sbuqoaqy.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3ypqhkira.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3abfkgifp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3pyrkhbbd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qbslifnw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3uruvocbm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3kzvlefmm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3zhnuyxxz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3jfumbtrl.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3golatdjp.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ubazhrgh.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3zbovldqq.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3mahkugdq.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jlrvngad.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cfgknxcq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3cevwcmez.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3oqczarlw.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3dleuacue.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3irpugjpm.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3srwkujwi.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uyqiwscz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3pxirhuln.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cvqncmsk.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lwnyqzsq.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hueyxurb.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lzldcazd.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3rmiymdlr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3yyunhqoy.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3sidupcif.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3jxmlatmb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3hfpaeluv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3gkvspznk.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fwwvvtmy.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fwziocod.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3lzqezprd.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3fqpthmuk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3dzrntvub.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3hlorghun.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3libpmvxt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3iqkksmnq.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ospaqozr.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ziiehczs.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3rqcvperu.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3jntvarss.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3nxfehbef.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3fxyhwbpg.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ussqgfar.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3uiesjbxf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ueyhyxpy.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3hptmqlzo.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3papzfgdn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3hbbccjsd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3yfuwklxs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3rscdsrma.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3coafyljv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bynuyrpx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3jofbwxfr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pwapotal.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ndkywocx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rlmxmfpc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qbkgejjz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qvxcvaox.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3sygptsmn.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3htqdhgno.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3veexmddn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3gbnbrooj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ucliqlxz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3sprrtkij.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3stzjwzsh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3lrrujodv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3iluayeos.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3pygrtqnb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3velawwyy.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wqaodijc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3waslcszh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3oocubpmt.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3xdvthvso.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3lolrhxgt.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3iawjqluk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3iqupowhn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ipsuaeyb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fkpzosrk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3qakgxbws.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3xdxaquqn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3gigelthi.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3etckajsr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3wejnwnwc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ckqwmbjc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3btudtwif.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3pppkwexx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3juvbgfil.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3mzgnnesr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nmypcgfc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3smmhqkiw.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3fnhysrrx.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3riirmzgu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnxekufs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3pppwowpo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3dlzwdmyn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3tgcothoa.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3myijphxc.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lumkfkpo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3hrpiznjd.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iyeyvhuy.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3zkyxmxwr.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3egkgxjjz.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tfnvsncb.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nfkpywdv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3djqcmciv.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3cmquidmz.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tvltoije.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3gcqdkbwb.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3zegtqjiv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3hxwrkazg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3xbblakrw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3znecyyzd.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3tlytkuob.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3rlcsqrwl.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3nigwocjp.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3fgzacfqa.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3smpvqunq.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3hwzugjar.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3limqkgun.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3pyfbblfj.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vegrmnls.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cenxlbxe.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qbhuyawf.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gbgaclmj.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3mbydophl.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3sjjmcowg.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3huqnsdkh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bshtylsq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rpoufrey.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3aqxwlrei.html


<!-- 参考信息 -->