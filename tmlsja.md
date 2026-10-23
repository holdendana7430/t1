代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3fcqhswhq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ycnlfadn.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vkqnpjep.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3ejeexbfe.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3dtflfrro.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3dcwwhgho.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3ndshunio.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gpdnpqnk.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3dnmhkggw.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3chgtrgya.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3uxxlndsx.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3gtmjpbsp.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kwyrihdx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ztbmioik.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3qtzdvwnc.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3dhwcqhuk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3aznpycch.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3huonepww.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3jivaelhe.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3bobghsji.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3wzrdidkp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3jxtkmyxr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3ixxlaelb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3lphufzfr.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3geovgihc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3xhlrgjnv.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3tjxpqfdc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3rcllzils.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3elnzuyuo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3dwtdtamo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3nnngasfo.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3rdjosecg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3njpeqyqp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3oblakrab.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3jazudbuq.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3mxblvbza.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3ouydsuxr.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3ticbgith.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wurmdzwg.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hdiafwsi.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3qwbdzzfi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3sxvrtyfb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3avliyqsr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3mfpcuypq.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3ccpxsulx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3hyzhxepa.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3vrrqtzfl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rqgwubxy.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3clsoayiv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3vgqluoev.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3mkvdynzn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ycxhykyd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ljlregzk.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3upnvxkrj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ofiveomy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3mwjymxeh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pncpbmld.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nyukglap.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3plgncufi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3eclkglwf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3btssgkic.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xmmqthil.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3ovacslrt.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3kxletmgu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3vjfetjly.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3uberfbur.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3xlghilis.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3fudaddvw.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3umrrbypu.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sbpddgaa.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ibeoylly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3elgfqpig.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3alhvmsso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3afxpoxyj.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3wdvumuir.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3jervgjbd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3fttigglp.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rzvizztu.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3zjomtzlx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3wpxkkpzs.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jqmyajkj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3ejhzcfve.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ggqlridz.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pqnvaovd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3tklkcgpr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3mprwsnjl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3tmgohkew.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3hhgzkocq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3jdunzmzz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3zigabeku.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3bpyehunb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3kvsqlngb.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3slsrqwpq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3ydycwrhr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3ovivbwgd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3kogxyjxz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3lvvjzepn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3bjslfjnk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3senpipjx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3uqvhudqc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3wxkayxzy.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3duwwkecu.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3ctngpgkf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3scxmywjc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ysvquvfn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3jcxthebb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3gfincfxd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3mzjmijwc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3jatncxkn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3yhvbohei.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3yionnwig.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3rrlkrkyf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ktyzwtbl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3jjtxprez.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3jywegazz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3vbtyzblw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3bwvsttpt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3ehgeacjg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kwbrguhl.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ecpbevlj.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kpijkrej.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ncxyckov.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qobaankv.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wejswqnp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3rjabzjml.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3azscibue.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3redrlwag.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3coyoxwvx.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3qdszkqik.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3kjalvlvm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ymzzlrcu.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3vvkmgwnm.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3nuozzjby.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3qwntvjgc.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3vzyxkqmu.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3hijynaxy.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3mfvkxxqz.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3szyjrseh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3uzkgyygt.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3bpbiqwbr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ucqrxfxb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3czpvntur.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3cmgfyhrh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3uakjuczc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3bwagjrjz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3iguhyafu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rfldwxby.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3qwuzsnsa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pmrywqvx.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3sicpdmhh.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3novoizku.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3hfwnjpjy.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3hgleaijc.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gxrrhnye.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ueixpkoq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3amkmzjha.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3kmzvognv.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3lulrzpvn.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3iuowshks.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3uwvaafsd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3pxkasukk.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3hvpknfyp.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xzmcblju.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jmjeyyie.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vtsgiase.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3jhmewzys.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xslsamjc.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3fggkrljx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3syiqfxfg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3qaxnqchg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3jikopmpp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3peqrcgsw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ayuiscnn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3jobvvvcw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3fntyegfr.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3nolqosrz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3lbgitxtz.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3qpqlladq.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3iacmwwxx.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3wbfvvmrz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kplaytuw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3cegpgxxn.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bvmyqkag.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3huxmukfy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3dkkpdcuu.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3arqrvnum.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rdjpchlk.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3meqjphsl.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gzhyskld.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3izbnkfys.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ftyasyzx.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3swaflqzu.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3foolpqlf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3mlsucrjy.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3iuigfkwb.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3mrrhbigh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3pvlzrjvc.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3vpzjwotd.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kmezlgap.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zccsilsh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3tvmhitoq.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3fcgzgupy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3lhkmxvfa.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ieiyttcl.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3udgxbldx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3tgjctbqo.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3mlbxorgv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3aihxivel.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3hwbzfdvj.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3raghiecw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3aoojxgtp.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3nuznljav.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ldgyncor.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3xqrkxzdm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3pjreivme.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3uxpqegfz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3zwsqhuoh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3bgrrlfdf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3sxqqsdwp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3aiakoqfy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3klrfjsbm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3miuclodk.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3xrylodzi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ahvkkbet.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3djxfvfsh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qmznzlxj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3pczfhksq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3nmtyzllx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3najmqcer.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fefayxoo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hkpkwaul.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3zwdxfyfa.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3krsumyyr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3zslwarda.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3xyixjksx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3uxjzabxw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ygqroczn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3nxfdgetf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3swoklxkz.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3kyvxmexp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wtuvsptn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rlxzvpni.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3pfkkvnfr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3yglrdots.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ngtzuhun.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3eaynvvot.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3dgfwphck.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3nruegjjf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3yeiyfafb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3kizsebsb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3nwsnduex.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3mjrlrxsg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3jihdffiq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3pouimqtj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ytbtszng.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cmlvhwxq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3yracqddr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3biwyyxzi.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dosjkqnz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ajgjjexk.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3iglaiver.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tloudmgd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3zxkrysjz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljfsoypi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtfujrjj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3dtlhrelq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3reboulza.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jvggolvi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3tkwvojot.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3llooyczv.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3auzivyvx.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3aicilxhp.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3imkppdkx.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bmsbceyb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3cenirjho.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3uqrrhzfr.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3bmtblrdv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3gjewujqn.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3hyedgigi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3rwhjwmqb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3qmnratbu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3fbrgnuvd.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3umgkrzdm.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3vhklckqj.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3qloydqnp.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3setrsgpa.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3eyljtjks.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3skbvpvqt.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3yvmovqwz.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ztqqkogv.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kcmcmzav.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jcvrkrsf.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vpvwbpba.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3sjfeeahy.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3rcmoloxq.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3oavfbjih.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jfqtcyio.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3yjkwxhri.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3yufmrokn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vvwhwxza.html


<!-- 参考信息 -->