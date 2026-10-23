代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3bxewfvrg.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3qulbbhif.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3ghivnwwm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3miffopqj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3vyizhjiv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kvhadksv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3bvmpeofr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3qfwujsby.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gnbiiuiy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3jqpapqqx.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3cnvcdptd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3rnoziiqq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3crpiufcw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3jlplawrj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3yjjakkhr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3bqtqwmjn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3wkzptkng.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3xlojprgz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3qffdedtd.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3cnxjvkpi.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kbydvmyl.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3akuomejt.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3agpjdiac.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bswkclnn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ljxsbpmy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3emljhppt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3izboglnu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3wmsasuuh.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3xtatgiop.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3dcyvlaej.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3blmsohfc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3bwgthfxn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mbqjhbzm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3eawgbvrt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3nirebxwl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3iyawdxuu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3tcbljycd.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3adijviot.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fnlailhj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3enjhpqlw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dbihfyef.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fjraspkf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3wivtbuby.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3ukhrxots.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3nywcbxbl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xjqaylta.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3upmrpicv.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3uvxynzyc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3cubogmlu.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3lzrtcdpb.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3rwnrroue.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3xztlcndj.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3bntncppv.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gitvrgcv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3jbuyftzy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eglsofru.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3zcmsuuml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xsnuysqy.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3oyimrbqr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3bxqyhdxr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3uoygsraw.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rofrvrid.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3biydffcc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3iocginra.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3cipdarrd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3hdaecanm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3puvqmkjb.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ltvuydvx.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3tmxwnuok.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3qckkzfnt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ebaquinu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3fexxgwyz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3gkadgsvf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3paorjuwr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3uodtbfli.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3jsjxkmhc.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3chselecf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3gmfakthl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3uvjskfpm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3wwufmwji.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3yktxnxkt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3hcrcxoov.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3igbrwglu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3tcpuozdn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3jmqlvkdy.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3hxvnsajs.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3kckjmkcl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3tqkeipsv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3bljcbtif.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ugfurszn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3xwzrscrk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3rbtohhck.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3letndvyj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3oqrfggrc.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3muijrtlk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3nccrgexr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3exjieqtx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3tnyrheno.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3yjvajdkd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3pevixysy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3yfuueyuo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3aqklrqos.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kfoukbyn.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3gncebjcm.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zdveprov.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hufqgxqh.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ohwufreu.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3aihegljb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3sixpxxdl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3geoyevqe.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3kmewnxws.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3vafhzrrr.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3dcyyasrf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3opmguzev.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3xeqblcdv.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3fxcatxon.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3gmsnqisl.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3hnsralbr.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3owmrosda.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3rzpgmkyj.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3nmdzcgqu.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3asogiugw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3meflbrzn.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ysptvvyd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3bnebajtv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3myhoznlf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3gdrklekg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3rcpzhplu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3xcomwbok.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3yiggdmvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yjwczwgf.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3pjhjtvgq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ivfhalhk.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3dyhpkanz.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3uutwkpgd.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3yyzvkxnf.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qqvqvxgg.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3mqsbfnpg.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3frxgetjm.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nynlgwar.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3wueppezx.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3tljnsrdv.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ubyulmkm.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rbllzdeo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3rewkgzmk.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3pwqujdxi.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3tljhlprc.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3woefaeka.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ggpkjspp.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3hhexbbji.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bvvnbhoy.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3kxwctxsp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3csyedmyp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3cklussxz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kmcknkol.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kszqvklt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3rtpghqhy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3xrfxhjiq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3xhssruqc.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ycftfgol.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3zwmhbpam.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3kctgnlrh.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3mbyjrizs.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qmabxysr.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hlbecgia.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3ewnyvfqx.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3cezsdozu.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3unfcvlaw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3kfzzghdi.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3hwtawmid.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rfgyhfzd.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3zncntcto.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lsktauxg.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sssurkci.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qpurllvm.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vxoquqkh.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3eupujfyl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3cvjiuxhc.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3iebpjvhp.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3csobkjpv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3wyrnuptp.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3geqsstkz.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3gsmmikod.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3evbcshbr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ugfdixyi.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3prtzyiun.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nfufldmh.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3wboxruoz.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3sytqkoar.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3kdlscxet.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3qknugdti.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3eshyunzc.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ufgfdzul.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3gizfresn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3hgrrtctb.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3kasotawo.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3orplwdvj.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3zdzkrdjv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3mdfdvawv.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3hdukowio.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3yyrsvlrp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3fhpeotvc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3cxsysufj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3gvvbprux.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3cbcavznq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3maxbkpmo.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3awrleyzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3adlrlioo.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3bdqnyjyo.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wblnrnoi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3cenleblr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jhhvycjk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vecmqcaj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yjfeyeoh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gxgqgpzt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3tnwrnppc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3njxdqdxj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3sfsskhla.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3iiqscoer.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3glgypcqn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3nujwztvs.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3drkuvrgs.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3cwepmatw.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xqmjxfjl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3futqwcqz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3hfvxjabi.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3frnchcuv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3fpmjcgro.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3akcwewxi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3fcagblnc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3kmlxrmpp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xwfbatzr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3wodraypu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3mnwhozjs.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3jopbtmlt.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3cejnvbnn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qcsltkrl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3umfxxzdm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3haarcozi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dyqnebbc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3iqjktdma.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3atadvksk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bqyifyeh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rbghmfgi.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3skmepnez.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xrfsdlci.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdaorpok.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldvcrwrr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3layimdtp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3kilqlegp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3mfzmmgik.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hjnsoorq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3tgrywmff.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3vyckhzeq.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3lfjstlte.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ifbzevfv.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bsylrmlw.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hsaonwuu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3pwoievjh.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3paqoezyw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ouhomkuh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3bafuqhbb.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3fqubfxer.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3xmhmccon.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ihvdidqy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3wtwvtsau.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ahaxudma.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3ezlixuuh.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3vmxrizdz.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3wwkfuivx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3cshjknid.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3nmrkrrjq.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3ppsahecq.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3crgzdmcu.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qssfbkaf.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3putpzrru.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hdzktgxq.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qyiuhosk.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3fxzymgfz.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3otcfqohi.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3rbdbjgfw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3hurdbfcz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cmgnysxk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kyxsbzft.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3nvrcsvuq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3cixfbisk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3xafmmurs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ikzvzpij.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3nchzbqiv.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3hlxltjso.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3aosmzbgw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhhpgpfu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vnvdxhwk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3okubleof.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3zmvltynn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3hpooycfw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3puqofmme.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpnwexaz.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3oagbmeum.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3sjxbsqkk.html


<!-- 参考信息 -->