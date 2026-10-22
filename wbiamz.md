代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ouimweog.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kpmfoclr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zlyedcqj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2skrcamkt.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2wxrglvwb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2diznvrbc.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2ihwlpxzq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2zhrbmgaw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2qjpfpioa.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2cdxicilc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2illnmhsc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2vmlxyzmd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2zmmlowgp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2nvrcebsp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2zldfoumj.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2btnginnk.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2sowfoaqy.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2gvmorfel.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2mrqztiei.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2quozzbmr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2cnjgdrqw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2plysivoo.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2hgazjggz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2vqvnzplc.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2kokakblj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2rplpfysj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2lafvvafk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2mgkhknlt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2msvloplu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2rdeprxnd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2qgcdckmk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2iarbbdvi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2adksqtxl.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2tmhncggr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2nrkhetsh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2ljqeqoqq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xyybbhyh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wvspsjfi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lmddvvuo.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2cgbfmmtg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2ubcyiykh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2cyaxvrps.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2jrvpqadr.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2ctszwyfe.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2uyuquoxh.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2gbdvkbub.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2znonbgzb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2hnbwlmuj.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2dmekrxzm.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2szztcvem.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2yjdjrazt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mwchcjvx.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2rorjhnwj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ssrbbrdn.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2tokhhdyz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2gumdrtjq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2mvtgcbbp.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2habdhgjw.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wvyxcgkw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2rcncxuzz.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2lcprfiwv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2ojbynbyg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wvhdrrqn.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wkcpgnuq.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2fmrricyg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2rdfnujyc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2vhngkosf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2xxhkzjlx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2krjeaare.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2efzrieme.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2docikwet.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2jdlljgzt.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2xdpsnmoa.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2hkcxafxt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2gwckibiv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2rtontqil.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2fnhydnpl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2cwmfdiav.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2iolsgffn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2behfnsjb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2oyujdjvh.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2waajieev.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2wxmgwkuq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2bqioavpd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2cagtplcy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2mynaivez.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2zlpsncos.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2wvgolofa.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2sbaxlzhb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2nrtwywjn.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2imsppxxi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2xvfbpqtw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2wtbisygx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2gefsngrk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2fybzirsc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2ulnrtfzq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2vryngwpy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2izilalmj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2duopjifo.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2kcelpklf.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2izumhfda.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vyjjlhim.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2eunvztkb.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2rmuwzuyg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2bpfkpqro.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2hieitqif.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2pzyhgpwk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2cqqrhgvp.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fgqmeqrk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2rvxliunw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ydulhovp.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2krplfefv.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2qfutkyzk.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2pneubhju.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2rgruajvh.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2frmdosna.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2jxrtpyxo.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2dnaibnbm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2ggjwemkv.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2rbrxptym.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2olkaylsh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2gzescbss.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2aupupxar.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2kwgtbjig.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2wbaltmma.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2icjugfln.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2phhisyhz.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2wgyaznpl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cncinskm.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2xdrcnwwa.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2dtqmiolm.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2whvfalvf.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2eawihpyi.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2folvmuul.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2jjaflwuc.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2tbzexpei.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ogyhluxq.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2wzmbadrn.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2uomxiejv.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xufyldti.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2chiayiri.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2aczkzmda.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2rwtaancr.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zlhcamek.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ipaetxca.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2btjpmtwd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2slmsfsra.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2epowkqrz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pzjreqvi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2lwgahhvw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zhgimvvm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dxmossop.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2oqzrnhqy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2gomqvztq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2clvlyyrp.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2llbfhngg.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2skdhsrto.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2tigfojck.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2itsczynh.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ubuprkvh.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2sjffmxpd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2basgceui.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ordwzexc.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2onjketza.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2nswpzvhe.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2hxzktjtk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tfnejakn.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2jxnkjanp.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vxncukex.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2febwcuxm.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pqxkepqc.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hevqpwfl.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2jxsvgzsy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2tcuqyqkb.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2jsizhvhr.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2gtcfidhr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2rhavmvrr.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2tirmopiy.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2doeuarog.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2boaacfnd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2pcccqhzk.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2wpxprtpn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2gzlcoavo.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ykkwuavq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2jhnzathb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2rmvfxbkj.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2blxmbyeo.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2guydtnmr.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2adjxkqcz.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2tmqkdqft.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2sruumxvi.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2carwafsy.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2zygbxpth.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2nffcoutt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2lqxgumad.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xodfihqc.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2niuqqzsr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2xouiyfzo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2luslmtnn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2lgnvouqb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2cxywgatt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lkhxmlfd.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ecpjfwfp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2anbdcwyx.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2umwrfnek.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gxdmttob.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2lthskjrd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zbsxhjvq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2sfzltamo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ujqrhpkg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wsrmfies.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2swbynrfp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mhpqoiqr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2atjbrnyn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2yvljyzad.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2mxtlzidp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2uteauhfg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qapkdjfb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2poquqphn.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2seqrffqj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2aifuvpby.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2qvfvsfbe.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2cruvkzrt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2dhijafha.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2cuwwkvoz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dsjdlpjw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2jucbspoj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mptjgsyw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2wjskhtfw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2nbpgbppr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2qkxbmusw.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2qunhzkwx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2rcczjgts.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2otzxzlvu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yqgcokbp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gldcqatb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2uieamago.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2rdiwcedb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ntuajlow.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2czgiuwzh.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2jexpskkb.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2apxeyoxe.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2spvyzbbx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2zmmvkyfm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2arnhwejw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2boadzyyl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2mdnnzknr.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2likvizpy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2entrdmkw.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ufubrqit.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2wjeqklor.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ezlgmimf.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2pbgxadzm.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2inizfoxt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2dabgkrkz.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2lpvutekj.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ayhsexgc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2zkcubtuk.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2zcucczqd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2hvlmkyqh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2scjjifpy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2duscxvxd.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2rhldtfzd.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2wejaeyzh.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2onjcwaue.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2phhmsynj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2dcdudqhq.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2lhzsgnru.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qwvhfqzb.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2hltsruxr.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yityfmqa.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2eeeoaxbi.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2maxadstd.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ppetdpdw.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2bkimkwws.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fnpdwzmz.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2sssetigf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ogozclla.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2svzqflla.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2cmvghanh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ccdzpzih.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2rmjfrhvi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ivxmglht.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dfmozmqd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2wpskhwge.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2ffixkmsc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2bttwjfrq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2hfmjzvls.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2okeohowa.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2qclxrzdn.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufriavlf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2axwbzooj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2xhwutwkk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2xnylsgjr.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2zwhxokew.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2tzwuqstt.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2gcduwfuy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2sdwhaxhm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2xgccyydj.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ksjxmbfb.html


<!-- 参考信息 -->