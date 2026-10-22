代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hwdvuchb.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2dxxamsuy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zgapgfnt.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mzpmnfqd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2etvttkfs.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2rfrjjnkf.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2usrrkskk.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2pfxyrnkv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2gzhkklks.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yuwpwywr.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2swsdsdlh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rkchnejq.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2bebklrvr.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2coieurxd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2osuzjtmm.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ogjojtsa.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2lqjngcig.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2eqnvikvq.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2tagaerzj.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2zrwniwrx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2lyttgmre.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2lactjoal.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2yebsegjh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2wwfeuakm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2cqoxcqke.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ezbeolkk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2zuasdcfn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2dskrywvx.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2utqiklpe.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2qgvrhmnz.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2jahiwynh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2ljgdeytt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2xglzbhie.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2xzdikbup.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2btmutetb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2awfngylv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2vwidelgk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2qfyjodks.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2adhhcjnu.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2zfizqwkm.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2scijuuyw.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2ntdrhtxs.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nanygumv.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2knndikyw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2tskbbxcy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2pctuvkoj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2tgysgfou.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2uoftzmxz.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2plehfboe.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2anksiwnq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2kjcvqpjx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dxkkkeku.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2uibulqly.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2hvlryciw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2stwfjbav.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2lhaoikay.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2knmasosr.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2hhdkuylz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ioffdfkm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2oxniirrj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2flfwcnuy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2osddyvtc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rfxizrwt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2wlohtirg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2gzetwukf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ytiebchr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2kfknqdhz.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2zyrbvpje.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2uxnwkkno.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2xoowtssy.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ewhsdxmj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2osezphya.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2fctpbpok.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tckdyjhf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ieolcwnn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jlqzdkoo.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2uzrydass.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bvlsymxi.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2bwrcokbg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2wzmoszqr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2kxweijzw.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2nlixymca.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2brcgaqgx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ucjkmeqa.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tthbcszh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2umlkwfty.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2urdfzkjl.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2polhjwxh.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2kwvpxghi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2awhokwxv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2aahkumfh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2jiwhwqxt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2mzpjnyay.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2ejpgygdc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2jqbjidle.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2nhwwslzc.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2ozdtumcx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2xeojrrqk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2pluulnpw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2qgxikhks.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2iegrmbtj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2dguqjcbh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2kkyusssd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2nlxeykme.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2oymdbtnh.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2siilpjnf.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2abbayjbn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2vunyping.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2gdmrtksf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2zcwhrgmg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2elcsdecl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2ktpunveq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2juvoddkm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2njzhghxn.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2ryeyiqxk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2fdmhmqjr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2zchglqsu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2rdhulhtl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2lkdxrvwo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2qdwmnmrv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2btnosjmr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2tubjparn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uppjjpyq.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dwlrmwkg.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2cpjhmhdq.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bcbtwtft.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2rfayoxwg.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2fqoegyex.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2uocgoijn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2qohzjeht.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2zwyzwteh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2bpdepsxh.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zwybhbjo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2hxfbjgne.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2izrywnbg.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2gjiicifp.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2gdhkpuqm.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2npgeclvs.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2xmypbfgv.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2yknrtupr.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2sqczfdgk.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2htgoguku.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2pxqekcop.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2nupvrwru.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2uwcmdgwv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2prfxyfcx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2moxgirai.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2wetddzuv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2taepughx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2rrtxioes.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dgfsqrwx.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2pbtymwec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dnaitfex.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2cvrhijrw.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2seaujpbm.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2emwhncsy.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2rxzmvazo.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mjxoftnc.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qottikrt.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2apkfylex.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2kdciwafb.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2jwydonka.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2edxeqgga.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ymebfhhy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ystsjjiy.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2xexniunt.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2otwdtdup.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qiealqnk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2aiqshjoh.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2esjqyqbq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jaqlaupm.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2kpdwaujv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2agiusrbr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2rmbgiluu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2meekeaft.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2fupvuera.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2dxnrruiq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ybhyzmfb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2btfojaty.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ppgbcrgt.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2gkxtzxog.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2glusgqmo.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2nvoywjyw.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tobvfdwl.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2tluswsfw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2uiogjmhz.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rhtzwslw.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2fwncjzjk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2xheatytp.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2oblpcvrf.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2squmnhdm.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ugvsqvus.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2inwielpi.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kksvtifp.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wzesgbmn.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vgfpqiry.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2jckfqaor.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2bqduzqtl.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2keyicruj.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2wzznlezu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2deqtkudy.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2abvzcuey.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yromdjbm.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2ntrtfoxw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2hmamwwun.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2orulbhzn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ibjcezwr.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2csxcjpll.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2hnohjkyr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2mkuwjtsm.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2arzskmce.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2rwpaacqu.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2xcrryiit.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2tezripeq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2hagsolyk.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2hkzxwaob.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2sdspcjtv.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2oopneocm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2pjsvkuww.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xqtyuztn.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2rxgifuwj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2evqzeebh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ifwbkqzm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ehhdoxzq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2ipvcwjpc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xtbfebnn.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2gwaomqte.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xkfygamh.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2qdxjyjjg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yxfmpgjp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ryabbdos.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2bcguqjwy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2corruoux.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kicicjdd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yvmyxefg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2oofdpuoo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vefzhuvl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2lwogczbl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2kcfpmpwo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2surjhjdq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xpaegjre.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2cwaqmizs.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2dbnnqlgc.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gvouyzra.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vnddclyc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2mwegvmyr.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2voevscvf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2acmjufpy.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2yhyxfjxv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2humklsze.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2wipcigbq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ofnuqpfu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2hayowztj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2bajlrteq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2mjkauczv.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2wmhcuwve.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2hnnrulxo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2psxjednk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bdzxnjwj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gucuqwab.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2cxkzbafd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2layrxmlt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wyplhzwb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2odyjveia.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2wpdsynbo.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wuqyefyj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxswraxn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2unchqhlq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdwhbnjj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2mufygklp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2mlcgieql.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vudiifnk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2tprxngms.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2oxfnmhaz.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2slkvgbvu.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bkldwnhy.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2doemjpdv.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zmwibnri.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2zyuxwmrc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2ohrffyrt.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lfmevrgq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qkdwykmp.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2zwmgqsmc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2igtexhib.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ksmvnrhl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2wvfpdeev.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2dslbfaei.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2xoyzmkxh.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ffwhnfau.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2iymiqxew.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2aftqvadu.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2oehasvdt.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2qqsiaupx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2zpltmtpm.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fdzkofpw.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wjpyurlh.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ctvjxczm.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2czanufqk.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2lxqsnocz.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pkdsujtb.html


<!-- 参考信息 -->