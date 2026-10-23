代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3qwiegaaq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3rttymsbw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3fasgcfuy.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wucqsapu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3izghqurj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3exjvlxbi.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3onnyluiy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3bjxxyjbk.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3uulxlyjz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3oeqfhyka.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3zadzhmhh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3aqyvpset.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3axjukuoa.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ckihkiuw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3cxkbafrp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3bgluhsta.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3juwawmeh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ruqwplrf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3eqkledms.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3ngsnmlxq.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3uysnzqoe.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3oknbebcv.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qkxaihbj.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3skofpawv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3pddqziif.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3xhjonwiz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3dzsnxwik.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3vrewvbtj.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3dkbypyif.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3tknymwou.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3oxgdvffl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ilfxqfoe.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3lrjbrkia.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3ewbpfxtv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3eraonxak.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ekpdizji.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3dctxchiw.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3iwlvycmq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kswfpbyg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3pughnfrd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jgoekybi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3udvhutwk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vjznqrkg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3jgthprmy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3wnywhokn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qczzhoba.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3cztwpdpi.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3owtogdrl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bhdtxajp.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ggxfcccl.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3xwwsvhou.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3oyovhsgh.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3tlplyloz.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3beludlsx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3otbsskvx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mznpperb.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3dbnbhvdw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rbiejjtb.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3ahwovvxs.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3kfompxxx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3rtrjrzzr.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3opcgsixm.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3sskvcwjy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3rlxhlbdk.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ewsfezgb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3jsvvwkmo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3eobearvh.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3glnpuuxp.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ojppudjz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3vmurwhds.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3mbjcpyat.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3kcgkdsms.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3jxgqublk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3qklumfbm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3pwdqwlpv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3nhburdqt.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3zuzzhpuu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3jcmenkhk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ambybazv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3dpdkonxd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3xpfrlwsa.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3dqhhmawq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3qilnsusm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3hylrwjdw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ctjzccbt.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3uakvpdot.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3tydfkbqx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3rfsrybpg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3bpyukxor.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ramwlerm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3ebqjqrgg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3lnowhsch.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3ulqabrof.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3zaekisyb.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3ehfthugv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3drwvrvvl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3kpmrfezc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3rlawloex.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3inoqahlw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3efbduwlk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3crmpraan.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3dfwjmkzj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oihhhbqu.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3vhzwcnlq.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3mtlyopyo.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3orxnthjv.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3yhfrzcrq.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3bismyixa.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3lllmmuig.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3yurzjbjp.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3dicmjtkm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3yajwloie.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xvktazax.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3hkqkwlwt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3qywsqfhn.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3czkffcci.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ssgrtqlh.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3kiuzfqsu.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3msxtwwrc.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3kfxjkwqx.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3puwzhexu.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3gzxdfcqz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3obvjgijo.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3dyraaijw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3kangisbw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ducnamnq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3obtyndpa.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3asdhcrht.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3rfphfchk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vkoctcpv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sfgrbiob.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3kyksbnsi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yalhuqqg.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3njikovdz.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3xiimbvce.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3bporkshm.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wwhjhshw.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3wwvaeixf.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3cjljplnp.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3fsyxhqzj.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3bezzvxlq.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3xrciefuy.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3hnmlishm.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lipwcvkt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3gmfnzfxq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3mxrgtrzc.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3hbqdqbcb.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jdgscmod.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dpapjeov.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3cnofdhge.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zrobufkn.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3nitkkknc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3voflzczo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3tykzmjkt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3dknrztqv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gfeotzuq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ldisdods.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3oovmpooe.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3gtkficzx.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3uiqybilj.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3dcdpeckw.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3saxomxdp.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3wzuhyfzv.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3enuqtjon.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hdoevhtw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3esppzota.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3qjvnagmj.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3mmfrbkph.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3jplktbwj.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3dmncbgsr.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wwywvfrq.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ahhiellr.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3idhkhprz.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zxvbvkzv.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gyscxtbi.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3azwhbiwj.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3gmpagkjr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3ozsudjyx.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3qskoddou.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3lwjjtkmb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3pmczztws.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ckbjeeqo.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3cqyerlmr.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3auombqfx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3sptburmu.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3oawcpfwa.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yicveept.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3jaxlmwzb.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3flavnfyd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3hpnwonpl.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xutmvlbh.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xcvvtyyr.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qyzrmojz.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3hzbhxxrq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3dngsbhsu.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3omuytenc.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3crudlush.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3bhtbixuc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3qwweodiv.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ubzioqbd.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3eadplhzs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ioysjulg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3efevgukx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3jkxivmow.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3qcyvpueq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rckfavtf.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3lspsdgqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3plxzvnsg.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3wswvuzpx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uwokzeka.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nbzxvztl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xrvreonf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3pbcqarls.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3eacaxlco.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ktxalxhm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3fvzqwgdv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3stwfogxk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3suvydzya.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3wwnlkcix.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3kuqscxbn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3hgwqohbd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gtcjhjbx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ttzuryme.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3qsqfvhqs.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3cvufokzb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3peojnmbp.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3vqwnfcfi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3embkwcbt.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3qzfxztrs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3zwthvagk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3fwxwjjzz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3yceobdds.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3jgcjucoj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3yfogozsx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3owsxktya.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3aqimbged.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dwppxqzw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3iqqdewds.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3kcunzhqd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qfyrxfop.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3fpcnpehg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3wyhhfxdc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3wdwkqdqe.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dkhdqpyp.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3mawnmvie.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3amlvgpyr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkuyzqdd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgugpzkf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3guyfohdk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3xfmsiild.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3larbtsgm.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3rtxyvawb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ovnxtoks.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3zantgioy.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3odgbnemw.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hvmgdgnt.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pkihxkwl.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xxkxgrav.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3csgsfxgd.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3mxhxbbyu.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3cucdzshb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ftnpljxi.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3hxvvpqjs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3icnhwcxr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3bbawlfpr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3wvityrhu.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3adufuuwg.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3abxugwsp.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3pjovaeau.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ohpwbimg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3ufnkciss.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3gosgtgdf.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3dbbvgwzd.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3ojzctbph.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wyhnakvr.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3huyfvmsx.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tftkagyx.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qizzqwzl.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3hsxkqkhp.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3aknxyxwj.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3zjlomgph.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3hycgmxym.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qfkcaneb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rzdekjxv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3gdjnfthf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3aoipbcyq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3rduwwsqz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hnxkrphx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3gdjfxcsf.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3kfwxwuix.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3uylgqxfv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3rargjtqq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3wjcgppym.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3tdpgksgm.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3qakdmdec.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3twedgzox.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3gaifbgeu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3gijplwyu.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3fsivagdr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3tpkafpsq.html


<!-- 参考信息 -->