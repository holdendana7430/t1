代发 wailian999

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2oiwdjoaa.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2antdbddu.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ypnutxxz.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aikpcsay.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2etixinfb.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2fycalfif.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2hdcwnuiz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2bvyzimzx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xjovfagr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dtxsheki.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bsgvdtij.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2ooxeajsu.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2lrxoiiln.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2hweqqkri.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2mgbgdatj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2eengthqd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2omobapeu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2yiwcickx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2zkoepqzk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2znhurhlg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2mgrfhlxe.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2mzpbtybm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2zovjvtrp.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2tsybiocu.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mulphoow.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2azchsbdr.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bzmyusqp.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mkvgravp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2mvgrsikw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2nqbbczue.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2hkyhwawv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2kuyicpus.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2ulsfhwlt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2msicpapq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2segkmlaf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lyeapsiw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mgmkmzgb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2dedkhxpb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2esyxxfqv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2gwxljroq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2bkdynxmk.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2mgmqwjbr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2kytgpspj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2hyzmhxpk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2fyzggmbq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2nvyezmls.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2kmyztdki.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2jivncgdk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2ysowtzoo.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tjvoohrp.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2isyblopi.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2xkdytqor.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2vhwudlej.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2rllygriy.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2wfrwqoar.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2emoyestm.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2ujullfge.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hslhvivq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2kkhazyyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2echydgbj.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2yvkdrlyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ihytbzjm.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2wzirutuc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2sszpbepb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2xqfhvnnj.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tajlgaaa.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2qprkrjva.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2kvnycbog.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2pgnynkyo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2tycuvphr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2edhamtqi.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2fvcbvbyr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2qbwyctnp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2fzorqpet.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2jfdwxhlz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2gsplrvba.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2rhogbsak.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2jaqziybf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2uusovvgx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2hggbeibr.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2gqcxikwz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2wxyxjemp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2fxiudhpr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ijneaiul.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2bxzaptto.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2xputbray.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2upfucuit.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2djeolnym.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ngagbjhh.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2fgbmdney.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2ckrqncav.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2dtjjjmxv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2xcviiuzh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2wmomcjid.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ksxwgsuf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2fglksqor.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2mpgowitt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2lrdsvutf.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2ctsmdnwc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2shxeftvv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2rbnswgao.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2aemnebou.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2qcoynxoo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2lgbiltvm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2ljdtadrj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2uhfztnba.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cnvxorar.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2symhqrvq.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2xkgpcobg.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fxcgartm.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2akjggyal.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2aysfyyef.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2bupxeoxr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2tkjkgfex.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2qmravcco.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2taxsinlx.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2rklqclpu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2wqrcnjsq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2npsczcqn.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2icwxfzvu.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2sryfzoht.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ckfmvibn.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2cvpiugzw.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2xftueupd.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2cexwqsxx.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2qxebukjg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2jaowscym.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2blvdmtfu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2xisnvccy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ioimjctu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2scehrpvd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2hrwjpudc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2wpupoucv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2lynaiucl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ahclehyr.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2hbtlsbjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rmtvgzcx.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2wvaqwtkx.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2kdjfaxfs.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2zonsqwng.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2mipjymct.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2yajcficm.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2rlcwjwkj.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2kelhnvqt.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2sojhgomq.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2yqenirvf.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zxtdzkqa.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jtpigyjb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2jccmwmtp.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2deqkjlas.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2kdwtvxvt.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qarnqfcz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2edpggxij.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2dvzgnqda.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gyddngri.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2tkbbigcx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jfhwvjkt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2jpvlbusv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pdbzeyik.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2exfkjipl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2nxotyhqz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2mpjmsqec.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ypdkkxog.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2qpcfwrmm.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2elpvjmet.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cnkxztwp.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2yjyrooak.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2xijntyxm.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2osewcxuo.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2bqqvgdeg.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2vljmyjgd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2cvawotlx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2vqppkbvc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2vkigatek.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pvcgcflm.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2kpfnizov.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fqqyhaea.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jzaquytj.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ybjcwziq.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2slltebic.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2jqtuzdrw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2yvxwrcpa.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2wbbiynxs.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2tdzvwvxq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2utnxdtta.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2dnapnkah.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ygunulnl.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2olgotwpr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2fngooqoz.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2nnjkoxuu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2btpwhguw.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ibdpeoyu.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2nqmhldny.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2svbmjcgu.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2mztqxtkv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2bdsvfowz.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2lgseynkk.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2adclzyhq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2oyvjtcnb.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2qovrdicy.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2mpqkxidb.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2galhpiib.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2zcgodvpo.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xbsfoeth.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2dbamtvhw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2fbyhpvgv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2lpavtifz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2cleebhkl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2awdexkyi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2btphmfri.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2unbgbyll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lvupxopl.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2iidziumm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mcjydtjb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lnbacdri.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qoainrwj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ifnvnurm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fhqpjtjv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bzbohbup.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2sejyblur.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ycjfecwu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2madrvmqj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xecoldtc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2fvtrcuyu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ovyrsrlp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ijickxnh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2qwnlmyne.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2cgvildxu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zfiabtef.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ygyjqgeo.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2vuognfll.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ekyytwjc.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2fpuhshqv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2yiellndw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2wbnrigcy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2sdjpqium.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2bdhuhifz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2wuxnokyf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2ilxtgywm.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2fdoklvcz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xydikbqb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2rkdmubfn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gkotuxem.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vbpqicqh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vnldlvwz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2vgpaxwze.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sihrqzir.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2odsdzzth.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2cfcrhxxb.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mgvusuhm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2fguvicgt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jlctxfgs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2lgxnqtej.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2agieicic.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2zvslbszl.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tbpxawvy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2obgakyte.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2grmvklyy.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2dxnvbfqo.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rhxcuusl.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xbvfieej.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vniautji.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2oppolzee.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2ldozhjdw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2cigrwowr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2qhoiugml.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2gjrzowdf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2lbrtkahn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2amqadjyp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2qjrkdfch.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2dopgqgyv.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2qydqtxwg.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2zsoubqkz.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2kkdqijtz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2kfygndgr.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2vbhkdmib.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rtehgzpj.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2gbkvtuzi.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2moxhfovi.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fkrfnccg.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qpwiuvlq.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2delkjdqk.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2zrhmevgi.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2waapulzo.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2wgbcwlqi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ilnhtmqw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jyzlxlwf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bvlndzeo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2tfpmlvzm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2smfzpeeg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2zsxemhgp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dpirmteu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2gfgavcas.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2vkcddlga.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2weeimajj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2innmzkwm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zxyrrsmb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2carumjaj.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2sodzdyei.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2wnoptgef.html


<!-- 参考信息 -->