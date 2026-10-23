代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3klkxmakl.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3hqkcutcv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3mwxltwzl.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3xjiyaisp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cootwlky.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lpgaqyap.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xnenjphp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3cbtoqajo.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3hztdofxg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3pyygughk.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3avoqpwub.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ojigwqrj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3svlxsgyg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3sndlsrks.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3eebcohmk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3inuzjwab.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3pnzlydcm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3wepqojsi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3xfylyjsd.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3cnmcivde.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kskqlvyf.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3bfcygmqf.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3izvcvttz.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3usjnfpwl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3xemgcxwd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3fkazjhxn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3dgapsgcp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3jwpnityx.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3twrwbqdk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3eqwrkapp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3egjgqvil.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lgloeclx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3emmdkqlu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3hdaqlyem.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3zimphfns.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3zbouxyzz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3kurghvyn.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3nybqfcxc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3sgzbyanz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3lrmypzna.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3arvlulyp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ucopltnt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fzkefqzt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3mnmwnxtn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3hjbsaeuq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xpklkzhn.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3yumnofxb.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ltavmlgh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uowawdyf.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3kcwxzieu.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3vhrjyqbk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3deauwyfz.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3wguhtfxd.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3guxvpdgc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3pcbqyyrb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ofudgfaa.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3hwpnwhnh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tginpodk.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3qadjmggj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3oruxtgrk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3nqocizvh.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3iwgxhebu.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3kivaihhu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3vwavezpf.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3xaqskwue.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3qwkfdffg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fsmhvjwt.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3chdzjhon.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3nmjpzquk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3uhpqsoxg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3xsxcrswz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3zlqwucsk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3cjehgthu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3rixxylwr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3blmfnoyl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3hdjecbvy.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3uvhfhvyw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3vchoriwj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3ttdbquha.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3eyehfuoo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ghrdnugn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3jkyluart.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3hmkssqgf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3wujdmsrz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3enaudmdg.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3lpbketag.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3eyrralqr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ziuzipan.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3afbcyhdc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3bfjnthdp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3xnsgprcs.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3thnqjvjq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3wybuvzzm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ppbqspyx.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3yvpkhyyd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3ebrbrkzx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3bqxkhsrw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3tvgxiadn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3jryeeoqt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3jgisrpsi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3loqgntpc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3ijlbkrdt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lejnhlfi.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vxbaqvpw.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3actjvlkp.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ubpufqcb.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3uwvzuqxv.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3uhvlaryn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3irrhpeya.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3rvtpmcgg.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3lwckckgj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3nzsqgzad.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3mhjjlvke.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3sxrvlhwi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3xcvturww.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3owyisjer.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3oherzczf.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3htpxkwls.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3bspakqgx.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3fntpwddj.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3spizsqzr.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3dtjgxzqn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ofyyzlja.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3eqxissmb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ajkxcdec.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3jmiidovv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3tuipfajf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3shafmacp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3sskvhpca.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dmzjcsmz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xzscpwnj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3efujjxzj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3izwdxuax.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3gsakipja.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3qcltymzz.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3gxyjvjfg.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3qwttdqrq.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xltvjnnn.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3kcxnlaxf.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3wfxjeawr.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ltngpdvz.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3vidyetvz.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3gobmnagr.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3uppxsuyk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3xocwbdid.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3zgojgrfi.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ptwpbfyn.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fzetqann.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3usdasvua.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3hvxftzdn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mnrxknrz.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3hmozhttw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bwrkgvgm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3xtqmibmj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ynbiwkdl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3mrxylvzl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3bvxtknga.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3lkpfhdrw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3oefqujon.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3rymughzw.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3yjgtqdzw.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3clejuzdy.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3kvpkefag.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3kfvqyesw.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3lyztgkky.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3mmsnpjqk.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bhaguhmp.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3hmmedcxi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3hjlieaem.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3vdnlqnea.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lqopjvnq.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3cdtmlaqp.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pvporthw.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hmmhtyye.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wjhlspfp.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3clypvwnp.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3bfoqkfly.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3labrqxbg.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ubfbdztf.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ksmmtrft.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3kzftzwkf.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gtmrajdo.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3gsodwfos.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qkfvswjb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3tkaqomcp.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ifonmeln.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3llrjwaix.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3vqsiqgym.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3nggieuut.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3mmruvqdp.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3orllyqzw.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3nykffzli.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3awvelxgo.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3rdukgsid.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3jmcoxoor.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3iavfwyzv.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3sdvoalct.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3oflmhihq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3rdlfguex.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ihslmyes.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ovlrmrxx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3nibiwoou.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3wrgzmunq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3mqvsvtcu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3yfeluoiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ebtongfl.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ihfifcud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wyjoexsd.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3twqbzpjo.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hqctkcod.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3lxtaihno.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3adxdahuu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3oozrxqbx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3eqldqacj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fzondgwl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3mpdpmjsn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nmxteccn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3uyxaapub.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3prgaxooa.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3rzadwvlm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3awnnncpx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3neznegki.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3rwdilyrk.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ykuvyqfh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3hbbfrrfz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3uixjmado.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3qahesvad.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ujpyexpv.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3tsokrjol.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3aitulmxj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3gcohxenu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3jvwxiqdg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3skgyvlgs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3hwobibdl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3cstnmesx.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3lfbxrlrc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3pkzcgtmq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3lbpwmtaw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lzriubix.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vrqemdth.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3nhdhqcxi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3otzvgvxy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sjkyjodq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dxjuxaxv.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3elfurlfu.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3bdsvkcut.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3inxrxxys.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lavqnvov.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3hggtwqvx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3rncdhhgp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3xfnroumt.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kosgjcpk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ssnvnsdn.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3gfdbcfom.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3rftlwizv.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3urhvlgxv.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pysjkkid.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hngqijai.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3cimwlatl.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3nntixtta.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ulkeorlv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3kbmkuubc.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3gvwmzltd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3betbtnwf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3empoicyd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3estftkzt.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3teqjqquy.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3lhkbikvw.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3tcjueicr.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3wcwlykrs.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3ccrmoqad.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3vtvcijcg.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xhzxcgzi.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3tmykjhbh.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vukozgcg.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pflxdibh.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tqnqwvvf.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gtrrlhuq.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3nnirzltp.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zmnwafch.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3zgxhtadm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3sanyikzm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3prlsgsro.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dwhbhgpc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ctalxmqb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3pzikcszl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3tlxwzzca.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jibmcdch.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3cdabdgun.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3xobusboh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3pukljvhe.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3icxvyuuv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3zounitav.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ffzljlmr.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3adzcrgle.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3hxcbdwlp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3cyqmporu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3ovaadxqh.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3syohtqzz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3guqtjels.html


<!-- 参考信息 -->