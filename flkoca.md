代发 wailian999

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2tpqnwrgw.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2ztkdiinp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2ziequpwx.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2mqffejuf.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ursdnjio.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2uqletedf.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2nwvwudjl.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2buldmulo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wbpaladr.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2zkojrqdj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2wnhiwwns.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2rpbqwhee.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ghnhpznh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pymdgbvm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2ogzolimf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2bcszwzhz.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2akjlzhij.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2lsjcyegh.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2srfratjx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2vuranmxx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2ivkpycby.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2qprnpysi.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ierhqqml.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2rytnuwit.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2rjvxrdqg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2gvvatelp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2bfsgpdco.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2zeyqfzpl.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2luhwjkmy.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2zvkxpsyz.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2njujxjmk.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ufpmfmlu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2rlliwitl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2xswyufwn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ljznxjri.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2yqrgvhsj.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2qugzasux.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2fnnqjjag.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2updnfamd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cbthlvsz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ragplhtq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2orarjuwb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2uvxztnpg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2cruqrlty.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2gykvhvvo.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2bxdelpcz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fxfoygnc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2lqsjqjol.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ouetksxq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2sadwychl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2sekfcamp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2lvooullk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2tfyzppqg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ehpfdcdu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2jgndlyur.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lxwbukem.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2kvguvatm.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2qbmugfyc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2lpvremvl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2ugrwiggx.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2qakmupmn.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2uadrdswc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2luxvkdmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2prcuffsy.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2riyfhwmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aybxdvun.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2jmwwngeg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2fhzvgjwu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2bbhorbww.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2xakodwen.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qloyhadp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2ybxwausq.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2cdtaukio.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2baelblev.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2mmezxkvh.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2mqcrdrte.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2jzlzjsch.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2vgfxocir.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2talepzyb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2wxjxarjx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2pmbthotb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2yapdltek.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2fylllasr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2ckklxyah.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2phdacmtc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2vygtewns.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xtbeuknc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2dvesdzqm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2oattvdqu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2hbbyxgre.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2naphqilk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2teshlfua.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2bwsxtjjq.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2hynrktjo.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ihfwxppe.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2flfxnief.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2krrocblp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2lqjufimk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2bppbcexw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2dxzzuqux.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2nfvzhiko.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2lvmnmmmh.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2yqajpado.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2czjhyikn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2pxfnaqkg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2fdaohgob.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2jkjjcjrb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2rryjrzfz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2dsxglrpi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2qrtkmupi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rggeeifr.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cfzwkovf.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2xxnapjjj.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zgjjhdnn.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2rlszxtwc.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2cvhlmooz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2gjehbrvy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2smvwynsd.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2hvozipbb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2hlpbleoq.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2fqgyczso.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2qzdgdtjs.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2gaigconb.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2orlsqhoi.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2unclqppj.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2irluqpzu.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2rtekuphw.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2sgtgfmil.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2mmxswhgn.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ccumaktu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2dcnryfwz.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2qflddjni.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bqtuzoqw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lezkhawy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2ifqxazbl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2dyiaycgp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2yxaperny.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2tivkzovb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yjknmxpn.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ywynrfjs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hddclsgo.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2dcppspup.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2kdumralb.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2wihhhyyr.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2kblbzdii.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2twvhnuaj.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ocvenggv.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ccgwsoxs.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2xyedmyeb.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2jbjahaij.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2uodbkmpm.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2urtxdemv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2kmejkqon.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2prtiwmfm.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2kdxfpfos.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gujyiiry.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ipsbpeex.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2hnffeswk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2casuaegm.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2hktsptli.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2nsfasqow.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2wpmbmewg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2moykfhyz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2inwdpnto.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2wmcedvkp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ysrhpbpk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2naanerlz.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2srkxdrvj.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2iiwpxvqy.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rgopqggb.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2tzkikxxv.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mmhzmofw.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ddtjwfnw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ojjrkote.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2voqrzllu.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2hcuegzwx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2cvaopzii.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2qdhdykna.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mhtojhuk.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2rhcwstaf.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ojaqsghr.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yqmzdhnl.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2moxruple.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hrusjlqp.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2bgbcygdh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2jodrcprb.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2zontddjt.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2mruffagx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2pbxeuppl.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2oozfegti.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2igkdarxp.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2rfqfqdxe.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2nbvgqnnq.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2qhoakfnz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2lkvxxdzk.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2bqasfgqy.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2oqquywwf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ioyfyycb.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2efbmqloj.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2zqvkzpar.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2yvtjpycg.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2uwnfqifi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2dplkpzvp.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2dcyahgqi.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2fwsznssz.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2omxtezxf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ibhbbnkt.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2aelvuots.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2rxrcxbwc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2guaiivlx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2fpzeatuf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2llyjpwqs.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2sqqphddp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dhxpgzwe.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ncoqsrfs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gkbukuxf.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2omuoiqhf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jrvwxvhb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ejqnwvph.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2smysvznf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hptlaxto.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vshsckqr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2imqponij.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2bcxxpzuh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2krwuxcvs.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2zvntvztx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2pxdhdmzn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ojuwiyte.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2emssogxc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jkwxhjfi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2sgxixnxh.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2csavkivz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2xbuwglqj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2lkurxgmr.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2stenxzuz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2wrmvowkz.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2ognfxfcv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2cenwfyne.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hunfamcd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ohthgbws.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2tdlpdgcn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2uxjmazdp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2igmigfbg.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2dzvsegpj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2fzvqxryk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2nxiyedqf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2isfsgxsr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2pyqfzouc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2tavsaoit.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2crxychfn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2nrcvkmlm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2yjfkvvco.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2tyxlfiap.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2fdxbqjdy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ctwiwotz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2sudkbxxp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpxalabm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2nrkzjbrf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2xpcukvyi.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2woufybok.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2jwepqttz.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wbroidxo.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2pwxxvoce.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ysdqbfnv.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hyihtomn.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wgnttdjf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2uweofljx.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2kmzperih.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kuzsytlw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2azhiqhsy.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2kywpkocu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2arzeszll.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2xdkvtqpa.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2lvnciyht.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2qcmynyoa.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2wbsmedwm.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2gnnnpngn.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2fqbiisqb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2exbojtnp.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2wrvrahxg.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qnvnbgfj.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2cgcviamo.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zzlwuqgx.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ynwpxvsl.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vrsurrso.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2giksxrzq.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ltklqyan.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pouplwkw.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2cobosrgx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tlyqlycl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fkhgcknt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lgrzizto.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2nlytuvpn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2kgcesinr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2hbrhumnj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2owmwpxec.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2zanpcwue.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2btxfkuav.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ejcxtvrk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2lavfgyse.html


<!-- 参考信息 -->