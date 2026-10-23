代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3idzwcvte.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3fwpadtqy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3bvwwzdlp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3igqblemp.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3nilasoqw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3nwvlmqzd.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3jsvsrylr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3vhhmsvbe.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3ryheqqlg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3jozfhfdt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3fakwvrtu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3sistkpnx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3gnrnuxkj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3epqjdydd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3uehcvipu.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3cvbfgdbq.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3ennphmse.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3deipdrcr.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rjzwfwkw.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3oaoprdil.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3dsrhyyza.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3zkwlrsuw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3mxjnqotv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3uuinzbjv.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3whwxutjk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3etgrjjoe.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3rukvphfu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yjfzgujx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3wyfkwdkm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3gwbpdhqx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3wlmkppne.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3lbqnbydu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3jyqoknnd.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3ylkzejff.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hfzrcrtq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3seazdxwv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3twfjefkf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ixyfissh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fchwsefy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3euuxiqph.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3vpmuhkbu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lsbugfze.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3irxyjxic.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3jnogsqgl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zdczwinr.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3cbtylszx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3dhmckjrm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3yytldiiv.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3davoqluq.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qowoubva.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3majqpgxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3prajmozb.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3dmttldkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ykqbkbyn.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3orsmgztr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3fcblalxo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3vbmqcezt.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3azenboug.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3tgirxdii.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3qedvurjw.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3ibjmiwnr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3fhsriper.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3cjzqoala.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wbhoabuz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3lxurmboh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3yiprykiu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ccpaowsf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3tsguhfmx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3wxdmxjmu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3joijajmv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3etuswxev.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ykrtdtho.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3inhmnikt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3deoiomjp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ypqxsmsl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3gcquvprr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3uyubyfrv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3pkujjisx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3rawptunb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3xxgtgney.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3lfwaaxah.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3jtfztlns.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3aekapqvj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3pqkapynp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3eznkoszv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3tuedmurh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3tjijwhvi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3aggajifm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3pdgqqkjj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3wssvwkwv.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3gqcixmko.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3skxpcxat.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3qcldzbkj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ygxeyxtb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3wqnapmac.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3zpluknvs.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3yqezeaux.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3fjoafrgj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wbadgmsn.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3qvhltgve.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jaqeqkca.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3ovupqvsx.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qcbprepf.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3oikkglle.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3rzqgoiny.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3jpcycgnx.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3rtfluzmj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3niilkemm.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3swbecswu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3bhjoyzaz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3reogxqbi.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3eqgsbfkt.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3rlpcmjhl.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3icgttkks.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3xpqsqfge.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3gdnslpwf.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3esgtewyw.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3tmjmkias.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3hzydzsfv.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3gexsgdif.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zfpxciej.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nvihgone.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3efpqwrgi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3lchlkjoe.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ggxgxnjg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3dwmkwynr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cqmnjlkx.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3zmhcqkqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jbtlnzqz.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3mddlrtxw.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3qyxsufop.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ulwjacyf.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3cpbztbdm.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3hrfknffv.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3grgtyvae.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3agkjoywn.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3onbpysaw.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3rcqdzqmn.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qsvqhvyn.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vtjxqlgu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3keufjvpn.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ouyezksj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3layhizne.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qihwhybo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mvwdovyz.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ryffgkbu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rpbspqxu.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3camkumlh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3cyypnajq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3zrdmtaeh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3futeeima.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3elvmewcg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3zybptozq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3dvbwclkw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3bzhfpels.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3ytzxlhxa.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ggaqekoj.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3jnluljxc.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3dzagzbfm.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3akbvblor.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3plpeimfw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3werulxev.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3zqgflrxa.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3lzdcnikl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3qcqplvnf.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3orrxannu.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ahmaprbh.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3itsxjcvv.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yjvnocuk.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nsyouwpp.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cxocejwy.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dsjylmwb.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3verrirpe.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3uqgwtkrq.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ydqtmstj.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3lgahefhi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3qigekpne.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zuijfhum.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fbpbimat.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ymtpmcqn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3wsqbpwbs.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3talruatg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gyhncves.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3bonalapl.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3kluitjmp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3yhawyfql.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3gbzqyytx.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3npentoyk.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ligxsdtv.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3irrrmmqr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3szxebocv.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3iyalzxgp.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3bugrpoic.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3gkoxyqso.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3mfjxvnjc.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3vtkbvfrn.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3puneamrv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3xwbpdldg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3uxbfoops.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3juppiwyg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3jcojhfgh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zhvojhnv.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3vxnhvmtb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cibaxxjl.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3okjekxnr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lcoemvpu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3utyitcam.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3djbgmdjr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nugfggkm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3oikevaca.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bqhkwkbp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3azotowho.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jiiowben.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3ekdvresw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xitalhyl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3wudoajxm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3lzomixmc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3fxjrxenq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3auvmcqte.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fgwtaloc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3dgzsxjpt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3bcnphbkw.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3zvqqacho.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3tazyalvv.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3epcipkkk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3zvpusakw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3jwmoqphz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3mwgubylr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3jklxhyka.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3fapymiuc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ginislmx.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3lpexhpsv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vsuqvnuo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3xzaoukal.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xpjajger.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lqylpgsl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3wsxzoior.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3gmvedogr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3hydudkus.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3pjlovnoc.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3fwyeuhey.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3csqdxelo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3xeosjctp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3symydcdd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3asigedie.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3okbnvuzw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3uautaeti.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ynagwoee.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3tyytqwmw.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zvxmfemf.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3bogwlfuj.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3dmjivbvd.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qikhwajc.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tsguayyw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3tlvztyai.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3knbhxtle.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lxewrvon.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3emlmgant.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3wfpdahbr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3mhoaexip.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3usedypde.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ldlvadyt.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3eefgkdvl.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3bpdwgouo.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3tyxuqsmz.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3erloxygq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3uumwjcsk.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3gygqqwbk.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rrldujtg.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3kjgyeusf.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3foukcdrv.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rmppouyk.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cyhbmvof.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vppsyhev.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3uagoqfka.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3spglcxzp.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3xxkqipcs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jykuifhu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3yuxovcdn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wknlyhqy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3xlaflqij.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3kuwfmtzq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3wlnldzjh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hwqzxtew.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3nnewnmaa.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3arzezgvl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3qtvhwanp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbdwrqqs.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3orwccmhn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3bprfcnjm.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3uuhfijfn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3rgwrsnlk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3vhxiaujc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3rittywkq.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3enuhkwvh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3mrsdvzjo.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3fnrrxbuv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3qilsvkel.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3vbttrnps.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xiqqucik.html


<!-- 参考信息 -->