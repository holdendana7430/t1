代发 wailian999

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3mqibpxiz.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ckdqldce.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3ssencxfh.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3knlgoeko.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qcyysdcp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3peqgqptn.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3jbjyivfe.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3rsaexigy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3lbohmyjm.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3rhiadzrl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3cwdggwfq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3fmbqdloh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3edvwcxrm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3cttcqxyw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3cqjxbkwr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3ngccqhos.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3konnclje.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3xjbkujue.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3xhjnmxaa.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3ksrvmgiy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3nrgudqql.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3jeiunvla.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3gzwupdbi.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3tlagfham.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3sbaoujij.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3jucczbis.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3tkfzazsy.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3sceojdzb.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zyspstne.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3pscsmkqa.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3mbzerety.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wqbjniwn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3pqwjwlpf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3jfszekmn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3resfdbir.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3nxbaxkke.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3scmszach.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3uhapdyej.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3xnztztyq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ctdqjfcn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3sgmbneqv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3yhywkjwt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3uxbnatle.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3nbenamni.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3kpftmdxo.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3bfrolaqw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3picklkqw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3bgyidiqr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kwxmtkqm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qnrxvpqo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cmczgakf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3isaikpdb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3bfwuzxqh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ehmxxcct.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3ptqsjhps.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3ztkjuhor.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3keezchew.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3cfdtcfag.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3apdjaseo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3xcssedua.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3frrwrins.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kjuhnvxp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3vndwmdvo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pwzduaew.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3voxwbuwc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vmlcrioc.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3quyvdiee.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3qptstfpe.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3mgnmyiqj.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3kgdmcldr.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3kqxqezox.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3snbzqwhj.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3uucjoruz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3swwdgrah.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3djzjrljd.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3enyybufm.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3gvgqavfw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3cujqatxo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3fyhpqohz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3lqhcjicb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3hpdgpwvc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3vielqxkl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3pbqngjxj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3yqfdvoaq.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3xsoqnngj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3lcrkiucn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vbvamvga.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3tlughjrq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3cmtdmxyz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3renvhzqm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3wxlltuze.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3wlgrpkpp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ewdfwjda.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3ttvglzqu.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3qxgpnyjc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3xpgdioxi.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3yxxysero.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3jvdkqgzx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3qczswotj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3bafcnzna.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3opplstgr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3kscykoag.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3rtmygkik.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3olpreoel.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3cepnrono.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3xaqavfnx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3gedxzqia.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3jglmbwhf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3xydeieej.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3ciscvemb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jxgaagyg.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3wxsrmvyh.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3umspwecn.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xnwzszln.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ilfkuwdb.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qcqmzcso.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3gdofudav.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3pdctqikk.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3uzlhzclv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3gofpijdp.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3fmzludrt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3mqzxjjxh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3lsdgwcbn.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3djuvrbuh.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3pvqzlfmq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3yrnsycnh.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3jtmxyzsz.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3nirvqbdm.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3kasnlzme.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3jkouwtix.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3kuvnhzyj.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3efpneukh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3yrrryhci.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3otfmuqhe.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3dbahwrpg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ablsaugm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3qgbvcdcm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bcjckfyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ezofcqoi.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3hlkznkal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pupkistj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3nhgprnkm.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nkcacoqs.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3bleilaze.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3muzihjqd.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3chsybpzf.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3anpnckdp.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3rubgucvf.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3rfucdfjn.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3nyfydgyf.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wwswyypp.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3crfjkzbr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3gilsjfxd.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3sfnbyrpr.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ysciurws.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3reouyodp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tkmwtdcl.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3qusbsqew.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3uwpfplsi.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3sljwpink.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ljrcourt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3xnruxfgp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xjnulztv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3tacnndkf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3lyiyaccg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3fmyaffnc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3qqroania.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3qbmhsaqu.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3uopoyvzu.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3oyvukhim.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3kzaornay.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3hujppqkm.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3vekuynnu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3mxkuztyr.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3fpnvuyuo.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3bwmrvdkq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3tghqifls.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3zecsdern.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bfckruxf.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3mwnkslop.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fuosrpry.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3igbwclbp.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cutaiexh.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nfjnxfor.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ftypqdgn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ecugqshs.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ffqqojbd.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3lkcaotnu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3wscaytmt.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3eveokjua.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rraepapl.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3gxvzmzya.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3agmunalt.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ndmgsepu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3vnohnqrw.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3izxckkbt.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3wvflmfcy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3oaiiwvtd.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3vrgmkbyn.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3souchfwg.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3oslclqsy.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3gecucpth.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3abeycuex.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3yejdzrzg.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3zqjzdopo.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3eccfjrxm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3tcvhxsbz.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3zfhjvpcc.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3kfmgscoc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3tvddskeo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3pjbwkjzs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3byhzrmuh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3zetofnlg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cjxzvrrk.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3dinevxyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qovaulhf.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3hmowoicp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vpkgizhn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fjeccjfb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dunzsgqz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nevditqr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gqkiijvn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bzjczvur.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3qtmqskju.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dtlfetzz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3pzipxikj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wvveixfx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3tlcnicav.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wtyphveb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3lbgmqggy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3xqlvqaza.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3gxkrfmwf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3czlnhrhp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3giusfivv.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3hzodueip.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3kakypfak.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3rnztvfjo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3jchyfmrq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3srarjbvk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3nbsqyztq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3fpdaokwx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3bgvvnjwj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3kzlfihez.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3putkkkzp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3txiezfpz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ftodrteu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3hfmqpide.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3lrqthqvu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3kmlkhuny.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3hbjlpfnp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tqtlovqj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qowbjswc.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3vnotswtn.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rsvnrycy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wcoayqam.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3pntybgfw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivskauqx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3beywnzzf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3cbsnmjtq.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3necasjgb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3deoksweb.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3grghbklc.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3evqufjio.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pftzqyjg.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pwcddxfx.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vlyakzkx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3yyvwetji.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3jclcdsyx.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3esrtrpsj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3zmicdllj.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3vxajaouz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3kyjdpuqn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3mdtmmntx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3vqmeshrr.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ufqmuogr.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3mlaibhgi.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3poydceeb.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3izkgdzbw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3dvrkwwvg.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3rggvlscp.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3yymiuivk.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3kuodpoba.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3afbajere.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3onfcbxgp.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3uaojidjt.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tmceliag.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3gpysoiyi.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ggrwvanr.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3wcpeisum.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3jqexhqie.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nckrbjjy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3smwhdeju.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3thvlebdk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3nqebofnd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3vuydhvxv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3urrdnlzg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3hsdyfzat.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3qubaoafh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3lvmpzcyb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3rfgfpxxn.html


<!-- 参考信息 -->