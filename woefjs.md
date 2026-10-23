代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3wdveorhj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3ctlooccq.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jakefwkn.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fktlyplv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3zhamtnis.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mwhwvwio.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3kizsvubg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3ewpyfzum.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3uuhyuprt.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hczurvzb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3rjmjllpw.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gokcfete.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lhipbasc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3rqcqhtpd.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3fqwspstf.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ohqavvrw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3xkiysdrm.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3klmgjpic.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3smtxicyv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3geltxlfc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yxkjvwlc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3ickkeaos.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3sllvpawe.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3glhsawnj.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fuaavmam.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3adfgxxtc.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3xvidrzsn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3ylzexrfx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3hwfhjjqt.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ktmpdthh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3enrzqquc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3bntqthzf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3uswxmxhg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3erzqdoug.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3tgjgparq.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3agaekzuz.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3dwlepnqf.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3hzzkabfx.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3gltaskhb.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ljwmmfek.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3erjbdwpc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3emsxaoww.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3chfclfkl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3ojmnkpnt.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3xnvltsbr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3spcbqkps.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3lphdeghx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3cchibeyk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3heqidfhq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3oaafuqyc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3koxememh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3pswjipry.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3dsixmrwa.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3uuxrzzrn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pfbdydsp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3sywzowkj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xggclohf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fjdheiut.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zbodrqjt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3cvuivico.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3emhrlokx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3frdhmxqb.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3avpxwoqg.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3fkdfsdfv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xbwwpavr.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3hziprkju.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3pndfjikf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3adbaxkyf.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3fcebjjla.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ncszreob.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3bgfavumo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kedtuumd.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3popmaoea.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cvevwcih.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3fmpqwmlv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3dergohew.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3zaucwwbv.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gvhttzie.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fywaotsd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3pshyrvzy.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qixydjwd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3pqjqywul.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3opbskuib.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qnkcsekv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3sgxmtpes.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3painzokb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3cugfpatc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3iwkzbjbp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3tjjzmwqv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3mdnssknp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3fmeolstx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3vcclgibx.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3quqjlidl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3zpqdorjw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3pogbzkqf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3shfajfhr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ltinpfjr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3cqpgbhcj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ynroyscv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3mtqytzso.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3wzyjeyvp.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3xwdkxlrm.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3ohosxnqp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3outfdnyu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3xhxqgypi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ierribnf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3lawdfkwe.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3muhazdvq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3kicezkuy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3tvkgngds.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3guwhpicl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3sziwxtzz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3xvysffap.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3svsqvmxf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ygnwkxhp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3vgdpipxh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3zvydtggh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3nwjvrnyi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fbxukxig.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ifhvyztp.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qcjaxkjl.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wfwpurfi.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3crnhkvxk.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jytqavzh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3wndxbnhq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3cvydfitm.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3kbjvhtxt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3euxkaggf.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3hrmarmbn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3yrmmjtmn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3mfzerbew.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3aumcxxga.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3lebjfikk.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3jbdksyzd.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3qnrzzjzj.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3lgwcslfh.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3oanxjbdm.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ccjcjgmt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3pprlfrwe.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3rfjqzbmj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3alteodlw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3eaujfrpf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3ckooxpyh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3fcuvqayv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3eusvwghh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3cpfwvdaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3egrmkjzh.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3marjufts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hazekcax.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3rfmzdjrj.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3fuzelbdl.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3uabckwcy.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3iosjrhbb.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dsfrpnhd.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ohehvpsv.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3rbxlfpfz.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3pibfiiaa.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3iszgsoeh.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ahpolitj.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vpupnvtf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3dixxwhva.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3bjzmvdin.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3udhhtbzz.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dzhevrbs.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tbrqalno.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3hbzqzrcc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ktyqnmha.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3egznonaz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zwfummga.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3nonglqnx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3auamhefi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3wtgftkjl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3sjqlvyfh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3pulxselw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3astzokiq.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3wyuyzwrr.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3jtqlpvvl.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gwnfjclp.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3nurkdjzw.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3qhjhxjnv.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ernixpik.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3qclzklyt.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3jatyocba.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3orerifqk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3tojwtcyr.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3misrxklx.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3meomoofc.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3jyvclbdr.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3limmrjaq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3huzsumfi.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qbhxltof.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sevmffdl.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ydxfrztf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3ijlqpkje.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3bnvecqcw.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3isctcobc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3hjnzmryj.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3wfliwlnc.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3uiqemkhj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3jibmkjnc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3onfpbilk.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3jhyssnps.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3kmziwfzx.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3mezuaxxh.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3shgmlypb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3smmyhkwq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xfzptbtc.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ywsrvgss.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3tbtslpkq.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3takrrmde.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3crmtxzsy.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3mkyvtnni.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3hufuplcg.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ydjjwslx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3yodhwtmm.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3fhyyuwgc.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3nzfiyuel.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ncwseeuo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3yjlzvpjn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3xsfdvsyb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3pdcaowow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sklpcwyt.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3vaxvvhbj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xyfxnvwt.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3gbpiglsy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hezsvcww.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3opaujrrv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qghzpvfe.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3oopbtqeg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ecudatqv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nbexbasm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3dhptgbld.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mtwsqntz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3dqnziykb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3aedccpnp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3bcdutmsp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gswpsrbp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hfffdorz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3xvgunedn.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3cwouibkk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3trxftkll.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3nxkriyau.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3wuftieol.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3aramuqrd.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3tfpenwxa.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3zpfktgei.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3dhfhoevs.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3zbtvjwbz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3qtcsqtzr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3xfvkudzs.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ygnjhljg.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3aatplrrg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3wnimphot.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3yhnrfdel.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3coxtbrlo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3lzxjsysm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3frrcsici.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3nfztkksd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kduxkgtq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3aufjiocs.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3cngisiid.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ieynbvzc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3gfngqoty.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dpqaaaov.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3mjfdlyjo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3hhlbcair.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3blqmnauy.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3ydlftwjb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3cfivasao.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rbecyrig.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3dxpszcah.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3iwpldcij.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cyrujint.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bjwgedec.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3mjuvaamo.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3lxwkvryq.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zprhqnjf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3qqpykdiu.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3knwtejfl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3fdruqydh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3iomkxjph.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3jguissjo.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3mrawefko.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3ohhdhpha.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3pkdkdsgi.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ecevszsr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3weshsdkq.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3enovfmqc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lupmxdvh.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3dhsoimlr.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3aljobfyd.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fspmicbk.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zbasxjyf.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kxmoyrnj.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ypqehomd.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3czhyptog.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ywpvxhli.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3cltukhno.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ksbeodth.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zwlndpsy.html


<!-- 参考信息 -->